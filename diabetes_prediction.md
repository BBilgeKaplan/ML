# Diabetes Prediction Machine Learning Project

Bu projede Pima Indians Diabetes veri seti kullanılarak bireylerin diyabet hastalığına sahip olup olmadığını tahmin eden bir makine öğrenmesi sistemi geliştirilmiştir.

## Amaç

Erken diyabet riskini tespit edebilecek bir karar destek modeli oluşturmak ve farklı makine öğrenmesi algoritmalarının performanslarını karşılaştırmak.

## Veri Ön İşleme

- Eksik değerler (özellikle insulin ve glucose) ortalama ile dolduruldu  
- Anlamsız 0 değerleri temizlendi  
- Yeni özellikler türetildi  
- Veriler eğitim ve test olarak ayrıldı  

## Kullanılan Modeller

- Logistic Regression  
- Decision Tree (regularization uygulanmış)  
- Random Forest (ensemble learning)  

## Model Değerlendirme

Modeller sadece accuracy ile değil aşağıdaki metriklerle değerlendirildi:

- Recall  
- Precision  
- F1-score  
- ROC-AUC  

**5 katlı cross validation sonucu:**
- Ortalama doğruluk: %75.2  

## Bulgular

En önemli değişkenler:

- Glucose seviyesi  
- BMI (Vücut kitle indeksi)  
- Yaş  

Modelin diyabetli bireyleri yakalama oranı %69’a kadar çıkarılmıştır  
(threshold tuning ile %87’ye ulaşılmıştır).

## Sonuç

Küçük ve gürültülü bir sağlık veri setinde, uygun ön işleme ve model karşılaştırması ile stabil ve genellenebilir bir makine öğrenmesi modeli geliştirilmiştir.
