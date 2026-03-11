# XOR Neural Network Experiment

Bu proje, **XOR probleminin yapay sinir ağları ile çözülmesini** incelemek amacıyla hazırlanmıştır. XOR problemi doğrusal olarak ayrılabilir olmadığı için tek katmanlı perceptronlar tarafından çözülemez. Bu nedenle çalışmada gizli katman içeren bir **Multilayer Perceptron (MLP)** modeli kullanılmıştır.

Bu çalışma **Derin Öğrenme dersi ödevi** kapsamında hazırlanmıştır.

---

## Problem

XOR veri seti aşağıdaki gibi tanımlanır:

| x1 | x2 | y |
|----|----|---|
| 0  | 0  | 0 |
| 0  | 1  | 1 |
| 1  | 0  | 1 |
| 1  | 1  | 0 |

Bu veri yapısı doğrusal olarak ayrılabilir değildir, bu nedenle doğrusal modeller problemi çözemez.

---

## Kullanılan Model

Model mimarisi:

- Input layer: 2 nöron
- Hidden layer: 2–8 nöron
- Output layer: 1 nöron (sigmoid)

Model eğitimi sırasında:

- **Loss function:** Binary Crossentropy  
- **Optimizer:** Adam  

kullanılmıştır.

---

## Yapılan Deneyler

Notebook içinde şu deneyler gerçekleştirilmiştir:

- XOR veri setinin görselleştirilmesi
- Tek katmanlı model denemesi
- Çok katmanlı sinir ağı kurulması
- Eğitim sürecinin analiz edilmesi
- Hidden layer çıktılarının incelenmesi
- Decision boundary görselleştirmesi
- Grid search ile hiperparametre denemeleri

Grid search kapsamında farklı:

- hidden neuron sayısı
- aktivasyon fonksiyonu
- optimizer
- epoch

kombinasyonları test edilmiştir.

---

## Sonuç

Deneyler sonucunda tek katmanlı perceptronun XOR problemini çözemediği, ancak gizli katman içeren MLP modelinin doğrusal olmayan karar sınırları öğrenerek problemi başarıyla sınıflandırabildiği gösterilmiştir.

---


