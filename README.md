# llm-box
This repo is just a handful of docker files that describe a basic LLM server setup. There's nothing special going on here, I just wanted a way to track my configuration.

## Whats included here exactly?
A the moment theres one compose file that sets up an OpenWebUI server and a FireCrawl instance, plus a handful of compose files that each describe a LlamaCpp server configured to run a model on my 3060 12GB.
The configs here are by no means optimal, I run models that are way too big for my GPU because its fun and I don't care about cratering my t/s. I have a ton of DDR3 laying around so I just offload anything that can't fit on the GPU into system ram.

**IF YOU USE THIS EXPECT IT TO BE SLOW**

## Usage
`docker compose -f docker-compose.yml -f <name-of-model-compose-file> up -d`
