---
title: "Credencial Estudiantil Digital"
description: "Full-stack platform for digital student credential management enabling urban transportation access through mobile app and scalable backend."
image: "/projects/credencial-estudiantil.png"
date: 2025-12-01
tags: ["Flutter", "ASP.NET", "PostgreSQL", "TimescaleDB", "MediatR", "Android", "iOS"]
published: true
---

## The Problem

Students rely on physical credentials to access public transportation, leading to issues with loss, counterfeiting, and slow validation processes. Transportation companies need a modern and secure way to verify student identity while maintaining accurate access records.

## The Solution

**Credencial Estudiantil Digital** is a complete platform that digitalizes school credentials for urban transportation access. Students carry their verified credential on their smartphone, while the backend system records each validation in real-time with architecture designed to scale.

### How It Works

1. **For Students**: Download the mobile app → Register their school credential → Present the QR/digital code when boarding → Access validated instantly

2. **For Transportation Operators**: Scan the digital credential → System validates in real-time → Records access event → Generates usage reports

3. **For the Platform**:
   - **Mobile Application**: Built with Flutter for Android and iOS with secure credential storage
   - **Backend**: ASP.NET architecture with Mediator pattern (MediatR) designed for future microservices migration
   - **Database**: PostgreSQL with TimescaleDB for efficient time-series logging (validations, accesses)

The result: students with fast and secure access, operators with instant validation, and administrators with detailed analysis of transportation usage patterns.
