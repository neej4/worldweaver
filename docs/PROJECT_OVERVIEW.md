# EMPATHY ENGINE: Collective Context & Emotional Mapping Platform

## Visi Singkat
Platform pencarian empati kolektif: User mengetik topik apapun (misal: "prabowo merendahkan rupiah"), agent otomatis mencari, mengklaster narasi dan reaksi emosi publik, lalu memberikan analisis narasi, peta emosi, tren, dan reasoning berbasis memori sejarah digital bangsa.

---

## 1. Fitur Utama
- **Context Search Engine:** Input topik → multi-agent pipeline berjalan seperti search engine, hasilkan klaster narasi & visual emosi.
- **Empathy Mapping:** Deteksi dan visualisasi spektrum emosi (cemas, marah, bangga, dsb) lintas daerah/komunitas.
- **Long-term Memory:** Agent mengakses dan membandingkan pola sejarah narasi/emosi pada kasus serupa di masa lalu.
- **Explainable Reasoning:** Jawaban agent jernih, siap ditanya ulang ("kenapa pola ini muncul?").
- **UI Interaktif:** Input bebas topik, klik "Cari Empathy", hasil analitik multimodal (heatmap, timeline, headline).

---

## 2. Struktur Direktori
```text
EMPATHY_ENGINE/
├── docs/                   # Dokumen (spec, riset)
├── core/                   # Pipeline inti multi-agent
│   ├── crawler.py          # Data fetching (news, X, IG, dll.)
│   ├── context_ranker.py   # Klaster/topik discovery
│   ├── emotion_mapper.py   # Deteksi & mapping emosi publik
│   ├── memory_agent.py     # Memori jangka panjang (pattern historis)
│   └── answer_agent.py     # Responsible Q&A/penjelasan lanjutan
├── ui/                     # Frontend/UX (streamlit/web/cli)
│   └── search_ui.py
├── data/                   # Kumpulan data hasil crawl/analisa
├── assets/                 # Visualisasi, diagram, resources
└── .env                    # Kunci API, credential
```

---

## 3. Pipeline Kerja Multi-Agent
1. **User Input:** Kata kunci/topik via UI ("Cari Empathy")
2. **Crawler Agent:** Fetch data multi-platform (real/dummy berjenis teks, visual)
3. **Contextualizer:** Klaster & filter narasi paling relevan
4. **Empathy Mapper:** Klasifikasi & mapping emosi kolektif + distribusi demografi
5. **Memory Agent:** Bandingkan pola narasi/emosi dengan masa lalu
6. **Answering Agent:** Jawab interaktif ("kenapa", "bagaimana", dsb)
7. **Visualisasi:** Timeline, heatmap, klaster headline narasi

---

## 4. Contoh Use Case (User Journey)
- User tulis: "prabowo merendahkan rupiah", klik Cari Empathy
- SYSTEM:
    1. Crawl 5000+ post/news 2 minggu terakhir
    2. Klaster narasi/isu: sentralisasi headline
    3. Empathy mapping: "50% marah, 30% apatis, 20% mendukung (lokasi/demografi..."
    4. Memory: "Mirip sentimen demo 2019."
    5. Agent siap Q&A: "Kenapa marah di Jawa lebih tinggi dari Sumatra?"

---

## 5. Target Stack
- **Python (FastAPI/Streamlit/CLI)**: Orkestrasi & UI
- **Qwen Cloud/LLM API**: Reasoning, emosi, memori
- **Scrapling/X-API/NewsAPI**: Crawler
- **Plotly/Leaflet**: Peta & grafik visual interaktif

---

*File created by Hermes Agent, 2026-06-02*
