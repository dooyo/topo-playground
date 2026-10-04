# Topo Playground

An interactive demo of Topo, a live map of how a company's software works: code, services, data, cloud and monitoring in one view.

Four made-up sample companies to switch between:

- **acme-shop**: Node and Go services on Kubernetes
- **globex-freight**: a NestJS monorepo (Nx) with Kafka, gRPC and Prisma
- **initech-claims**: AWS serverless in Python (Lambda, Step Functions, EventBridge)
- **hooli-health**: a Rails monolith being split into services

Each one has four scenarios: ask how something works, see what breaks if you change it, replay an incident, and compare an AI coding tool with and without the map.

Everything is sample data. The page is a single static `index.html`, served by nginx on port 8000.

```sh
docker build -t topo-playground . && docker run -p 8000:8000 topo-playground
```

Logos: [Simple Icons](https://simpleicons.org) (CC0) and the AWS Architecture Icons via [aws-icons](https://github.com/MKAbuMattar/aws-icons) (MIT). All logos belong to their owners.
