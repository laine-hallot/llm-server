# llm-server
This repo is just a handful of docker files that describe a basic LLM server setup. There's nothing special going on here, I just wanted a way to track my configuration.

## Whats included here exactly?
A the moment theres one compose file that sets up OpenWebUI, FireCrawl, Kokoro TTS, and LlammaCpp. Everything is configured to run on my 3060 12GB.
The configs here are by no means optimal, I run models that are way too big for my GPU because its fun and I don't care about cratering my t/s. I have a ton of DDR3 laying around so I just offload anything that can't fit on the GPU into system ram.

**IF YOU USE THIS EXPECT IT TO BE SLOW**

## Usage
Download the model files from huggingface and then run `docker compose -f docker-compose.yml up -d`
