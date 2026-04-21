# Submission Akhir BMLP - Nur Rahmawati

Repositori ini berisi pekerjaan akhir untuk dua tugas utama:
- Clustering
- Klasifikasi

## Struktur Proyek

- `[Clustering]_Submission_Akhir_BMLP_Nur_Rahmawati.ipynb` - notebook utama untuk clustering.
- `[Klasifikasi]_Submission_Akhir_BMLP_Nur_Rahmawati.ipynb` - notebook utama untuk klasifikasi.
- `data_clustering.csv` - dataset clustering.
- `data_clustering_inverse.csv` - dataset inverse/preprocessed clustering.
- `model_clustering.h5` - model K-Means clustering.
- `PCA_model_clustering.h5` - model clustering berbasis PCA.
- `decision_tree_model.h5` - model decision tree.
- `explore_RandomForest_classification.h5` - model Random Forest.
- `explore_LogisticRegression_classification.h5` - model Logistic Regression.
- `explore_KNN_classification.h5` - model KNN.
- `explore_SVM_classification.h5` - model SVM.
- `tuning_classification.h5` - model hasil tuning.

## Hasil Model

### 1) Clustering

**Algoritma:** K-Means (`n_clusters=3`)

| Metrik | Nilai |
|---|---:|
| Silhouette Score | 0.5120 |

### 2) Klasifikasi

#### Decision Tree (Basic)

| Metrik | Nilai |
|---|---:|
| Train Accuracy | 1.0000 |
| Test Accuracy | 1.0000 |
| Cross-validation Accuracy | 1.0000 |

#### Random Forest (Exploration)

**Best Parameters:**
- `n_estimators=150`
- `max_depth=9`
- `max_features='sqrt'`
- `min_samples_split=100`
- `min_samples_leaf=25`

| Metrik | Nilai |
|---|---:|
| CV Score | 0.8156 |
| Train Accuracy | 0.9299 |
| Test Accuracy | 0.9105 |
| Precision (weighted) | 0.9286 |
| Recall (weighted) | 0.9105 |
| F1-Score (weighted) | 0.9120 |

#### Logistic Regression (Exploration)

| Metrik | Nilai |
|---|---:|
| Train Accuracy | 1.0000 |
| Test Accuracy | 1.0000 |
| Precision (weighted) | 1.0000 |
| Recall (weighted) | 1.0000 |
| F1-Score (weighted) | 1.0000 |

#### KNN (Exploration, k=5)

| Metrik | Nilai |
|---|---:|
| Train Accuracy | 0.9925 |
| Test Accuracy | 0.9781 |
| Precision (weighted) | 0.9783 |
| Recall (weighted) | 0.9781 |
| F1-Score (weighted) | 0.9782 |

#### SVM (Exploration, RBF)

| Metrik | Nilai |
|---|---:|
| Train Accuracy | 1.0000 |
| Test Accuracy | 0.9920 |
| Precision (weighted) | 0.9922 |
| Recall (weighted) | 0.9920 |
| F1-Score (weighted) | 0.9920 |

#### Decision Tree (Tuning)

| Metrik | Nilai |
|---|---:|
| Train Accuracy | 0.9761 |
| Test Accuracy | 0.9702 |
| Cross-validation Accuracy | 0.9886 |

## Catatan

- Nilai metrik di atas diambil dari output notebook yang tersimpan.
- Reproduksi hasil dapat dilakukan dengan menjalankan kedua notebook utama secara berurutan.