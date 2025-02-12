# 📄 Image to Text Evaluation
🚀 Evaluate different OCR (Optical Character Recognition) frameworks to extract textual data from images. Upload an image and provide the ground truth to comapre the results.

##  ⚖️ Frameworks Compared
📌 **Pytesseract** - A Python wrapper for Google’s Tesseract OCR engine. Provides fast text extraction.  
📌 **PaddleOCR** - Provides fast and multi-language text extraction.  
📌 **EasyOCR** - A deep-learning-based OCR framework that supports multiple languages but not speed efficient.  
📌 **DocTR** - A TensorFlow/PyTorch-based OCR framework but requires large image size for extraction.  
📌 **PyOCR** - A lightweight wrapper for multiple OCR engines, including Tesseract and Cuneiform, offering basic text extraction capabilities.  

## 📊 Key Metrics  
✅ **WER (Word Error Rate)** - Measures the ratio of incorrect words to the total words in the ground truth.  
✅ **CER (Character Error Rate)** - Calculates the ratio of incorrect characters to the total characters in the ground truth.    
✅ **Precision** - Determines how many of the detected words were correct compared to the total words recognized.  
✅ **Recall** - Measures how many actual words from the image were correctly recognized.  
✅ **Latency** - Evaluates the time taken (in seconds) by the framework to process and extract text from an image.  

## ⚙️ Comparison
| Metric             | Pytesseract | PaddleOCR | EasyOCR | DocTR | PyOCR |
|--------------------|------------|-----------|---------|------|-------|
| **WER**           | 0.167      | 0.000     | 0.333   | 1.000 | 0.167 |
| **CER**           | 0.036      | 0.000     | 0.357   | 1.000 | 0.036 |
| **Precision**     | 0.923      | 1.000     | 1.000   | 0.000 | 0.923 |
| **Recall**        | 1.000      | 1.000     | 1.000   | 0.000 | 1.000 |
| **Latency (sec)** | 0.288      | 0.207     | 1.448   | 0.062 | 0.291 |

## 🎯 Summary


## 🚀 How to Use

## 🔗 References
