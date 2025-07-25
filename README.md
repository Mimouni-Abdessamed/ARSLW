# ARSLW Dataset: Arabic Sign Language Words (84,000+ Images)

## Dataset Overview

The ARSLW dataset contains over **84,000 real-time hand gesture images** representing Arabic Sign Language (ARSL) words. This dataset was created using a custom webcam-based tool to ensure high-quality, clean input from real signers.

- Suitable for: computer vision, deep learning, gesture recognition, and assistive applications  
- Format: JPG images, all resized to **224x224** pixels  
- Number of Categories: 5 (Colors, Health, Education, Family, Verbs)  
- Image Count: Roughly **200–6000 images per word**  
- Language: **Arabic word labels** for real-world relevance  

---

## Folder Structure

```
ARSLW
├── Dataset
│ ├── Colors
│ │ ├── أبيض
│ │ ├── أحمر
│ │ ├── أخضر
│ │ ├── أزرق
│ │ ├── أسود
│ │ ├── بنفسجي1
│ │ ├── بنفسجي2
│ │ ├── بني
│ │ └── وردي
│ ├── Health
│ │ ├── حرارة
│ │ ├── سعال
│ │ ├── إبرة
│ │ ├── أكسجين
│ │ ├── ألم
│ │ └── ميزان حرارة
│ ├── Education
│ │ ├── مدرسة
│ │ ├── معلم
│ │ ├── واجب
│ │ └── فصل
│ ├── Family
│ │ ├── أم
│ │ ├── أب
│ │ ├── أخ
│ │ └── أخت
│ └── Verbs
│ ├── أكل
│ ├── شرب
│ ├── نام
│ └── استيقظ
├── tools
```
- Each folder inside a category corresponds to a specific Arabic sign word.  
- Inside each word folder, you'll find **JPG images** of real signers performing the gesture.  
- All images are captured uniformly in controlled lighting conditions with a plain background.  

---

## How the Data Was Collected

We used a **custom Python tool built with OpenCV** to capture and resize each frame to 224x224 pixels.

- Gesture input was typed (e.g., "أحمر", "أكل") and recorded using a laptop webcam  
- Each image was automatically saved every 0.5 seconds  
- Tool ensured consistent formatting across all classes  

**Tool used:**  
[gesture-capture-tool/DataSetMaker.py](https://github.com/Mimouni-Abdessamed/gesture-capture-tool/blob/master/DataSetMaker.py)

---

## Additional Datasets Used

To enhance model robustness and expand gesture coverage, we also integrated and learned from other ARSL datasets:

1. **ARSL No Background V2** (by Rabie El Kharoua)  
   - [https://www.kaggle.com/datasets/rabieelkharoua/arsl-no-background-v2](https://www.kaggle.com/datasets/rabieelkharoua/arsl-no-background-v2)  
   - Licensed under **Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)**  
   - See: [https://creativecommons.org/licenses/by-sa/4.0/](https://creativecommons.org/licenses/by-sa/4.0/)

2. **ASLAD Arabic Sign Language Alphabet Dataset (190k images)** (by Salma Selmoghazy)  
   - [https://www.kaggle.com/datasets/salmaselmoghazy/aslad-190k-arabic-sign-language-alphabet-dataset](https://www.kaggle.com/datasets/salmaselmoghazy/aslad-190k-arabic-sign-language-alphabet-dataset)  
   - Licensed under **Attribution 4.0 International (CC BY 4.0)**  
   - See: [https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/)

These external datasets were used for:

- Additional training and validation  
- Expanding gesture variation and signer diversity  
- Improving recognition of fingerspelling-based signs  

We provide proper attribution as required by these licenses and comply with their terms.

---

## Reference and Accuracy

All signs were manually referenced from the official **Zayed Higher Organization's Arabic Sign Language Dictionary**:  
[UAE Arabic Sign Language Dictionary Gallery](https://zho.gov.ae/en/Sign-Language-Dictionary/UAE-Sign-Language-Categories/Arabic-Sign-Languages#gallery)


We ensured sign accuracy by:

- Carefully learning from video examples in the dictionary  
- Having real people replicate the signs as closely as possible  
- Capturing in realistic conditions (natural hand positioning and motion)  

---

## Use Cases

This dataset is ideal for:

- Training ARSL gesture recognition models (CNNs, MediaPipe, etc.)  
- Building translation tools for Arabic Sign Language  
- Research in sign language linguistics  
- Developing assistive mobile or web applications for the deaf community  

---

## Notes

- Some gestures may contain slight variations due to signer posture and lighting  
- Words with multiple sequential signs (e.g., بنفسجي1 and بنفسجي2) represent gestures that require **more than one sign in sequence** to express a complete word  
- Dataset is continually expandable using the provided tool  

---

## Important Notes

- This dataset reflects **real-world variability** in sign performance.
- Some minor inconsistencies may occur due to lighting, positioning, or movement — mimicking natural signing environments.
- Ensure ethical and responsible use.
- Please **cite this dataset** in your research or public applications.

---

## Author & Contact

- **Author:** Mimouni Abdessamed  
- **Email:** abdessamedfreelance@gmail.com  
- **GitHub:** [Mimouni-Abdessamed](https://github.com/Mimouni-Abdessamed)

---
## Contributors

- **Meniri Younes**

- **Ouici Zin Abidine** — [GitHub: X0echo](https://github.com/X0echo)

- **Brahami Sidou** — [GitHub: Sidou104](https://github.com/Sidou104)

- **Bellaoudj Younes**

- **Belhachemi Anes** — [GitHub: anes-bela](https://github.com/anes-bela)

---
## License

This dataset is released under the **MIT License**.  
You are free to use, modify, and distribute it with proper attribution.

See the `LICENSE` file for full terms.
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)

