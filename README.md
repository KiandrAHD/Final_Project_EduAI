# 🎓 EduAI - Education Chatbot

[![Python Version](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.28%2B-FF4B4B.svg)](https://streamlit.io/)
[![Google Gemini](https://img.shields.io/badge/AI-Google%20Gemini%202.5%20Flash-8E44AD.svg)](https://ai.google.dev/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> **EduAI** adalah chatbot pendidikan berbasis AI yang dirancang sebagai teman belajar pintar bagi pelajar di Indonesia. Aplikasi ini dibuat menggunakan **Streamlit**, terintegrasi dengan **Google Gemini API (`gemini-2.5-flash`)**, dan dikembangkan melalui lingkungan **Google Colab** yang dihubungkan ke publik menggunakan **Ngrok**.

---

## 📌 Daftar Isi
- [Fitur Utama](#-fitur-utama)
- [Tech Stack](#-tech-stack)
- [Struktur File](#-struktur-file)
- [Panduan Cara Menjalankan](#-panduan-cara-menjalankan)
  - [Metode 1: Menjalankan di Google Colab (Rekomendasi)](#metode-1-menjalankan-di-google-colab)
  - [Metode 2: Menjalankan di Komputer Lokal](#metode-2-menjalankan-di-komputer-lokal)
- [Cara Kerja System Memory](#-cara-kerja-system-memory)
- [Lisensi](#-lisensi)

---

## ✨ Fitur Utama

- 💬 **Interaktif & Respon Cepat**: Membantu menjelaskan materi sekolah (Matematika, Fisika, Biologi, Informatika, dll.) langkah demi langkah dengan bahasa yang ramah dan mudah dipahami.
- 🧠 **Dynamic Session Memory**: Sistem membaca dan mengingat profil pengguna (Nama, Jenjang Sekolah, dan Mata Pelajaran Favorit) dari percakapan secara otomatis.
- 🎨 **Modern Dark Theme**: Tampilan antarmuka yang bersih dan responsif menggunakan Custom CSS pada Streamlit.
- 🔑 **Pengaturan API Key Mandiri**: Pengguna dapat memasukkan Google Gemini API Key milik mereka sendiri melalui sidebar aplikasi.
- 🧹 **Reset Session & Memory**: Kemampuan untuk mengosongkan riwayat obrolan dan menghapus memori profil kapan saja.

---

## 🛠️ Tech Stack

- **Framework Interface**: Streamlit
- **AI Model & SDK**: Google Gemini API (`google-genai` SDK, Model: `gemini-2.5-flash`)
- **Tunneling Tool**: `pyngrok` (Mengakses server Streamlit Colab dari URL publik)
- **Asynchronous Execution**: `nest_asyncio`

---

## 📁 Struktur File

```text
Final_Project_EduAI/
│
├── Final_Project_EduAI.ipynb   # Notebook Google Colab utama (setup ngrok & run streamlit)
├── streamlit_chat_app.py       # Source code aplikasi Streamlit & logika chatbot
└── README.md                   # Dokumentasi proyek
