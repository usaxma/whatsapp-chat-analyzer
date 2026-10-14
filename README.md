# WhatsApp Chat Analyzer

NLP / EDA tool for exported WhatsApp chats. The notebook walks through parsing and analysis; a Streamlit app lets you upload a `.txt` export and inspect activity, word clouds, and busiest users.

## Skills

- Chat-log parsing (timestamps, users, system messages)
- Text stats, URL extraction, emoji counts
- Word clouds with Hinglish stopwords
- Time-series activity plots
- Streamlit dashboard

## How to get a chat file

In WhatsApp: chat → Export chat → Without media. Upload that `.txt` in the app.

## Run the notebook

```bash
pip install -r requirements.txt
jupyter notebook notebooks/WhatsApp_Chat_Analysis.ipynb
```

## Run the app

```bash
cd app
pip install -r ../requirements.txt
streamlit run app.py
```

## Structure

```
whatsapp-chat-analyzer/
├── notebooks/
│   └── WhatsApp_Chat_Analysis.ipynb
├── app/
│   ├── app.py
│   ├── preprocess.py
│   ├── stats.py
│   └── stop_hinglish.txt
├── requirements.txt
└── README.md
```
