# TechCorp Service Mesh - Internal Infrastructure

## Alex's Investigation Log - Day 3

I've isolated the compromised service configurations here. Three services, three pieces of evidence.

## How The Insider Operated

They knew exactly how our microservices architecture works. They moved through the system methodically:

1. They already had valid credentials (suspicious)
2. They modified routing rules to intercept traffic
3. They set up shadow logging to an unauthorized destination

## Reading These Configurations

Each YAML file represents a microservice. I've added investigation notes in the `metadata` sections - those weren't part of the original configs.

**Start with:** `auth-service.yaml`  
It will guide you to the next file. Follow the service dependency chain.

## What You're Looking For

As you read through these, you're building a profile of the insider:
- **What they knew:** Deep understanding of our architecture
- **What they did:** Specific modifications to routing and logging
- **What they deployed:** Physical hardware (this is the smoking gun)

The data service configuration reveals their final move - and a clue to their identity.

## A Personal Note

I've been at TechCorp for 5 years. I know everyone here. The fact that it's an insider... that's what haunts me. Someone I've worked with, maybe even trusted.

But the evidence doesn't lie. Keep following it.

— Alex