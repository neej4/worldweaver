# EmpathyNet – Project AI Requirements & Technical Explanation

## Visi Singkat
EmpathyNet adalah search engine empati dan konteks global. User mencari topik apapun (misal: “prabowo merendahkan rupiah”), AI agent society otomatis mencari narasi, menganalisis dan mengklaster reaksi emosi kolektif, lalu menampilkan insight, visualisasi emosi, ringkasan reasoning, serta fungsi tanya jawab transparan—untuk semua negara, bisa filter lokal.

---

## 1. Functional Requirements
- **FR-1: Contextual Search** – Input apapun (isu, tokoh, peristiwa) → trigger agent pipeline.
- **FR-2: Multi-source Data Fetching** – Ambil data dari news/portal, X (Twitter), IG, TikTok, forum, dsb. untuk seluruh dunia (multi-negara; bisa filter region/bahasa/platform).
- **FR-3: Advanced Context Clustering** – Klaster narasi/isu secara otomatis (LLM-powered), urutkan headline dan sub-topik terpopuler.
- **FR-4: Empathy & Emotion Mapping** – Deteksi, klasifikasi, dan visualisasi spektrum emosi kolektif (cemas, marah, sedih, harap, dsb.) secara global atau tersegmentasi wilayah/komunitas.
- **FR-5: Cross-session Memory** – AI agent mengingat pola narasi dan emosi dari masa lalu, sehingga bisa memberikan insight perbandingan lintas waktu/kasus.
- **FR-6: Explainable Reasoning** – Agent siap memberi jawaban atas pertanyaan “kenapa”, “bagaimana”, dan perbandingan dengan kasus historis.
- **FR-7: User-facing Dashboard** – UI real-time, input bebas, visualisasi heatmap emosi, timeline, headline, disertai tanya-jawab interaktif.

---

## 2. Non-Functional Requirements
- **NFR-1: Scalable** – Siap melayani ratusan query dalam waktu bersamaan; pipeline agent tidak bottleneck di satu negara saja.
- **NFR-2: Privacy-aware** – Tidak menyimpan data privat user, data scraping disanitasi dan dienkripsi jika sensitif.
- **NFR-3: Modular** – Komponen (crawler, contextualizer, emotion mapper, memory, answer agent) bisa di-upgrade/ganti model.
- **NFR-4: Multilingual Support** – Deteksi dan klasifikasi narasi dalam berbagai bahasa, serta analisis kode-switching (misal IG post campur Indo-Inggris).

---

## 3. Agent Society & Context-aware Logic
- **Pipeline Multi-Agent:**
    - Crawler Agent: data fetch & sanitize.
    - Contextualizer Agent: topik/narasi discovery & clustering (LLM).
    - Empathy Mapper Agent: emosi/agregasi lintas region.
    - Memory Agent: menyimpan & retrieve pattern sejarah.
    - Answer Agent: Q&A + explainable output ("kenapa", "mirip kasus...").
- **Context Awareness:**
    - Agent membaca detail permintaan user (negara, waktu, sub-grup).
    - Setiap hasil analitik disertai metadata (asal region, confidence, range emosi).
- **Adaptive:**
    - Jika user ganti region, pipeline langsung filter/re-run untuk area baru.

---

## 4. Technical Stack
- **Backend:** Python (FastAPI/Flask, langchain-like orchestrator), Qwen Cloud API/LLM API.
- **Frontend:** Streamlit, React, atau dashboard web.
- **Scraping:** Scrapling, X(Twitter)-API, NewsAPI, trend harvester IG/Tiktok (via plugin atau partner API).
- **Visualization:** Plotly/Leaflet/d3.js — untuk heatmap, timeline, klaster narasi.
- **Database:** SQLite atau NoSQL (untuk memory/cache/data crawling interaktif).
- **Deployment:** Qwen Cloud siap production, Docker support for local dev.

---

## 5. Use Case Example (Global Context)
- User (dari Kenya) input “election disinformation 2025”, filter country: Indonesia.
- Pipeline fetch + klaster narasi + peta emosi nasional + bandingkan dengan pola pemilu Afrika.
- Agent siap jawab: "Pola emosi negatif di Indonesia cenderung lebih cepat redam dibanding Kenya, berdasarkan archive 5 tahun."

---

## 6. Security & Ethics
- Tidak pernah menyimpan data privat user.
- Scraping mengikuti ToS API/sumber publik.
- Jelaskan data confidence/limitation di output agent.

---
*Draft by Hermes Agent, 2026-06-02. Brand: EmpathyNet.*
