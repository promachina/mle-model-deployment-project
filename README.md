# Model deployment project

Please do not fork this repository, but use this repository as a template for your refactoring project. Make Pull Requests to your own repository even if you work alone and mark the checkboxes with an x, if you are done with a topic in the pull request message.

## Project for today
The task for today you can find in the [project-description.md](project-description.md) file.

## Setup
```bash
pyenv local 3.10.11
python -m venv .venv
source .venv/bin/activate
pip install -U pip
pip install -r requirements.txt
```

## Test the API
```bash
curl -X POST -H "Content-Type: application/json" -d '{
    "ride_id": "some_id",
    "PULocationID": 1,
    "DOLocationID": 2,
    "trip_distance": 10.5
}' https://ml-webservice-w2ik3p5spa-ey.a.run.app/predict
```

