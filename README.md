# Judol LLM - Deteksi Komentar Judi Online dengan Deep Learning & Transformers

Judol LLM adalah proyek riset yang bertujuan untuk mendeteksi komentar yang mengandung unsur judi online pada media sosial menggunakan berbagai pendekatan machine learning dan deep learning, termasuk LSTM, CNN, Random Forest, dan model language model modern seperti GPT, BERT, RoBERTa, dan DeBERTa.

## Fitur Utama
- **Preprocessing Data Komentar**: Membersihkan dan menyiapkan data komentar untuk pelatihan model.
- **Training Model Klasifikasi**: Mendukung berbagai arsitektur (LSTM, CNN, RF, GPT, BERT, RoBERTa, DeBERTa, Gemma).
- **Evaluasi & Visualisasi**: Menyediakan metrik akurasi, loss, dan visualisasi hasil training per epoch.
- **Prediksi Komentar Baru**: Model siap digunakan untuk mendeteksi komentar baru secara otomatis.
- **Confusion Matrix**: Analisis performa model pada data training dan testing.

## Struktur Folder
- `judol_training_final_lstm_rf_cnn.ipynb` : Notebook training model klasik & deep learning.
- `judol_training_gpt.ipynb` : Notebook training GPT dan model transformer lain.
- `dataset.csv` : Dataset utama komentar.
- `save_model2/`, `save_model3/` : Folder penyimpanan model hasil training (tidak di-track git).

## Cara Penggunaan
1. **Instalasi Dependensi**
   ```bash
   pip install -r requirements.txt
   ```
2. **Jalankan Notebook**
   - Buka notebook yang diinginkan di VS Code/Jupyter.
   - Ikuti urutan cell dari preprocessing, training, hingga evaluasi.
3. **Prediksi Komentar Baru**
   - Gunakan fungsi `predict_comment()` pada notebook untuk mendeteksi komentar baru.

## Contoh Prediksi
```python
comment = "Main di BIBIT288 seru abis! Bonusnya mantap!"
result = predict_comment(comment)
if result == 1:
    print("komentar ini adalah judi online.")
else:
    print("komentar ini bukan judi online.")
```

## Kontribusi
Proyek ini terbuka untuk pengembangan lebih lanjut. Silakan fork dan pull request untuk perbaikan atau penambahan fitur.

## Lisensi
MIT License

---
**Judol LLM** - Riset deteksi komentar judi online berbasis AI & NLP Indonesia
