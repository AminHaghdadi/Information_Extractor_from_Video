# Information_Extractor_from_Video

![image](https://img.shields.io/badge/OpenAI-412991.svg?style=for-the-badge&logo=OpenAI&logoColor=white)
![image](https://img.shields.io/badge/FastAPI-009688.svg?style=for-the-badge&logo=FastAPI&logoColor=white)

This video summarization application allows users to upload a video and receive a concise text-based summary in return. It is built using FastAPI for the web framework and API creation. When a video is uploaded, the application leverages the pytube package to download the video file and save it locally. It then uses the subprocess module to convert the video to an audio format. The audio file is passed to the OpenAI Whisper speech recognition model which transcribes it into text. Finally, the text is summarized into key bullet points using OPENAI chatGPT. The summarized output is returned to the user in an easy-to-skim list of the main topics and ideas covered in the video. This video summarization tool provides a convenient way for users to get the key information from a video without needing to watch the full clip. The integration of FastAPI, pytube, Whisper, and text summarization algorithms makes it possible to take a raw video upload and distill it down to just the essential points.

## Deployment

To deploy this project run

1:
```bash
  git clone https://github.com/AminHaghdadi/Information_Extractor_from_Video.git
```
2: install requirements:
```bash
  pip install -r requirement.txt 
```
3:

Enter your OpenAI API KEY in app.py 

4: Run in Terminal
```bash
uvicorn app:app --reload
```
