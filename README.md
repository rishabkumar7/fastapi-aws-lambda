# FastAPI App on AWS Lambda

This repository is a demo for hosting a FastAPI application on AWS Lambda using Mangum.

## Project Structure

``` sh
. ├── .gitignore 
  ├── main.py 
  ├── README.md 
  └── requirements.txt
```

## Requirements

- Python 3.9+
- AWS Account

## Installation

1. Clone the repository:

    ```sh
    git clone https://github.com/rishabkumar7/fastapi-aws-lambda.git
    cd fastapi-aws-lambda
    ```

2. Create a virtual environment and activate it:

    ```sh
    python -m venv .venv
    .venv\Scripts\Activate  # On Linux/Mac use `source .venv/bin/activate`
    ```

3. Install the dependencies:

    ```sh
    pip install -r requirements.txt
    ```

## Running Locally

You can run the FastAPI application locally using Uvicorn, but will need to install uvicorn:

```sh
pip install uvicorn
uvicorn main:app --reload
```

## Deploying to AWS Lambda

Zip your FastAPI application and upload the zip to an AWS Lambda Function.

Zip on Windows:

``` powershell
Compress-Archive .\.venv\Lib\site-packages\* aws_lambda.zip
Compress-Archive .\main.py -Update aws_lambda.zip
```

## Demo

![https://img.youtube.com/vi/b0XCH04K8eQ/maxresdefault.jpg](https://youtu.be/b0XCH04K8eQ)
