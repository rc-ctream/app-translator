# 🗣️ Flutter Test Assignment: Real-Time Speech Translator

## Scenario  
Imagine you are traveling abroad. You are in a meeting where one person speaks **German** and the other **English**. Both want to understand each other without delay.  

The goal: build a **mobile app prototype** that works like a **personal live translator**.  
The app should **listen continuously**, **transcribe speech live**, and once a natural pause is detected, it should **translate the spoken segment** into the selected target language and show it on screen. This creates the feeling of a **synchronous conversation**.  

---

## What the app should do  

1. **Live Speech Recognition (Speech-to-Text)**  
   - The user presses **Start** to begin speaking.  
   - While speaking, their words are shown **live on screen** as transcription.  
   - When the speaker makes a **natural pause** (end of utterance), the transcription is finalized as a segment.  

2. **Translation (AI API)**  
   - Each finalized segment is sent to a **real translation API** (DeepL, Google Translate API,OpenAI or some of individual choice).  
   - Only finalized segments should be translated (not the interim words).  
   - The translation is displayed directly under the original text.  

3. **Conversation View**  
   - Show a **chronological list** of segments:  
     - Original transcription (with timestamp).  
     - Translation below it.  
   - The list grows as the conversation continues, like a live chat between languages.  

---

## Requirements  

- Input languages: **German** and **English** (user speaks either).  
- Output languages: **German ↔ English** (target language selectable at the start).  
- Use a **real API** for translation (no mocks).  
- Handle pauses correctly → translation only after utterance is complete.  
- Keep the code **clean and structured** (separation of logic, UI, and API handling).  
- Provide a short **README.md** with setup instructions and known limitations.  

---

## Bonus (optional, if time allows)  
- Show a small indicator while user is speaking vs. paused.  
- Allow copying translations to clipboard.  
- Add simple but clear styling to make the conversation view pleasant.  

---

## Timeframe  
- You have **5 hours** to complete this task.  
- Focus on the **use-case experience**: live transcription, segmented translation, and a clear conversation flow.  

---

## Deliverables  
- Push your code to the provided **Git repository** within **5 hours** after starting the assignment on a dedicated branch named by your fullname.
- Updated `README.md` with:  
  - Which translation API you used.  
  - Setup instructions (how to add API keys, how to run).  
  - Any assumptions or limitations.  

---

## Evaluation Criteria  
- **User experience**: does it feel like a conversation translator?  
- **Correct segmentation**: translations only after pauses, not mid-sentence.  
- **API integration**: proper use of a real translation service.  
- **Code clarity**: clean and understandable structure.  
- **Robustness**: handles errors gracefully (e.g., no crash on missing permission or API error).  
