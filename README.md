Official pre-release repository for [The 01 Project](https://twitter.com/hellokillian/status/1745875973583896950).

> **4** days remaining until launch

<h1 align="center">○</h1>

<p align="center">
    <a href="https://discord.gg/Hvz9Axh84z">
        <img alt="Discord" src="https://img.shields.io/discord/1146610656779440188?logo=discord&style=social&logoColor=black"/></a>
    <br>
    <br>
    <strong>The open-source language model computer.</strong><br>
    <!-- <br><a href="https://openinterpreter.com">Preorder the Light</a>‎ ‎ |‎ ‎ <a href="https://openinterpreter.com">Get Updates</a>‎ ‎ |‎ ‎ <a href="https://docs.openinterpreter.com/">Documentation</a><br> -->
</p>

<br>

![poster](https://pbs.twimg.com/media/GDqTVYzbgAIfLJf?format=png&name=4096x4096)

<br>

<!-- <p align="center">
Today is launch day. Read our <a href="https://changes.openinterpreter.com/log/the-new-computer-update">founding statement →</a>
</p>
<br> -->

```shell
pip install _01OS
```

> Not working? Read our [setup guide](https://docs.openinterpreter.com/getting-started/setup).

```shell
01 # Run this to start the 01.
```

<br>

**The 01 project** is an open-source ecosystem for artificially intelligent devices.

By combining code-interpreting language models with speech recognition and voice synthesis, the 01’s flagship operating system (the _01OS) can power conversational, computer-operating AI devices similar to the Rabbit R1 or the Humane Pin.

We intend to become the “Linux” of this space— open, modular, and free for personal or commercial use.

<br>

## Setup

### Install dependencies

```bash
# MacOS
brew install portaudio ffmpeg cmake

# Ubuntu
sudo apt-get install portaudio19-dev ffmpeg cmake
```

If you want to run local speech-to-text using Whisper, install Rust. Follow the instructions given [here](https://www.rust-lang.org/tools/install).

### Install and run the 01 CLI

```shell
pip install _01OS
```

```shell
01 # This will start a server and a client.

01 --server # Start only a server.
01 --server --expose # Start and expose a server via Ngrok. This will print a `server_url` for clients to connect to.

01 --client --server_url your-server.com # Start only a client.
```

### Swap out service providers

The 01 is model agnostic to speech-to-text, text-to-speech, and language model providers.

Select your provider by running:

```shell
01 --tts-service openai
01 --llm-service openai
01 --stt-service openai
```

[View all providers ↗](https://docs.litellm.ai/docs/providers/), or [join the 01 team by adding a service provider. ↗]()

### Run the 01 locally

Some service providers don't require an internet connection.

The following command will attempt to download and use the best providers for your hardware:

```shell
01 --local
```

## How Does it Work?

The 01 equips a language model (wrapped in a voice interface) with an `exec()` function, which allows it to write and run code to control computers.

We only stream speech to/from the end user's device.

# Contributing

Please see our [contributing guidelines](docs/CONTRIBUTING.md) for more details on how to get involved.

### Setup for development

```bash
# Clone the repo
git clone https://github.com/KillianLucas/01.git

# Go to the _01OS directory
cd _01OS

# Install python dependencies
poetry install

# Run it
poetry run 01
```

<br>

# Roadmap

Visit [our roadmap](https://github.com/KillianLucas/open-interpreter/blob/main/docs/ROADMAP.md) to see the future of the 01.

<br>

## Background

### [Context ↗](https://github.com/KillianLucas/01/blob/main/CONTEXT.md)

The story of devices that came before the 01.

### [Inspiration ↗](https://github.com/KillianLucas/01/tree/main/INSPIRATION.md)

Things we want to steal great ideas from.

<br>

## Direction

### [Goals ↗](https://github.com/KillianLucas/01/blob/main/GOALS.md)

What we're going to do.

### [Use Cases ↗](https://github.com/KillianLucas/01/blob/main/USE_CASES.md)

What the 01 will be able to do.

<br>
