# go-pubsub
Simple Golang Google Pubsub Project

## Table of Contents
- [Installation](#installation)
- [Requirements](#requirements)
- [Usage](#usage)
- [Features](#features)

# With Credentials File
1. Change Variable creds in publish/publish.go and subscribe/subscribe.go to true

2. Add .env
```
ACCELERATION=path/to/creds.json
```

# Local
## Installation
```
https://github.com/wildanfaz/go-pubsub.git
```

## Requirements
1. Install python@3.9
```
brew install python@3.9
```

2. Install [gcloud CLI](https://cloud.google.com/sdk/docs/install)

```
./google-cloud-sdk/install.sh
```

```
./google-cloud-sdk/bin/gcloud init
```

3. Start gcloud pubsub
```
./google-cloud-sdk/bin/gcloud beta emulators pubsub start --project=notifier --host-port=localhost:8000
```

4. Add .env
```
PUBSUB_EMULATOR_HOST=localhost:8000
```

5. Change Variable creds in publish/publish.go and subscribe/subscribe.go to false

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
- Publish
- Subscribe
