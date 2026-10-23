# 🦙 LlamaStudio: Autonomous Document & Historical Media Video Engine

LlamaStudio is an end-to-end, server-side autonomous media creation engine that compiles raw research topics or uploaded historical imagery into highly produced documentary content. Built for the **Meta Global AI Developer Hackathon**, it transitions traditional text prompts into cinematic long-form and vertical short-form videos completely programmatically.

## 🚀 Core Architecture & Features
* **Multimodal Grounding (Llama 3.2 Vision):** Automatically extracts context from primary visual sources like historical photos, document scans, or news clippings to drive narration scripts.
* **Structured Script Synthesis (Llama 3.1):** Enforces strict JSON Schema guardrails to research complex historical events and structure multi-scene documentary chapters.
* **Open Audio Generation (Meta AudioCraft):** Leverages open-weights voice generation to synthesize lifelike narration completely free and natively within the ecosystem.
* **Programmatic Rendering Pipeline:** Calculates synchronized audio-to-video duration tensors, applies real-time linear image histogram color matching, and overlays atmospheric particle filters via a customized parallelized FFmpeg backend.

---

## 🛠️ Technical Stack
* **Frontend Dashboard:** Streamlit (Pure Python Interface)
* **LLM & Vision Layer:** Meta Llama 3.1 (70B/405B) & Llama 3.2 Vision via Groq/Together AI API
* **Audio Synthesis:** Meta AudioCraft / Bark API
* **Media Compositor:** Hard-optimized FFmpeg systems engineering framework
* **Image Processing:** OpenCV (cv2), NumPy, SoundFile

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
AUDIO_API_KEY=your_audio_generation_key
```

---

## 🏎️ Execution Flow
To launch the interactive generation dashboard interface, execute the following target entry point:
```bash
streamlit run app.py
```
