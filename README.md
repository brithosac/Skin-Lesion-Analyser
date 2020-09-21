## Technical Report: Multi-class Skin Cancer Image Classification
Brittney Hosac<br>
June 2020

### Skin Cancer Statistics 
Information was sourced from [The Skin Cancer Foundation](https://www.skincancer.org/?gclid=CjwKCAjw5vz2BRAtEiwAbcVIL8mqF-E6D7wMD43ae4LYM1CludUDQgRf4h0RwJz7hGPlj8IALD_P8RoCwdkQAvD_BwE)
- More people are diagnosed with skin cancer each year in the United States than all other cancers combined. 
- In the U.S., more than 9,500 people are diagnosed with skin cancer every day. 
- 1 in 5 Americans will develop skin cancer by the age of 70.
- The annual cost of treating skin cancers in the U.S. is estimated at $8.1 billion.

### Problem Statement
 
99% of all skin cancer cases are curable if they are diagnosed and treated early enough. Monthly self examinations and yearly check-ups are important but a majority of the population doesn't follow this recommendation.

<b>How can early detection become more managable?</b>

Skin cancer is the cancer you can see and having a visual on the problem is a powerful tool that the public can utilize to detect cancer early when it's easiest to cure, before it can become dangerous, disfiguring or deadly. The goal is to create an online tool that can notify everyday people the three highest probability diagnoses for a given skin lesion. If a potentially dangerous diagnosis has a high probability then there would be more insentive to follow up with a medical professional.


### Data
Skin Lesion metadata and images were gathered from [Harvard Dataverse](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DBW86T)<br>

### Data Overview

![Examples of Each Cancer Class](https://github.com/brithosac/Skin-Lesion-Analyser/blob/master/assets/category_samples.png)

<b>Melanocytic nevi (nv)</b><br>
Melanocytic nevi are benign pigment-producing skin cells commonly called birth marks or moles that rarely become cancerous.<br>
[6705 images]

<b>Benign Keratosis-like Lesions (bkl)</b><br>
Benign keratosis is a generic class and one of the most common benign skin growths in older adults.<br>
[1099 images]

<b>Melanoma (mel)</b><br>
When detected early, the 5-year survival rate for melanoma is 99% but even still, an estimated 6,850 people will die of melanoma in 2020. Of those, 67% will be men and 33% will be women.<br>
[1113 images]


<b>Basal Cell Carcinoma (bcc)</b><br>
Basal Cell Carcinoma is the most common form of skin cancer and an estimated 4.3 million cases of BCC are diagnosed in the U.S. each year.<br>
[514 images]

<b>Actinic Keratoses (akiec)</b><br>
Actinic Keratoses are the most common precancer (3 million US cases per year) and because it can become cancerous, it's usually removed as a precaution once identified. Actinic Keratoses progress to Squamous cell carcinoma (SCC), which is the second most common form of skin cancer, in fact, more than 1 million cases of SCC are diagnosed in the U.S. each year. <br>
[327 images]

<b>Vascular skin lesions (vasc)</b><br>
Vascular skin lesions are relatively common abnormalities of the skin and underlying tissues, more commonly known as birthmarks.<br>
[142 images]

<b>Dermatofibroma (df)</b><br>
Dermatofibroma is a benign skin lesion regarded as either a benign proliferation or an inflammatory reaction to minimal trauma. Dermatofibromas are common benign fibrous nodules that most often arise on the skin of the lower legs.<br>
[115 images]

<b>[Total images = 10015]</b>

### Exploratory Data Analysis
[Metadata EDA](https://github.com/brithosac/Skin-Lesion-Analyser/blob/master/code/01_Metadata_EDA.ipynb).


![Diagnostic Class Distribution](https://github.com/brithosac/Skin-Lesion-Analyser/blob/master/assets/Distribution%20of%20Diagnostic%20Categories.png)


### Model Summaries

- [Simple CNN](https://github.com/brithosac/Skin-Lesion-Analyser/blob/master/code/02-cnn-model.ipynb)
 - 77% accuracy in classification of individual cancer classes
- [MobileNet](https://github.com/brithosac/Skin-Lesion-Analyser/blob/master/code/03-mobilenet-cnn-model.ipynb)
 - 82% accuracy in classification of individual cancer classes
 - 89% accuracy in classification of top 2 probable cancer classes
 - 96% accuracy in classification of top 3 probable cancer classes

![Accuracy: True class within top 3 predicted classes](https://github.com/brithosac/Skin-Lesion-Analyser/blob/master/assets/top_three.png)

![Confusion Matrix](https://github.com/brithosac/Skin-Lesion-Analyser/blob/master/assets/confusion%20matrix.png)

### Conclusion

Goals and next steps:<br>
- Continue to train various Neural Networks for higher accuracy
- Make the desired online tool, SkinScreen, a reality
    - Deploy website or mobile app for general public
- Users are able to submit a picture of a skin lesion and get the three highest probability diagnoses for a given skin lesion instantly.

Recommendations:<br>
- Depending on the type, skin cancer can grow rapidly and become life-threatening if not treated early. 
- Examine your skin once a month and See your dermatologist annually
- Wear Sunscreen everyday and as an extra precaution, don’t forget to SkinScreen
    - Not intended for final diagnostic conclusion; please seek medical follow up with dermatologist to confirm the results of skin lesion classification by SkinScreen. 
