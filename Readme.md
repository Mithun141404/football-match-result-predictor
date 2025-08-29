<div align="center">

# 🎤 Tamil Speech to Sign Language Converter ✋

### *Bridging Communication Through AI-Powered Tamil Speech Recognition*

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.7%2B-blue?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/AI-Wav2Vec2-green?style=for-the-badge&logo=artificial-intelligence&logoColor=white" alt="AI">
  <img src="https://img.shields.io/badge/Tamil-Language-orange?style=for-the-badge&logo=google-translate&logoColor=white" alt="Tamil">
  <img src="https://img.shields.io/badge/Sign_Language-Accessible-purple?style=for-the-badge&logo=accessibility&logoColor=white" alt="Accessible">
</p>

<p align="center">
  <strong>Transform spoken Tamil words into beautiful sign language representations in real-time</strong>
</p>

![Demo](https://via.placeholder.com/800x400/1a1a2e/eee?text=Tamil+Speech+to+Sign+Demo)

</div>

---

## 🌟 **Features**

<table>
<tr>
<td width="50%">

### 🎯 **Core Capabilities**
- 🗣️ **Real-time Speech Recognition**
- 🔤 **Comprehensive Tamil Character Support**
- 🔢 **Smart Number Conversion**
- 🖼️ **Visual Sign Language Display**
- ⚡ **Lightning Fast Processing**

</td>
<td width="50%">

### 🎨 **User Experience**
- 🌙 **Modern Dark Theme Interface**
- 📱 **Responsive Layout**
- 🎧 **Built-in Audio Recording**
- 🧹 **One-click Clear Function**
- 🔄 **Seamless Mode Switching**

</td>
</tr>
</table>

---

## 🚀 **Quick Start**

### **Prerequisites**
```bash
Python 3.7+ | Microphone Access | Internet Connection (first run)
```

### **Installation**
```bash
# 1️⃣ Clone the repository
git clone <repository-url>
cd tamil-speech-to-sign

# 2️⃣ Install dependencies
pip install -r requirements.txt

# 3️⃣ Set up sign images directory
mkdir tamil_alphabets
# Add your Tamil sign language images here

# 4️⃣ Run the application
python tamil_speech_to_sign.py
```

### **Requirements File**
```txt name=requirements.txt
tkinter
pillow>=9.0.0
sounddevice>=0.4.0
scipy>=1.7.0
torch>=1.11.0
transformers>=4.20.0
torchaudio>=0.11.0
numpy>=1.21.0
```

---

## 🎮 **How to Use**

<div align="center">

### **Three Simple Steps**

```mermaid
graph LR
    A[🎤 Click Record] --> B[🗣️ Speak Tamil] --> C[✨ View Signs]
    
    style A fill:#4CAF50
    style B fill:#2196F3  
    style C fill:#FF9800
```

</div>

| Button | Function | Duration |
|--------|----------|----------|
| **🎤 Words to Sign** | Record Tamil words/sentences | 4 seconds |
| **🔢 Numbers to Sign** | Record Tamil numbers | 4 seconds |
| **🧹 Clear** | Reset display and transcription | Instant |

---

## 📝 **Supported Characters**

<details>
<summary><strong>🔤 Tamil Vowels (உயிர்)</strong></summary>

```
அ  ஆ  இ  ஈ  உ  ஊ  எ  ஏ  ஐ  ஒ  ஓ  ஔ  ஃ
```

</details>

<details>
<summary><strong>🔤 Tamil Consonants (மெய்)</strong></summary>

```
க  ங  ச  ஞ  ட  ண  த  ந  ப  ம  ய  ர  ல  வ  ழ  ள  ற  ன
```

</details>

<details>
<summary><strong>🔢 Numbers & Digits</strong></summary>

**Tamil Digits:** ௦ ௧ ௨ ௩ ௪ ௫ ௬ ௭ ௮ ௯

**English Digits:** 0 1 2 3 4 5 6 7 8 9

**Tamil Words:** ஒன்று, இரண்டு, மூன்று, நான்கு, ஐந்து, ஆறு, ஏழு, எட்டு, ஒன்பது

</details>

---

## ⚙️ **Technical Architecture**

<div align="center">

```mermaid
graph TB
    A[🎤 Audio Input] --> B[🔊 Sound Processing]
    B --> C[🤖 Wav2Vec2 Model]
    C --> D[📝 Tamil Transcription]
    D --> E[🔤 Character Splitting]
    E --> F[🖼️ Sign Image Display]
    
    style A fill:#e1f5fe
    style C fill:#f3e5f5
    style F fill:#e8f5e8
```

</div>

### **🧠 AI Model Specifications**

| Component | Specification |
|-----------|--------------|
| **Model** | `Amrrs/wav2vec2-large-xlsr-53-tamil` |
| **Framework** | Hugging Face Transformers |
| **Language** | Tamil (தமிழ்) |
| **Sample Rate** | 16kHz |
| **Processing** | CPU Optimized |

---

## 🏗️ **Project Structure**

```
📦 tamil-speech-to-sign/
├── 📄 tamil_speech_to_sign.py    # 🚀 Main application
├── 📄 requirements.txt           # 📋 Dependencies
├── 📄 README.md                  # 📖 This file
├── 📁 tamil_alphabets/           # 🖼️ Sign language images
│   ├── 🖼️ அ.jpg
│   ├── 🖼️ ஆ.jpg
│   ├── 🖼️ க.jpg
│   └── 🖼️ ... (other characters)
└── 📄 output.wav                 # 🎵 Temporary audio file
```

---

## 🎨 **Customization**

<details>
<summary><strong>🖼️ Adding New Sign Images</strong></summary>

1. **Prepare Image**: Ensure it's in `.jpg` format
2. **Naming**: Use the Tamil character as filename (`அ.jpg`)
3. **Location**: Place in `tamil_alphabets/` directory
4. **Size**: Recommended 200x200px or higher

</details>

<details>
<summary><strong>⏱️ Adjust Recording Duration</strong></summary>

```python
# In record_and_transcribe() function
duration = 5  # Change from 4 to 5 seconds
```

</details>

<details>
<summary><strong>🎨 Theme Customization</strong></summary>

```python
# Background colors
root.configure(bg="#your_color")

# Canvas styling  
canvas = tk.Canvas(root, bg="#your_canvas_color", ...)

# Text colors
transcription_label = tk.Label(..., fg="#your_text_color", ...)
```

</details>

---

## 🐛 **Troubleshooting**

<details>
<summary><strong>❌ Common Issues & Solutions</strong></summary>

| Issue | Solution |
|-------|----------|
| **🎤 No audio detected** | Check microphone permissions & connection |
| **🖼️ Missing sign images** | Verify `tamil_alphabets/` folder exists with proper naming |
| **🐌 Slow performance** | Ensure stable internet for first-time model download |
| **🔒 Token errors** | Verify Hugging Face token validity |
| **💾 Memory issues** | Close other applications, restart if needed |

</details>

---

## 🤝 **Contributing**

We welcome contributions! Here's how you can help:

<div align="center">

[![Contribute](https://img.shields.io/badge/Contribute-Welcome-brightgreen?style=for-the-badge&logo=github)](https://github.com)

</div>

### **Areas for Enhancement**
- 🎯 Additional Tamil dialects support
- 🖼️ Expand sign image database
- ⚡ Performance optimizations
- 🎨 UI/UX improvements
- 📱 Mobile app version
- 🌐 Web-based interface

---

## 📄 **License & Attribution**

<div align="center">

[![License](https://img.shields.io/badge/License-Open_Source-blue?style=for-the-badge)](LICENSE)

</div>

### **Acknowledgments**
- 🤗 **Hugging Face** - For providing the AI model infrastructure
- 👨‍💻 **Amrrs** - For training the Tamil Wav2Vec2 model
- 🤟 **Tamil Sign Language Community** - For language references
- 💻 **Open Source Contributors** - For making this possible

---

## 🎯 **What's Next?**

<div align="center">

### **Roadmap 2024-2025**

```mermaid
timeline
    title Development Roadmap
    
    Q4 2024 : Mobile App
           : Web Interface
    
    Q1 2025 : Multi-dialect Support
           : Performance Boost
    
    Q2 2025 : Advanced ML Models
           : Community Features
```

</div>

---

<div align="center">

## 💙 **Made with Love for Tamil Community**

<p>
<strong>Empowering communication • Breaking barriers • Connecting hearts</strong>
</p>

<p>
<img src="https://img.shields.io/badge/Made_with-❤️-red?style=for-the-badge" alt="Made with Love">
<img src="https://img.shields.io/badge/For-தமிழ்_Community-orange?style=for-the-badge" alt="Tamil Community">
</p>

---

### 📞 **Support & Contact**

<p>
<a href="mailto:support@example.com"><img src="https://img.shields.io/badge/Email-Support-blue?style=for-the-badge&logo=gmail" alt="Email"></a>
<a href="#"><img src="https://img.shields.io/badge/Discord-Community-purple?style=for-the-badge&logo=discord" alt="Discord"></a>
<a href="#"><img src="https://img.shields.io/badge/Documentation-Wiki-green?style=for-the-badge&logo=gitbook" alt="Docs"></a>
</p>

**Created by:** [Mithunkumar14](https://github.com/Mithunkumar14) • **Last Updated:** August 29, 2025

</div>
