# Day 6 – Load Balancing with Nginx

## Objective
Implement load balancing across multiple backend servers using Nginx.

## Architecture

User → Nginx Load Balancer → Backend Servers

## Implementation

1. Created second backend VM.
2. Installed Python HTTP server on both backend machines.
3. Configured Nginx upstream servers.
4. Enabled request distribution.

## Nginx Configuration

upstream backend_servers {
    server 10.0.1.4:8000;
    server 10.0.1.5:8000;
}

location / {
    proxy_pass http://backend_servers;
}

## Result

User requests are distributed across multiple backend servers.

## Key Learning

Load balancing improves scalability and reliability in cloud architectures.
