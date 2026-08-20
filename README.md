# Speech-to-Text and Text-to-Speech Chatbot — feat. GlowBot
 
A Java console application that combines text-to-speech, a basic keyword chatbot, and **GlowBot**, a mood/outfit "bestie" chatbot with dynamic, template-based responses and a built-in user feedback system, all powered by the FreeTTS speech synthesis engine.

## Project Description
 
This project started as a simple Text-to-Speech and chatbot demo built on [FreeTTS](https://freetts.sourceforge.io/docs/index.php), an open-source Java speech synthesis engine. I expanded it by adding **GlowBot**, a themed chatbot that:
 
- Detects the mood or topic behind what you type (outfit, confidence, tiredness, sadness, or general chat) using keyword matching
- Generates a **dynamic response** each time by randomly selecting from a bank of template replies for that category and inserting a snippet of your own message into the reply, so it never feels like the same canned line twice
- Speaks every response out loud using the existing FreeTTS voice engine
- Asks you to **rate each response 1–5** and logs that rating, along with a timestamp, your message, and the bot's reply, to a local file (`glowbot_feedback.txt`) so feedback can be reviewed or analysed later
- Prints a session average rating when you exit GlowBot
The original features (plain text-to-speech, the basic hello/bye chatbot, and a voice-listing utility) are still in the app, GlowBot is an added menu option, not a replacement.
