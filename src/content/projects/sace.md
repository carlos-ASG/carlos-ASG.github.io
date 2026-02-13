---
title: "SACE - Sistema de Administración y Control Escolar"
description: "Cross-platform mobile application for teachers and parents to manage and monitor student attendance in real-time with Supabase backend."
image: "/projects/sace.png"
date: 2025-10-01
tags: ["Flutter", "Supabase", "PostgreSQL", "MVP", "Android", "iOS"]
published: true
---

## The Problem

Traditional school attendance tracking is manual, delayed, and error-prone. Parents discover their children's absences days later, teachers waste time with paper lists, and institutions lack real-time data to intervene early in cases of absenteeism.

## The Solution

**SACE (Sistema de Administración y Control Escolar)** is a mobile application designed for DEGETI/CEBETIS 306 that digitalizes the attendance process. Teachers record attendance from their smartphone and parents receive instant notifications about their children's status.

### How It Works

1. **For Teachers**: Open the app at class start → Select their group → Mark attendance/absence with a tap → System automatically records date and time

2. **For Parents**: Receive push notification when their child is absent → Check attendance history → Identify absenteeism patterns

3. **For Administrators**: Monitor attendance rates by group → Detect chronic absenteeism cases → Generate reports for decision-making

### Technical Details

- **Frontend**: Developed with Flutter for simultaneous deployment on Android and iOS
- **Backend**: Supabase (PostgreSQL + integrated authentication) for rapid MVP iteration
- **Validation**: Functional pilot at CEBETIS 306 to assess market fit

The result: a validated prototype in a real scenario demonstrating technical viability and user acceptance before full-scale development.
