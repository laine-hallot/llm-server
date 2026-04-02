FROM node:latest
USER firecrawl:firecrawl
RUN npm i -g pnpm@10.25.0
COPY ./api-src/ /home/firecrawl/api/
WORKDIR /home/firecrawl/api/
CMD ["pnpm", "start"]
