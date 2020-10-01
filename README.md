# Named Entity Recognition using a Bidirectional Long Short Term Memory (LSTM)

## Model

- The used dataset is provided by [kaggle](https://kutt.it/udr2g1)
- The model is build using Keras Deep learning API, you can find the implementation in [this
  kaggle notebook](https://kutt.it/bW4pgW)

## Usage

- Example Usage

```bash
curl -X GET "https://frozen-coast-03690.herokuapp.com/classify/Ali is swimming"
```

- The API is hosted on a heroku instance for easier access
- The API is implemented using [FastAPI](https://fastapi.tiangolo.com/) providing out-of-box documentation, checkout
  autogenerated docs in [heroku](https://frozen-coast-03690.herokuapp.com/docs)

## Local Development

- Install the requirements `pip install -r requirements.txt`
- start the development server with hot-reloading `uvicorn main:app --reload`

### Directory structure

├── main.py &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;=> main program file with API implementation <br>
├── NER-BiLSTM.h5 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;=> trained tensorflow model <br>
├── Procfile &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;=> heroku service file <br>
├── README.md &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;=> ... <br>
├── requirements.txt &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;=> required pip packages <br>
└── word_idx.obj &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;=> list of all words in used corpus <br>
