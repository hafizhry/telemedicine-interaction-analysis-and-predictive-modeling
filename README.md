# Telemedicine Interaction Analysis and Predictive Modeling

## Project Overview
This repository contains the implementation and results of the final term project for HS650 Fall 2024 at the University of Michigan School of Nursing. The project leverages machine learning and natural language processing techniques to analyze telemedicine interaction data and generate actionable insights for improving healthcare service delivery. 

The project focuses on three key areas:
1. **Simplifying Pregnancy-Related Answers**: Grouping diverse pregnancy-related queries into three themes to streamline information for expectant mothers.
2. **Triage Prioritization for HIV-Related Questions**: Developing a predictive triage model to prioritize high-risk consultations.
3. **Conversation Generation**: Creating synthetic patient-physician conversations in Indonesian and English using OpenAI's GPT-4o-mini API.

---

## Key Features

### 1. Simplifying Pregnancy-Related Answers
- **Goal**: Streamline support for expectant mothers by clustering pregnancy-related consultations into three themes:
  - **Pregnancy Progression and Maternal Health**
  - **Early Pregnancy Signs and Hormonal Concerns**
  - **Fertility, Conception, and Sexual Health**
- **Method**: K-means clustering with TF-IDF vectorization and visualization using t-SNE.

### 2. Triage Prioritization for HIV-Related Questions
- **Goal**: Prioritize high-risk HIV-related consultations to enhance response times.
- **Method**:
  - **Clustering Analysis**: Segment questions into six clusters using k-means.
  - **Predictive Analysis**: Train an LDA-based triage prediction model with 95.72% accuracy.

### 3. Conversation Generation
- **Goal**: Create a dataset of synthetic patient-physician conversations in Indonesian and English for training large language models (LLMs).
- **Method**: Use OpenAI GPT-4o-mini API with prompt engineering for contextual and anonymized conversation generation.

---

## Results

### Pregnancy-Related Consultations
- Grouped into three clusters:
  - Pregnancy Progression and Maternal Health
  - Early Pregnancy Signs and Hormonal Concerns
  - Fertility, Conception, and Sexual Health

### HIV-Related Consultations
- Clustered into six themes with triage priorities assigned:
  - Sexual Relationships and Protection (Low Priority)
  - Unprotected Sexual Activity Risks (High Priority)
  - Testing and Diagnosis (Medium Priority)
  - HIV/AIDS Awareness and Symptoms (High Priority)
  - Potential Exposure to Viruses (Medium Priority)
  - Treatment and Recovery Support (High Priority)

### Predictive Triage Model
- Achieved 95.72% accuracy using Linear Discriminant Analysis (LDA).

### Synthetic Conversations
- Generated question-answer pairs in Indonesian and English using OpenAI GPT-4o-mini API.

---

## References
- Juanita, Safitri; Purwitasari, Diana; Purnama, I Ketut Eddy; Purnomo, Mauridhi (2023), “Doctor’s Answer Text Dataset in Indonesian Contains Information on Medical Interview Patterns”, Mendeley Data, V1, doi: [10.17632/p8d5bynh3m.1](https://doi.org/10.17632/p8d5bynh3m.1).

- S. Juanita, D. Purwitasari, I. Ketut Eddy Purnama, A. Famasya Abdillah and M. H. Purnomo, “Topic Modeling for Online Health Consultation on Low-Risk Diseases,” 2024 International Seminar on Intelligent Technology and Its Applications (ISITIA), Mataram, Indonesia, 2024, pp. 196-201, doi: [10.1109/ISITIA63062.2024.10667722](https://doi.org/10.1109/ISITIA63062.2024.10667722).

- Wang, Junda & Yao, Zonghai & Yang, Zhichao & Zhou, Huixue & Li, Rumeng & Wang, Xun & Xu, Yucheng & Yu, Hong. (2024). NoteChat: A Dataset of Synthetic Patient-Physician Conversations Conditioned on Clinical Notes. 15183-15201. doi: [10.18653/v1/2024.findings-acl.901](https://doi.org/10.18653/v1/2024.findings-acl.901).

- OpenAI API Documentation. [https://platform.openai.com/docs/overview](https://platform.openai.com/docs/overview).
