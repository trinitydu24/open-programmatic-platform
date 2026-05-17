# Open Programmatic Platform

## Overview

Open Programmatic Platform (OPP) is an open-source experimental adtech analytics platform designed to simulate and analyze a modern programmatic advertising ecosystem.

The project combines:
- real-time RTB simulation
- fraud detection
- attribution modeling
- carbon/emissions analytics
- interactive dashboards
- machine learning
- statistical analytics

The goal is to build a realistic portfolio-grade platform inspired by real adtech infrastructures used by DSPs, SSPs, media analytics teams, and programmatic advertising companies.

---

# Vision

This project aims to demonstrate how a modern programmatic advertising platform can:
- generate RTB events
- analyze advertising performance
- detect suspicious traffic
- estimate environmental impact
- measure marketing attribution
- expose analytics through dashboards and APIs

The platform is built progressively as a long-term engineering and data science portfolio project.

---

# Main Features

## RTB Simulation Engine
Simulates:
- auctions
- ad impressions
- bids
- clicks
- conversions
- users
- campaigns
- publishers

---

## Fraud Detection Engine
Detects:
- click fraud
- bot traffic
- suspicious publishers
- anomalous user behavior

Using:
- anomaly detection
- machine learning
- statistical analysis

---

## Carbon Intelligence Engine
Estimates:
- energy consumption
- CO₂ emissions
- campaign environmental impact

Designed to explore sustainability challenges in digital advertising.

---

## Attribution Engine
Implements:
- last-click attribution
- probabilistic attribution
- Markov chain attribution models
- advanced analytics

---

## Analytics Dashboard
Provides:
- campaign KPIs
- fraud monitoring
- carbon metrics
- attribution insights
- real-time analytics

Built with R Shiny and Plotly.

---

# Architecture

```text
                ┌────────────────────┐
                │ RTB Simulator      │
                │ Python             │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │ PostgreSQL         │
                │ Event Storage      │
                └─────────┬──────────┘
                          │
        ┌─────────────────┼─────────────────┐
        ▼                 ▼                 ▼

┌───────────────┐ ┌───────────────┐ ┌───────────────┐
│ Fraud Engine  │ │ Carbon Engine │ │ Attribution  │
│ Python ML     │ │ R Analytics   │ │ Python + R   │
└──────┬────────┘ └──────┬────────┘ └──────┬────────┘
       │                 │                 │
       └─────────────────┼─────────────────┘
                         ▼

               ┌────────────────────┐
               │ Shiny Dashboard    │
               │ Analytics UI       │
               └────────────────────┘
```

---

# Technology Stack

## Backend
- Python
- FastAPI

---

## Data Science & Analytics
- R
- Tidyverse
- Scikit-learn
- XGBoost

---

## Visualization
- Shiny
- Plotly

---

## Database
- PostgreSQL

---

## Infrastructure
- Docker
- Kafka
- Redis

---

# Project Structure

```text
open-programmatic-platform/

├── backend/
├── analytics/
├── dashboard/
├── database/
├── datasets/
├── docs/
├── tests/
└── README.md
```