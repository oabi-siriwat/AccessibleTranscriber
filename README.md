# Accessible Transcriber

Turns Thai speech into text, live from a microphone or from the computer's own sound, or from a sound or video file. Everything runs on your computer: no internet and no account are needed.

It is made for screen reader users. The window uses standard Windows controls, every button has a Ctrl key, for example Ctrl+O opens a file, and NVDA reads each new piece of text as soon as the speaker pauses.

คู่มือภาษาไทย: [README.th.md](README.th.md)

## Download

Download the latest version: [AccessibleTranscriber.zip](https://github.com/oabi-siriwat/AccessibleTranscriber/releases/latest/download/AccessibleTranscriber.zip)

This link always gives the newest version. Extract the zip: it holds an AccessibleTranscriber folder with `AccessibleTranscriber.exe` and the English and Thai manuals (`AccessibleTranscriber_README.txt`, `AccessibleTranscriber_README_TH.txt`). Open `AccessibleTranscriber.exe` from that folder, not from inside the zip. It is one file of about 200 MB, because the speech model is inside it. It needs no installing.

The file is not signed. Windows SmartScreen may warn that it does not know the publisher. Choose More info, then Run anyway.

## Requirements

- Windows 10 or Windows 11, 64-bit
- A microphone, or sound playing on the computer, or a sound or video file
- NVDA is not required, but the program speaks through it when it is running

## How to use it

1. Choose the input (Ctrl+I): a microphone or the computer sound.
2. Press Ctrl+T to start listening, and speak. The text appears in the Transcript box.
3. Press Ctrl+T again to stop, then Ctrl+S to save the text as a file.

Ctrl+O opens a sound or video file to transcribe. When it is done, the text is saved by itself as a .txt with the same name, in the same folder as the sound file (an existing file is never overwritten). While a file is transcribed, the window shows only a status box with the file, the percentage and the time left, and only three keys work: Space says the progress, F5 the status, Escape stops (it asks first). Ctrl+comma opens the settings: the menu language (Thai or English), reading new text aloud, a time before each line, numbers as digits, removing fillers such as เอ่อ อ่า อืม, the word list, and how long a pause makes a space or a new line.

The word list (Edit word list in Settings) fixes words the program often gets wrong. Write one word per line as misheard=right. It comes with common English words that the model writes in Thai letters, for example ฟิตแบค=feedback, so they come out in English. Put # before a line to stop that word changing. Ctrl+H opens the full help inside the program.

## Updates

Each time it opens, the program checks for a newer version. When there is one, it asks first, then downloads it, checks the file and restarts. When there is none, it says nothing. While the update downloads, there is a beep on every percent and the percentage is said every 10 seconds; the window shows only a status box, Space says the percentage and the time left, F5 the status, and Escape stops the download (it asks first). Settings (Ctrl+comma) also has a Check for update button.

## Credits

- Speech model: Typhoon ASR Real-Time by Typhoon (SCB 10X), licence CC BY 4.0
- Cutting the sound at pauses: Silero VAD (MIT)
- Thai word list: PyThaiNLP (CC0)

## License

Free to use and to share unchanged at no charge. See [LICENSE](LICENSE).
