# EmpathyNet – Project Story (Devpost Submission)

## The Problem
In an era where global events, crises, and social movements can spark instant emotional waves across societies, understanding collective emotions and their evolution isn't just a "nice-to-have"—it’s a necessity. Yet, policymakers, researchers, media, and the public have no real-time, reliable tool to search, analyze, and visualize how sentiments and empathy shift worldwide (or just in their region) about any issue, person, or event.

## The Solution
**EmpathyNet** is an AI-powered empathy & context search engine. It combines advanced AI agent society with real-time data crawling and global multi-language reasoning. With a single search (e.g., “prabowo merendahkan rupiah”), EmpathyNet fetches, analyzes, and clusters narratives and collective emotional reactions from news, social media, forums—anywhere. The result: an instant, interactive map of public empathy, emotional timelines, and explainable insights, for any country or community.

## How It Works
- **User Input:** Type any issue/person/event in the search box, select a filter (region, timeframe, platform, etc.).
- **AI Agent Pipeline:** 
   1. Data Crawler Agent fetches and sanitizes content globally (multilingual, cross-platform)
   2. Contextualizer Agent clusters/topicalizes trending narratives (LLM-powered)
   3. Empathy Mapping Agent detects and quantifies nuanced emotions (not just positive/negative)
   4. Memory Agent compares current patterns to historical archives
   5. Answer Agent delivers interactive explanations ("why is this area angry?"/"how is this similar to past events?")
- **User Experience:** Output includes heatmap and timeline of emotion clusters, headline narratives, and context-aware Q&A

## What Makes It Unique
- Not just sentiment analysis: EmpathyNet dives into emotional and cultural nuance, across languages and demographics.
- Global with local sensitivity: Filter or compare by country, city, or community. Understand how issues resonate differently in Jakarta vs. New York.
- End-to-end transparency: Users can interactively ask why/when/how public emotions shifted, and see memory-driven pattern analysis.

## Real-World Impact
- **Government/NGOs**: Early warning for disinformation/social unrest; understand ideological shifts or policy impact in real time
- **Media**: Validate or debunk viral narratives; identify hidden “empathy gaps” between demographics
- **Education/Research**: Study collective psychology, monitor wellbeing, enhance digital citizenship
- **Business/CSR**: Track public perception of brands, campaigns, or social programs at massive scale

## Tech Stack
- **Backend:** Python (FastAPI/Flask, Qwen Cloud or opensource LLMs)
- **Frontend:** Interactive dashboard (Streamlit/React)
- **Data:** Real-time crawling (Scrapling, NewsAPI) + Multilingual AI processing
- **Visualization:** Plotly, Leaflet/d3.js (heatmaps, timelines)
- **Scalability:** Modular multi-agent architecture, Docker/Qwen Cloud for global reach

## Demo Flow (User Journey)
1. User: Types “climate anxiety India” & selects country: India, timeline: 2024
2. EmpathyNet fetches multi-platform content, clusters narratives by topic/topic
3. EmpathyNet visualizes clusters of fear, hope, action — on map and time series
4. User can ask: “Why are youth most anxious?” and get root-cause, historical comparison, and explainable answer

---

*EmpathyNet: See what the world feels.*
