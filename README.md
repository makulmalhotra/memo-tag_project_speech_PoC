# memo-tag_project_speech_PoC
This project builds a simple tool to spot early signs of cognitive decline (like memory issues) by analyzing voice recordings. It’s part of MemoTag’s speech intelligence system. The goal is to process voice clips and find patterns, like pauses or stumbles, that might show cognitive stress.

We used a Google Colab notebook with Python tools like librosa (for audio), speech_recognition (to turn speech into text), and scikit-learn (for patterns). Since we didn’t have real audio, we tested with fake data for 10 voice samples, tracking six features:

Pauses in sentences
Filler words (“uh,” “um”)
Speech speed
Voice pitch changes
Repeated words (for memory issues)
Unfinished sentences
The tool extracts these features, groups similar samples using clustering (K-Means), and flags odd ones as risks (Isolation Forest). It also has a function to score new audio for cognitive decline risk. Graphs show which features matter most, and a short report explains the findings.

## Conclusions 
This project shows voice analysis can catch signs of cognitive decline. Pauses and filler words stood out as big clues—people with more of these seemed at risk. Speech speed and unfinished sentences also helped spot differences. The clustering grouped samples well, and the anomaly detection caught unusual patterns, like too many pauses.

Since we used fake data, real-world tests are needed next. The tool is simple and clear, great for early ideas, but could improve with better word error detection and real patient audio.


