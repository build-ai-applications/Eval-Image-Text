# 📄 Image to Text Evaluation

🚀 This repository provides a comprehensive evaluation of different OCR (Optical Character Recognition) frameworks to extract textual data from images. Users can upload an image, provide the ground truth text, and compare the results across multiple OCR frameworks.

## ⚖️ OCR Frameworks Compared

📌 **Pytesseract** - A Python wrapper for Google’s Tesseract OCR engine, providing fast text extraction.  
📌 **PaddleOCR** - Offers fast, multi-language text extraction with high accuracy.  
📌 **EasyOCR** - A deep-learning-based OCR framework supporting multiple languages, but less efficient in speed.  
📌 **DocTR** - A TensorFlow/PyTorch-based OCR framework that requires high-resolution images for optimal extraction.  
📌 **PyOCR** - A lightweight wrapper supporting multiple OCR engines, including Tesseract and Cuneiform, for basic text extraction.  

## 📊 Key Evaluation Metrics

✅ **WER (Word Error Rate)** - Measures the ratio of incorrect words to the total words in the ground truth.  
✅ **CER (Character Error Rate)** - Calculates the ratio of incorrect characters to the total characters in the ground truth.  
✅ **Precision** - Determines how many of the detected words were correct compared to the total recognized words.  
✅ **Recall** - Measures how many actual words from the image were correctly recognized.  
✅ **Latency** - Evaluates the time taken (in seconds) by each framework to process and extract text from an image.  

## ⚙️ Performance Comparison

| Metric             | Pytesseract | PaddleOCR | EasyOCR | DocTR | PyOCR |
|--------------------|------------|-----------|---------|-------|-------|
| **WER**           | 0.167      | 0.000     | 0.333   | 1.000 | 0.167 |
| **CER**           | 0.036      | 0.000     | 0.357   | 1.000 | 0.036 |
| **Precision**     | 0.923      | 1.000     | 1.000   | 0.000 | 0.923 |
| **Recall**        | 1.000      | 1.000     | 1.000   | 0.000 | 1.000 |
| **Latency (sec)** | 0.288      | 0.207     | 1.448   | 0.062 | 0.291 |

## 🎯 Summary of Findings

- **PaddleOCR** is the best choice for fast and accurate text extraction.  
- **PaddleOCR, Pytesseract, and PyOCR** provide fast extraction.  
- **EasyOCR** delivers good accuracy but is the slowest among the evaluated frameworks.  
- **DocTR** performs best with high-resolution images but may not be suitable for smaller inputs.  

## 🚀 How to Use

1️⃣ Clone the repository:
```sh
 git clone <repo-url>
```

2️⃣ Navigate to the project directory:
```sh
 cd image-to-text-evaluation
```

3️⃣ Open and run the Jupyter notebook:
```sh
 jupyter notebook Evaluation_Image_to_Text.ipynb
```

4️⃣ Upload an image and run the script to evaluate OCR performance.

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request if you'd like to improve the evaluation methods or add new OCR frameworks.

## 📜 License

This project is licensed under the [Apache 2.0](LICENSE), allowing free and open usage, modification, and distribution.

## 🔗 References

- [Pytesseract](https://github.com/madmaze/pytesseract)  
- [PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR)  
- [EasyOCR](https://github.com/JaidedAI/EasyOCR)  
- [DocTR](https://github.com/mindee/doctr)  
- [PyOCR](https://gitlab.gnome.org/World/OpenPaperwork/pyocr)  

