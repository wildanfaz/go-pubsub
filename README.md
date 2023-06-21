# go-pubsub

Simple Golang Google Pubsub Project (Local Test)

## Table of Contents

- [Installation](#installation)
- [Requirements](#requirements)
- [Usage](#usage)
- [Features](#features)

## Installation
```
git clone https://github.com/wildanfaz/go-pubsub.git
```

## Requirements
1. Install python@3.9
```
brew install python@3.9
```

2. Install [gcloud CLI](https://cloud.google.com/sdk/docs/install)

3. Start gcloud
```
./google-cloud-sdk/bin/gcloud beta emulators pubsub start --project=notifier --host-port=localhost:8000
```

4. Add .env
```
PUBSUB_EMULATOR_HOST=localhost:8000
```

## Usage
Subscribe
```
make s
```

Publish
```
make p
```


## Features

- Publish Message
- Subscribe Topic
