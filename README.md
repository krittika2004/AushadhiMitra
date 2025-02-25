# AushadhiMitra - Pharmacist's Assistant

## Brief Summary
A Pharmacist’s assistant that automatically reads handwritten prescriptions and converts them into digital text using a Vision Language Model (VLM). This solution enhances prescription clarity, reducing medication errors and automating record-keeping for pharmacies.

## Problem Statement
Handwritten prescriptions are often difficult to read, leading to potential medication errors for patients and manual transcription burdens for pharmacists. This system leverages a VLM to digitize prescriptions, ensuring accurate medicine dispensing and automated data entry.

## Access code
You can access the jupyter notebook to view the code.

## Design Idea and Approach
### Technologies proposed to be Used:
- **VLM**: Open-source models like Ollama for handwriting recognition.
- **Backend**: Python (FastAPI/Flask) for data processing.
- **Frontend**: Streamlit for a simple UI.
- **Deployment**: Google Colab/Kaggle for testing, Streamlit Cloud/Hugging Face Spaces for deployment.
- **Storage**: Firebase/Google Sheets for structured data storage.

### Implementation Plan:
1. Build a pipeline to extract text from handwritten prescriptions using a VLM.
2. Develop a web-based app for users to upload prescription images.
3. Process and structure the extracted text for easy access and record-keeping.

### Scaling Considerations:
- Supports small image files (~5MB per prescription).
- Initial system handles ~10 queries per second (QPS), scalable as needed.

### Rollout Strategy:
1. **Phase 1**: Prototype on Google Colab/Kaggle.
2. **Phase 2**: Deploy a basic version via Streamlit Cloud.
3. **Phase 3**: Scale with pharmacy integrations.

### Algorithm Approach:
- VLM for zero-shot handwriting recognition.
- Preprocessing to improve text extraction quality.
- Postprocessing to structure extracted data efficiently.

## Impact
This project directly addresses the issue of illegible prescriptions that contribute to medication errors. By automating transcription, it ensures prescription clarity, improves patient safety, and streamlines pharmacy workflows. Grounded in existing research on AI-based handwriting recognition, the solution will be deployed via cloud-based and app solutions for real-world impact.

## Feasibility
- **Technical Feasibility**: The project relies on open-source, cloud-deployed VLMs like Ollama and Qwen.
- **Data Availability**: Freely available datasets on handwritten medical prescriptions can be used for fine-tuning.
- **Expert Involvement**: Identifying domain experts for validation and real-world application.

## Use of AI
This solution applies Vision Language Model (VLM) AI to extract text from handwritten prescriptions and generate structured digital records, significantly improving prescription readability and pharmacy efficiency.

## Alternatives Considered
- **OCR Models**: Traditional OCR models require extensive training on diverse handwriting styles and are prone to errors, whereas VLMs can perform zero-shot inference with high accuracy.
- **Closed-Source Models**: GPT-4o and Gemini Flash 2.0 provide high accuracy but are not open-source and may have access restrictions.
- **Qwen API**: While a great option, Qwen’s API is not available in India, and local deployment was infeasible due to hardware constraints.

## References and Appendices
### Public Datasets Used:
- [Illegible Medical Prescription Images Dataset](https://www.kaggle.com/datasets/mehaksingal/illegible-medical-prescription-images-dataset/data)
- [Doctors’ Handwritten Prescription Dataset (Bangladesh)](https://www.kaggle.com/datasets/mamun1113/doctors-handwritten-prescription-bd-dataset)
- [IAM Handwritten Forms Dataset](https://www.kaggle.com/datasets/naderabdalghani/iam-handwritten-forms-dataset)

## Diagram for Proposed Solution

![image](https://github.com/user-attachments/assets/3112647f-289f-42c4-92a8-033e9a4ba3c3)
