def set_intention(self, desire):
    if not desire.strip():
        return "Please provide a clear intention. Example: 'Abundant career opportunities'"
    return f"Intention set to: {desire}"

def detect_limiting_belief(self, belief):
    reframed = self.reframe_belief(belief)
    return reframed

def reframe_belief(self, belief):
    # Add conversational follow-up
    if not any(re.findall(r"can't|don't|not enough", belief, re.I)):
        return f"Let's craft a custom affirmation for: '{belief}'"
    reframed = re.sub(r"I can't", "I am able to", belief, flags=re.IGNORECASE)
    reframed = re.sub(r"I don'?t deserve", "I am worthy of", reframed, flags=re.IGNORECASE)
    reframed = re.sub(r"(I'm not|I am not) good enough", "I am enough", reframed, flags=re.IGNORECASE)
    reframed = re.sub(r"I'll never (.*)", r"I will \1", reframed, flags=re.IGNORECASE)
    reframed = re.sub(r"It's (too hard|impossible)", "It's within my capabilities", reframed, flags=re.IGNORECASE)
    return f"New empowering belief: '{reframed}'"User: "I have a limiting belief: I'll never get out of debt"/settings/access# Handles image input using CLIP or similar model def analyze_image(image_path):     return f"[MOCK] Analyzing image: {image_path}"python cli.py --text "Write a dream interpretation"
python cli.py --image path/to/image.jpg
python cli.py --audio path/to/audio.wav# Handles audio input using Whisper or similar model def transcribe_audio(audio_path):     return f"[MOCK] Transcribing audio from: {audio_path}"# Handles text input using an LLM def generate_text(prompt):     return f"[MOCK] Response to: '{prompt}'"python cli.py --text "What does a duck dream of?"def set_intention(self, desire):
    if not desire.strip():
        return "Please provide a clear intention. Example: 'Abundant career opportunities'"
    return f"Intention set to: {desire}"

def detect_limiting_belief(self, belief):
    reframed = self.reframe_belief(belief)
    return reframed

def reframe_belief(self, belief):
    # Add conversational follow-up
    if not any(re.findall(r"can't|don't|not enough", belief, re.I)):
        return f"Let's craft a custom affirmation for: '{belief}'"
    reframed = re.sub(r"I can't", "I am able to", belief, flags=re.IGNORECASE)
    reframed = re.sub(r"I don'?t deserve", "I am worthy of", reframed, flags=re.IGNORECASE)
    reframed = re.sub(r"(I'm not|I am not) good enough", "I am enough", reframed, flags=re.IGNORECASE)
    reframed = re.sub(r"I'll never (.*)", r"I will \1", reframed, flags=re.IGNORECASE)
    reframed = re.sub(r"It's (too hard|impossible)", "It's within my capabilities", reframed, flags=re.IGNORECASE)
    return f"New empowering belief: '{reframed}'"User: "I have a limiting belief: I'll never get out of debt"
