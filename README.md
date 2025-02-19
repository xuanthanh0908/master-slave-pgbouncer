# PgBouncer with Docker Compose Setup Guide

## Table of Contents

1. [Introduction](#introduction)
2. [System Requirements](#system-requirements)
3. [Setup and Deployment](#setup-and-deployment)
   - [Install Docker and Docker Compose](#install-docker-and-docker-compose)
   - [Configure `docker-compose.yml`](#configure-docker-composeyml)
   - [Configure PgBouncer](#configure-pgbouncer)
4. [Starting the System](#starting-the-system)
5. [Configure NestJS to Connect to PgBouncer](#configure-nestjs-to-connect-to-pgbouncer)
6. [Testing and Verification](#testing-and-verification)
7. [Troubleshooting](#troubleshooting)

## Introduction

This guide explains how to set up **PgBouncer** for PostgreSQL Master and Read Replica using **Docker Compose** to manage database connections efficiently.

## System Requirements

- **Docker** and **Docker Compose**
- **PostgreSQL 15** or compatible
- **PgBouncer** for connection pooling

## Setup and Deployment

### Install Docker and Docker Compose

Ensure **Docker** and **Docker Compose** are installed on your system:

```bash
# Install Docker
sudo apt update
sudo apt install docker.io

# Install Docker Compose
sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
```
