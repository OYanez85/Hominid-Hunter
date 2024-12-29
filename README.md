# Hominid-Hunter
Evolution of Humans DataSets for Clasification

# Hominid Hunter: Evolutionary Insights from the Past

## Project Overview
**Hominid Hunter** is a machine learning project designed to analyze and predict evolutionary characteristics of ancient hominids. Using a comprehensive dataset, the project classifies hominids by genus, species, and locomotion type (bipedal or not) while uncovering patterns in human evolution.

---

## Dataset
The dataset contains **12,000 rows and 28 columns**, covering a range of features:
- **Genus & Species**: Taxonomic information for classification.
- **Time Period**: Chronological context of each hominid.
- **Geographical Features**: Location, Zone, Current Country.
- **Morphological Traits**: Cranial capacity, height, incisor size, jaw shape, etc.
- **Behavioral Traits**: Technological presence, diet, migration patterns.
- **Bipedalism**: Indication of bipedal locomotion.

---

## Objectives
1. **Classify Hominids**:
   - By `Genus & Species`.
   - By bipedal locomotion (`Biped`).
2. **Feature Importance Analysis**:
   - Identify key features influencing predictions.
3. **Build and Evaluate Models**:
   - Use optimized Random Forest classifiers.
   - Ensure generalizability with cross-validation.

---

## Steps in the Project

### 1. Preprocessing
- Missing values filled using the column mode.
- Categorical features encoded with `LabelEncoder`.
- Numerical features standardized using `StandardScaler`.

### 2. Exploratory Data Analysis (EDA)
- Distribution visualizations for `Biped` and `Genus & Species`.
- Feature importance analysis using Random Forest classifiers.

### 3. Model Training
- Separate models built for:
  - `Genus & Species Classification`
  - `Biped Classification`
- Models optimized using **GridSearchCV** for hyperparameter tuning.

### 4. Evaluation
- Metrics:
  - **Classification Report**: Precision, Recall, F1-score.
  - **Cross-validation Accuracy**: Stratified 5-fold.
- Visualized feature importance for interpretability.

---

## Results

### Genus & Species Classification
- **Accuracy**: 100%
- **Top Features**:
  - Habitat
  - Current Country
  - Time

### Biped Classification
- **Accuracy**: 100%
- **Top Features**:
  - Time
  - Sexual Dimorphism
  - Technology Presence

---

## How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/your-repo/hominid-hunter.git
   cd hominid-hunter
