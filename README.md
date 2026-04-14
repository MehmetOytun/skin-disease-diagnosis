# Skin Disease Diagnosis System

## English

Artificial Neural Networks course project - 3 person team.

### Team Members

| Name | Student ID | Model |
|------|-----------|-------|
| Mehmet Oytun ÖZER | 23040301043 | DenseNet121 |
| Furkan Işık | 23040301063 | ResNet50 |
| Ali Çelik | 23040301059 | EfficientNet-B3 |

### Project Description

CNN Ensemble based skin disease diagnosis system. Each team member trained a different CNN model on a curated subset of the DermNet dataset. Final prediction is made by combining all models with Soft Voting.

### Dataset

| | |
|---|---|
| **Name** | DermNet (6-class subset) |
| **Total images** | ~6,500 |
| **Classes** | 6 skin diseases |
| **Split** | Train %85 \| Validation %15 \| Test (separate folder) |

**Selected Classes:**
1. Acne and Rosacea Photos
2. Eczema Photos
3. Psoriasis pictures Lichen Planus and related diseases
4. Urticaria Hives
5. Nail Fungus and other Nail Disease
6. Scabies Lyme Disease and other Infestations and Bites

### Models

| Model | Developer | Framework |
|-------|-----------|-----------|
| DenseNet121 | Mehmet Oytun ÖZER | PyTorch (Windows) |
| ResNet50 | Furkan Işık | PyTorch (Windows) |
| EfficientNet-B3 | Ali Çelik | PyTorch (Windows) |

### Ensemble Method

| | |
|---|---|
| **Method** | Soft Voting |
| **Final prediction** | Average of 3 model probability outputs |

### Common Standards

| | |
|---|---|
| **Image size** | 224x224 |
| **Batch size** | 16 |
| **Epochs** | 100 |
| **Seed** | 42 |
| **Learning Rate** | 0.0005 |
| **Optimizer** | AdamW |
| **Augmentation** | HorizontalFlip, Rotation(15°), ColorJitter, RandomResizedCrop |

### Results

| Model | Test Accuracy | Precision | Recall | F1 Score |
|-------|--------------|-----------|--------|----------|
| DenseNet121 | %75.70 | %69.91 | %74.57 | %71.10 |
| ResNet50 | %70.13 | %70.97 | %70.13 | %69.59 |
| EfficientNet-B3 | %XX | %XX | %XX | %XX |
| **Ensemble** | **%XX** | **%XX** | **%XX** | **%XX** |

### Project Structure

```
skin-disease-diagnosis/
├── MehmetOytunÖzer_23040301043_DenseNet121.ipynb
├── FurkanIşık_23040301063_ResNet50.ipynb
├── AliÇelik_23040301059_EfficientNetB3.ipynb
└── README.md
```

---

## Türkçe

Yapay Sinir Ağları dersi dönem projesi - 3 kişilik takım.

### Takım Üyeleri

| İsim | Öğrenci No | Model |
|------|-----------|-------|
| Mehmet Oytun ÖZER | 23040301043 | DenseNet121 |
| Furkan Işık | 23040301063 | ResNet50 |
| Ali Çelik | 23040301059 | EfficientNet-B3 |

### Proje Açıklaması

CNN Ensemble tabanlı cilt hastalığı teşhis sistemi. Her takım üyesi, DermNet veri setinden seçilen 6 hastalık sınıfı üzerinde farklı bir CNN modeli eğitmiştir. Nihai tahmin, tüm modellerin Soft Voting ile birleştirilmesiyle yapılmaktadır.

### Veri Seti

| | |
|---|---|
| **İsim** | DermNet (6 sınıf alt kümesi) |
| **Toplam görsel** | ~6,500 |
| **Sınıf sayısı** | 6 cilt hastalığı |
| **Bölünme** | Eğitim %85 \| Doğrulama %15 \| Test (ayrı klasör) |

**Seçilen Sınıflar:**
1. Acne and Rosacea Photos (Akne ve Roza)
2. Eczema Photos (Egzama)
3. Psoriasis pictures Lichen Planus and related diseases (Sedef/Liken)
4. Urticaria Hives (Kurdeşen)
5. Nail Fungus and other Nail Disease (Tırnak Mantarı)
6. Scabies Lyme Disease and other Infestations and Bites (Uyuz/Isırıklar)

### Modeller

| Model | Geliştirici | Framework |
|-------|-------------|-----------|
| DenseNet121 | Mehmet Oytun ÖZER | PyTorch (Windows) |
| ResNet50 | Furkan Işık | PyTorch (Windows) |
| EfficientNet-B3 | Ali Çelik | PyTorch (Windows) |

### Ensemble Yöntemi

| | |
|---|---|
| **Yöntem** | Soft Voting |
| **Nihai tahmin** | 3 modelin olasılık çıktılarının ortalaması |

### Ortak Standartlar

| | |
|---|---|
| **Görüntü boyutu** | 224x224 |
| **Batch size** | 16 |
| **Epoch** | 100 |
| **Seed** | 42 |
| **Learning Rate** | 0.0005 |
| **Optimizer** | AdamW |
| **Augmentation** | Yatay Çevirme, Döndürme(15°), Renk Değişimi, Rastgele Kırpma |

### Sonuçlar

| Model | Test Doğruluğu | Precision | Recall | F1 Score |
|-------|---------------|-----------|--------|----------|
| DenseNet121 | %75.70 | %69.91 | %74.57 | %71.10 |
| ResNet50 | %70.13 | %70.97 | %70.13 | %69.59 |
| EfficientNet-B3 | %XX | %XX | %XX | %XX |
| **Ensemble** | **%XX** | **%XX** | **%XX** | **%XX** |

### Proje Yapısı

```
skin-disease-diagnosis/
├── MehmetOytunÖzer_23040301043_DenseNet121.ipynb
├── FurkanIşık_23040301063_ResNet50.ipynb
├── AliÇelik_23040301059_EfficientNetB3.ipynb
└── README.md
```
