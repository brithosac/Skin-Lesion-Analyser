## Technical Report: Multi-class Skin Cancer Image Classification
Brittney Hosac<br>
June 2020

### Problem Statement
Depending on the type, skin cancer can grow rapidly and become life-threatening if not treated early. 

### Skin Cancer Background

<b>nv</b>
Melanocytic nevi are benign neoplasms of melanocytes and appear in a myriad of variants, which all are included in our series. The variants may differ significantly from a dermatoscopic point of view.
[6705 images]

<b>mel</b><br>
Melanoma is a malignant neoplasm derived from melanocytes that may appear in different variants. If excised in an early stage it can be cured by simple surgical excision. Melanomas can be invasive or non-invasive (in situ). We included all variants of melanoma including melanoma in situ, but did exclude non-pigmented, subungual, ocular or mucosal melanoma.
[1113 images]
M
<b>bkl</b><br>
"Benign keratosis" is a generic class that includes seborrheic ker- atoses ("senile wart"), solar lentigo - which can be regarded a flat variant of seborrheic keratosis - and lichen-planus like keratoses (LPLK), which corresponds to a seborrheic keratosis or a solar lentigo with inflammation and regression [22]. The three subgroups may look different dermatoscop- ically, but we grouped them together because they are similar biologically and often reported under the same generic term histopathologically. From a dermatoscopic view, lichen planus-like keratoses are especially challeng- ing because they can show morphologic features mimicking melanoma [23] and are often biopsied or excised for diagnostic reasons.
[1099 images]

<b>bcc</b>
Basal cell carcinoma is a common variant of epithelial skin cancer that rarely metastasizes but grows destructively if untreated. It appears in different morphologic variants (flat, nodular, pigmented, cystic, etc) [21], which are all included in this set.
[514 images]

<b>akiec</b><br>
Actinic Keratoses (Solar Keratoses) and intraepithelial Carcinoma (Bowen’s disease) are common non-invasive, variants of squamous cell car- cinoma that can be treated locally without surgery. Some authors regard them as precursors of squamous cell carcinomas and not as actual carci- nomas. There is, however, agreement that these lesions may progress to invasive squamous cell carcinoma - which is usually not pigmented. Both neoplasms commonly show surface scaling and commonly are devoid of pigment. Actinic keratoses are more common on the face and Bowen’s disease is more common on other body sites. Because both types are in- duced by UV-light the surrounding skin is usually typified by severe sun damaged except in cases of Bowen’s disease that are caused by human papilloma virus infection and not by UV. Pigmented variants exists for Bowen’s disease [19] and for actinic keratoses [20]. Both are included in this set.
[327 images]

<b>vasc</b><br>
Vascular skin lesions in the dataset range from cherry angiomas to angiokeratomas [25] and pyogenic granulomas [26]. Hemorrhage is also included in this category.
[142 images]

<b>df<b/><br>
Dermatofibroma is a benign skin lesion regarded as either a benign proliferation or an inflammatory reaction to minimal trauma. It is brown often showing a central zone of fibrosis dermatoscopically [24].
[115 images]


<b>[Total images = 10015]</b>

### Data
Skin Lesion metadata and images were gathered from [Harvard Dataverse](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DBW86T)<br>

### EDA and Image Preprocessing
Began with [Metadata EDA](https://github.com/brithosac/Skin-Lesion-Analyser/blob/master/code/01_Metadata_EDA.ipynb).


![Diagnostic Class Distribution](https://github.com/brithosac/Skin-Lesion-Analyser/blob/master/assets/Distribution%20of%20Diagnostic%20Categories.png)


### Model Summaries



### Conclusion and Recommendations
Depending on the type, skin cancer can grow rapidly and become life-threatening if not treated early. If you’re one to forget your sunscreen or if your family has a history of skin cancer don’t forget to [App Name]. 
Follow up: adding metadata to CNN model to strengthen image classification
- [App Name] is not intended for final diagnostic conclusion.
- Follow up with medical professional to confirm the results of skin lesion classification by [App Name]. 