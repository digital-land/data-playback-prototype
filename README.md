# Data submission playback prototype

Based on the [govuk-flask-prototype-kit](https://github.com/digital-land/govuk-flask-prototype-kit)

### Getting staerted

We recommend using a virtual env.

Install dependencies

`make init`

Run flask application

`flask run`

Run flask application and watch for changes

`make watch`

### Before pushing changes

The first time you run the tests you will need to install the chromium browser for play-wright

```
python -m playwright install chromium
```

Run the following to eyeball the pages are all still working

```
pytest tests/acceptance -p no:warnings --headed --slowmo 1000
```
