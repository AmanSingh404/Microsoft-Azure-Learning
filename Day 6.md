# Day 6 — Server Monitoring and Log Analysis

## Objective
Learn how to monitor server performance and analyze logs.

## Commands Used

top
htop
free -h
df -h
systemctl status nginx

## Log Monitoring

Nginx error logs:
/var/log/nginx/error.log

Nginx access logs:
/var/log/nginx/access.log

## Monitoring Script

#!/bin/bash

echo "CPU Load:"
uptime

echo "Memory Usage:"
free -h

echo "Disk Usage:"
df -h

## Result

Successfully monitored server health and analyzed logs to troubleshoot issues.

## Key Learning

Monitoring and logging are essential for maintaining system reliability.
