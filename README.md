# mini-rag

## Requirements

- Python 3.8 or later

##### Install Python using MinicConda

1) Download and Install MiniConda from [here](https://docs.anaconda.com/miniconda/#quick-command-line-install)
2) Create a new envoronment using the following conda command:
```bash
$ conda create -n mini-rag python=3.8
```
3) Activate the environment:
```bash
$ conda activate mini-rag
```
### (Optional) Setup you command line interface for better readability
```bash
$ export PS1="\[\033[01;32m\]\u@\h:\w\n\[\033[00m\]\$ "
```

## Installation

### Install the required packages
```bash
$ pip install -r requirements.txt
```

### Setup the envornment variables 
```bash
$ cp .env.example .env
```
Set your environment variables in the `.env` file. Like the `OPENAI_API_KEY` value.

### Run the FastAPI server
```bash
$ uvicorn main:app --reload --host 0.0.0.0 --port 5000
```