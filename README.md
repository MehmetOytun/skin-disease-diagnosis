# Skin Disease Diagnosis System

---

## English

Artificial Neural Networks course project - 3 person team.

### Team Members
| Name | Student ID | Model |
|------|-----------|-------|
| Mehmet Oytun Özer | 23040301043 | MobileNetV2 |
| Furkan Işık | 23040301063 | ResNet50 |
| Ali Çelik | 23040301059 | EfficientNet-B0 |

### Project Description
CNN Ensemble based skin disease diagnosis system. 
Each team member trained a different CNN model. 
Final prediction is made by combining all models with Soft Voting.

### Dataset
- **Name:** DermNet
- **Images:** 19,500
- **Classes:** 23 skin diseases
- **Split:** Train %68 | Validation %12 | Test %20

### Models
| Model | Developer | Framework |
|-------|-----------|-----------|
| MobileNetV2 | Mehmet Oytun Özer | PyTorch (Windows) |
| ResNet50 | Furkan Işık | PyTorch (Windows) |
| EfficientNet-B0 | Ali Çelik | PyTorch (Windows) |

### Ensemble Method
- Method: Soft Voting
- Final prediction: Average of 3 model probability outputs

### Common Standards
- Image size: 224x224
- Batch size: 32
- Epochs: 15
- Seed: 42
- Optimizer: Adam (lr: 0.001)
- Augmentation: HorizontalFlip, Rotation(10°), Brightness, Contrast

### Results
| Model | Test Accuracy | Precision | Recall | F1 Score |
|-------|--------------|-----------|--------|----------|
| MobileNetV2 | %39.98 | %36.53 | %40.39 | %36.77 |
| ResNet50 | %41.25 | %39.52 | %43.01 | %38.56 |
| EfficientNet-B0 | %55.80 | %56.45 | %55.80 | %55.04 |
| **Ensemble** | **%XX** | **%XX** | **%XX** | **%XX** |

### Project Structure
```
skin-disease-diagnosis/
├── MehmetOytunÖzer_23040301043_SkinDiseaseDiagnosis/
│   ├── MobileNetV2.ipynb              # Training code and model architecture
│   ├── best_mobilenet_model.pth       # Trained model weights (best checkpoint)
│   ├── probabilities_mobilenet.npy    # Softmax output probabilities for ensemble
│   ├── test_labels.npy                # Ground truth labels for test set
│   └── confusion_matrix_mobilenet.jpg # Per-class prediction visualization
├── FurkanIşık_23040301063_SkinDiseaseDiagnosis/
│   ├── Resnet50Code.ipynb             # Training code and model architecture
│   ├── best_resnet50_model.pth        # Trained model weights
│   ├── probabilities_resnet50.npy     # Softmax output probabilities for ensemble
│   ├── test_labels.npy                # Ground truth labels for test set
│   └── confusion_matrix_resnet50.jpg  # Per-class prediction visualization
└── AliÇelik_23040301059_SkinDiseaseDiagnosis/
    ├── sefoya.ipynb                   # Training code and model architecture
    ├── sefoya_final_gpu_model.pth     # Trained model weights
    ├── probabilities_sefoya.npy       # Softmax output probabilities for ensemble
    ├── test_labels_sefoya.npy         # Ground truth labels for test set
    └── confusion_matrix_sefoya.png    # Per-class prediction visualization
```

---

## Türkçe

Yapay Sinir Ağları dersi dönem projesi - 3 kişilik takım.

### Takım Üyeleri
| İsim | Öğrenci No | Model |
|------|-----------|-------|
| Mehmet Oytun Özer | 23040301043 | MobileNetV2 |
| Furkan Işık | 23040301063 | ResNet50 |
| Ali Çelik | 23040301059 | EfficientNet-B0 |

### Proje Açıklaması
CNN Ensemble tabanlı cilt hastalığı teşhis sistemi.
Her takım üyesi farklı bir CNN modeli eğitmiştir.
Nihai tahmin, tüm modellerin Soft Voting ile birleştirilmesiyle yapılmaktadır.

### Veri Seti
- **İsim:** DermNet
- **Görsel Sayısı:** 19,500
- **Sınıf Sayısı:** 23 cilt hastalığı
- **Bölünme:** Eğitim %68 | Doğrulama %12 | Test %20

### Modeller
| Model | Geliştirici | Framework |
|-------|-----------|-----------|
| MobileNetV2 | Mehmet Oytun Özer | PyTorch (Windows) |
| ResNet50 | Furkan Işık | PyTorch (Windows) |
| EfficientNet-B0 | Ali Çelik | PyTorch (Windows) |

### Ensemble Yöntemi
- Yöntem: Soft Voting
- Nihai tahmin: 3 modelin olasılık çıktılarının ortalaması

### Ortak Standartlar
- Görüntü boyutu: 224x224
- Batch size: 32
- Epoch: 15
- Seed: 42
- Optimizer: Adam (lr: 0.001)
- Augmentation: Yatay Çevirme, Döndürme(10°), Parlaklık, Kontrast

### Sonuçlar
| Model | Test Doğruluğu | Precision | Recall | F1 Score |
|-------|--------------|-----------|--------|----------|
| MobileNetV2 | %39.98 | %36.53 | %40.39 | %36.77 |
| ResNet50 | %41.25 | %39.52 | %43.01 | %38.56 |
| EfficientNet-B0 | %55.80 | %56.45 | %55.80 | %55.04 |
| **Ensemble** | **%XX** | **%XX** | **%XX** | **%XX** |

### Proje Yapısı
```
skin-disease-diagnosis/
├── MehmetOytunÖzer_23040301043_SkinDiseaseDiagnosis/
│   ├── MobileNetV2.ipynb              # Eğitim kodu ve model mimarisi
│   ├── best_mobilenet_model.pth       # Eğitilmiş model ağırlıkları (en iyi checkpoint)
│   ├── probabilities_mobilenet.npy    # Ensemble için softmax olasılık çıktıları
│   ├── test_labels.npy                # Test seti gerçek etiketleri
│   └── confusion_matrix_mobilenet.jpg # Sınıf bazlı tahmin görselleştirmesi
├── FurkanIşık_23040301063_SkinDiseaseDiagnosis/
│   ├── Resnet50Code.ipynb             # Eğitim kodu ve model mimarisi
│   ├── best_resnet50_model.pth        # Eğitilmiş model ağırlıkları
│   ├── probabilities_resnet50.npy     # Ensemble için softmax olasılık çıktıları
│   ├── test_labels.npy                # Test seti gerçek etiketleri
│   └── confusion_matrix_resnet50.jpg  # Sınıf bazlı tahmin görselleştirmesi
└── AliÇelik_23040301059_SkinDiseaseDiagnosis/
    ├── sefoya.ipynb                   # Eğitim kodu ve model mimarisi
    ├── sefoya_final_gpu_model.pth     # Eğitilmiş model ağırlıkları
    ├── probabilities_sefoya.npy       # Ensemble için softmax olasılık çıktıları
    ├── test_labels_sefoya.npy         # Test seti gerçek etiketleri
    └── confusion_matrix_sefoya.png    # Sınıf bazlı tahmin görselleştirmesi
```
