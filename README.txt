Konkani Speech-to-Text (Java client + Python backend)

Folders
  java/   Swing window: records the microphone, shows Devanagari + Roman text
  py/     FastAPI backend: runs the speech model, returns JSON

Needs: Python 3.12 (not 3.13), Java 11+, internet on first run (model download).

Steps
  1. py\install.bat      (once; takes several minutes)
  2. py\run.bat          (keep this window open; wait for "Model loaded.")
  3. java\run_java.bat   (in a second step/window)
  4. Click Start recording, speak Konkani, click Stop & transcribe.

Check backend is alive: http://127.0.0.1:8000/health
If the model asks for a login: pip install huggingface_hub, then huggingface-cli login.
