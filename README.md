# Multi-label-Text-Classification

พัฒนาระบบจำแนกประเภทข้อความร้องเรียนจากแพลตฟอร์ม **Traffy Fondue** เพื่อระบุหน่วยงานรัฐที่เกี่ยวข้อง (Multi-label Classification) 

## 🛠️ Tech Stack & Methodology
- **Model:** Fine-tuned `PhayaThaiBERT` (Thai-English Bilingual Model)
- **Library:** HuggingFace Transformers, PyTorch, Pandas
- **Techniques:**
  - **Text Preprocessing:** จัดการกับข้อความผสมภาษาไทย-อังกฤษ และอักขระพิเศษ
  - **Handling Imbalance:** แก้ปัญหา Data Imbalance (บางคลาสมี < 1%) ด้วยเทคนิค *Class-specific Threshold Optimization and Focal Loss*
  - **Evaluation:** เน้นการวัดผลด้วย **Macro F1-score** เพื่อให้มั่นใจว่าโมเดลทำนายคลาสที่มีข้อมูลน้อยได้อย่างแม่นยำ


## 🚀 Quick Links
- **Code & Outputs** [Open in Google Colab With Outputs](https://colab.research.google.com/drive/117QqzOXCzVF3nzwbvkIiBpySPNIzV5rP?usp=sharing)