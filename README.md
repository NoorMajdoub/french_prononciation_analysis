

## French Pronunciation Evaluator for Kids

###  Project Overview

This project is a **French pronunciation evaluator for children**, designed to analyze spoken sentences and provide **friendly, structured feedback** based on:
1. **Nasal vowels** (e.g., *on*, *an*, *un*)
2. **Over-articulation or foreign rhythm** (like English or Arabic influence)
3. **Liaison and final consonant rules** (silent letters, connected sounds)

It uses a child's **spoken sentence** and **phonetic transcription** to generate personalized feedback in a child-friendly tone.

---

### 🛠️ Features

- Accepts a **target sentence** and the **phonetic transcription** of the child's speech.
- Evaluates pronunciation based on:
  - Accuracy of nasal vowels
  - Native-like French rhythm
  - Correct liaisons and final consonant use
- Outputs:
  - ✅ What the child did well
  - ⚠️ What could be improved
  - 🎯 A helpful tip for each category
  - ⭐ An overall clarity score (1 to 5 stars)
- Can be adjusted for a more teacher/parent tone or child-directed tone

---

### ▶️ How to Use

1. **Open the Notebook**
   Open `french-pononciation-evalautor.ipynb` in Jupyter Notebook or Google Colab.

2. **Provide Input**
   - `result["text"]`: The correct sentence the child tried to say.
   - `transcription`: The phonetic transcription (IPA) of what the child actually said.

3. **Run the Evaluation**
   - The notebook will generate structured feedback focused on the 3 pronunciation areas.
   - Feedback is written in a **friendly, encouraging tone**, aimed directly at children.

---

### ✨ Example Prompt Template

```python
prompt = f"""🎧 Here's a sentence you said out loud, and this is how it sounded in special pronunciation symbols. I’m going to help you improve your French pronunciation by giving you some friendly tips!

We’ll look at:
1. Nasal sounds (like when your voice goes through your nose: "on", "an", "un")  
2. If you're using a different rhythm (like how English or Arabic sounds)  
3. How you connect words or finish them (like when some letters are silent or stick together)

For each part, I’ll tell you:
✔️ Something you did really well  
⚠️ Something that could sound even better  
🎯 A fun tip or trick to help you improve

At the end, I’ll give you a little star score out of 5 ⭐️

---

📝 **What you wanted to say:**  
{result["text"]}

🔤 **How it sounded when you said it (pronunciation symbols):**  
{transcription}
"""
```

---

### 🔧 Requirements

This project assumes you're using a language model (like OpenAI’s GPT) to generate feedback. You'll need:
- Python 3.x
- `openai` or equivalent API access (if integrated)
- Jupyter Notebook environment

---

### 🧒 Who is this for?

- French teachers and speech therapists working with children
- Educational app developers
- Parents teaching French at home


