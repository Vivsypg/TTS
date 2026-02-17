[frog_tts.py](https://github.com/user-attachments/files/25356501/frog_tts.py)
import pyttsx3
import os

# -------- STORY TEXT --------
text = """
It was a time when the whole world came to a standstill. Lockdowns were imposed due to the pandemic, and people went a little mad, confined within their homes.

During the second wave, we decided to stay at our farmhouse. It was monsoon, and the entire Western Ghats lay shrouded in a thick veil of fog. Driving was difficult even with the fog lamps on.

And then, suddenly, we noticed something. The whole road was writhing. Or so it seemed.

The road had come alive because it was full of frogs. Frogs upon frogs, crowding every inch of ground, croaking in unison.

That night, we caught a glimpse of the kingdom of frogs.
"""

engine = pyttsx3.init()
engine.setProperty('rate', 160)

output_path = os.path.expanduser(r"~/Documents/tts_project/frog_story.wav")

engine.save_to_file(text, output_path)
engine.runAndWait()

print("Saved:", output_path)

