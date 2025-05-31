# Deteksi Masker Menggunakan VGG16 (Transfer Learning)

Proyek ini membuat model klasifikasi gambar untuk membedakan wajah yang memakai masker dan tidak memakai masker menggunakan metode **transfer learning** dengan pretrained model **VGG16**.

## Dataset
- Jumlah: 200 gambar (100 masker, 100 tanpa masker)
- Ukuran: 224x224 piksel
- Sumber: Kaggle
- Split data: 80% train, 20% test

## Arsitektur Model
- Base model: VGG16 (ImageNet pretrained)
- Layer convolutional dibekukan
- Classifier baru:
  - Linear Layer (128 units, ReLU)
  - Dropout 0.5
  - Output: 2 kelas (sigmoid/softmax)

## Training
- Optimizer: Adam (lr=0.001)
- Loss: CrossEntropyLoss
- Epochs: 5
- Batch size: 16
- Device: CPU/GPU

## Hasil
- Train Accuracy: 95%
- Val Accuracy: 90%
- Confusion Matrix dan Classification Report sudah disediakan
- Prediksi gambar baru juga didemokan

## Contoh Gambar Prediksi
![image](https://github.com/user-attachments/assets/333693ef-d9c7-4f9e-b7f7-4e4a8a82ea0c)


