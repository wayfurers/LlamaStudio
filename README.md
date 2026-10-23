# 🦙 LlamaStudio: Autonomous Document & Historical Media Video Engine

LlamaStudio is an end-to-end, server-side autonomous media creation engine that compiles raw research topics or uploaded historical imagery into highly produced documentary content. Built for the **Meta Global AI Developer Hackathon**, it transitions traditional text prompts into cinematic long-form and vertical short-form videos completely programmatically.

## 🚀 Core Architecture & Features
* **Multimodal Grounding (Llama 3.2 Vision):** Automatically extracts context from primary visual sources like historical photos, document scans, or news clippings to drive narration scripts.
* **Structured Script Synthesis (Llama 3.1):** Enforces strict JSON Schema guardrails to research complex historical events and structure multi-scene documentary chapters.
* **Programmatic Rendering Pipeline:** Calculates synchronized audio-to-video duration tensors, applies real-time linear image histogram color matching, and overlays atmospheric particle filters.
* **Dual-Format Delivery:** Encodes high-definition master compositions alongside automated vertical promo crops optimized for TikTok, Shorts, and Reels using a customized parallelized FFmpeg backend.

---

## 🛠️ Technical Stack
* **Frontend Dashboard:** Streamlit (Pure Python Interface)
* **LLM & Vision Layer:** Meta Llama 3.1 (70B/405B) & Llama 3.2 Vision via Groq/Together AI API
* **Media Compositor:** Hard-optimized FFmpeg systems engineering framework
* **Image & Audio Engines:** OpenCV (cv2), NumPy, SoundFile, MeloTTS/Bark API

---

## 📦 System Installation & Requirements

Ensure you have system-level binaries for `ffmpeg` and `ffprobe` installed and exposed to your global system path environment.

```bash
# Clone the repository framework
git clone https://github.com
cd LlamaStudio

# Install explicit Python dependencies
pip install -r requirements.txt
```

### Environment Configuration
Create a `.env` file in the project root directory:
```env
LLAMA_API_KEY=your_meta_llama_api_provider_key
CLOUDFLARE_ACCOUNT_ID=your_cloudflare_id
CLOUDFLARE_API_TOKEN=your_cloudflare_token
```

---

## 🏎️ Execution Flow
To launch the interactive generation dashboard interface, execute the following target entry point:
```bash
streamlit run app.py
```
