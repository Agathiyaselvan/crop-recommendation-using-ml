 Crop Recommendation using Machine Learning

**Irrigreat**

 **Problem Definition**
Agricultural productivity needs to be increased so that farmers can maximize their yield from the same piece of land without degrading the soil. Several challenges contribute to reduced productivity:

- Indian farmers struggle to choose the right crop based on their soil requirements, which depend on factors such as Nitrogen (N), Phosphorus (P), Potassium (K), temperature, humidity, rainfall, and pH levels.
- Farmers are often unaware of the appropriate organic or standard fertilizers to use based on soil conditions.
- Inadequate and imbalanced fertilization leads to soil degradation, nutrient mining, and second-generation nutrient management problems.
- According to the Associated Chambers of Commerce and Industry of India, annual crop losses due to pests amount to Rs. 50,000 crore.

---

### **Objective**
This project aims to implement precision agriculture—a modern farming technique that utilizes research data on soil characteristics, soil types, and crop yield data collection. The main objectives include:

- Suggesting the right crop for farmers based on site-specific parameters to prevent wrong crop choices and increase productivity.
- Developing a recommendation system using an ensemble model with a majority voting technique to ensure high accuracy and efficiency in crop selection.
- Recommending fertilizers based on N, P, K values and the selected crop.
- Recognizing pests and recommending appropriate pesticides available in India as per ISO standards.

---

### **Methodology**

#### **Crop Recommendation**
1. **Dataset Acquisition**
   - Collecting soil and environmental parameter data.
2. **ML Model Training & .pkl File Creation**
   - Using an ensemble technique with majority voting among:
     - Support Vector Machine (SVM)
     - Random Forest
     - Naïve Bayes
     - k-Nearest Neighbors (kNN)
3. **Crop Recommendation**
   - Loading the trained `.pkl` model to recommend a crop based on input data.

#### **Fertilizer Recommendation**
1. **Dataset Acquisition**
   - Collecting NPK values for different crops from:
     - The Fertilizer Association of India
     - Indian Institute of Water Management
2. **Input Values Processing**
   - Comparing desired vs. actual NPK values:
     - High
     - Low
     - Upto the mark
3. **Dictionary-Based Suggestions**
   - Providing fertilizer solutions from verified sources.

#### **Pesticide Recommendation**
1. **Data Acquisition**
   - Image scraping from Google Images to gather pest data.
2. **Data Cleaning & Augmentation**
   - Removing irrelevant content and increasing dataset variability.
3. **Deep Learning Model Creation**
   - Training a model for pest detection and pesticide recommendation.

---

### **Conclusion**
India's farmers work hard to feed a population of nearly 1.4 billion. However, their productivity is often threatened by natural factors that can damage crops and livelihoods. This solution aims to:

- Maximize agricultural productivity.
- Reduce soil degradation.
- Provide informed recommendations for organic and chemical fertilizers.
- Suggest the most suitable crop based on multiple attributes.
- Address pest control effectively.

By implementing this system, both farmers and the environment will benefit from comprehensive predictions and precise recommendations.
