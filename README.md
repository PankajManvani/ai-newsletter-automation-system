# ai-newsletter-automation-system
End-to-end AI newsletter automation system built with n8n that ingests RSS feeds, analyzes news articles, generates AI summaries and insights, and publishes structured newsletters automatically.
AI News Ingestion & Storage Automation (n8n)

This project is an automated AI and technology news ingestion pipeline built using n8n.
The workflow collects news from multiple RSS sources, filters relevant articles, scores them using AI models, and stores the processed data in Airtable for further analysis and publishing.

The system eliminates manual news curation and creates a structured dataset of relevant AI and tech news articles.

🚀 Project Overview

This automation workflow performs the following operations:

Fetches RSS feeds from configured news sources.

Filters active sources and processes them sequentially.

Extracts article metadata including title, link, summary, and publication date.

Uses AI models to analyze and score articles based on importance and virality.

Filters high-quality articles using predefined thresholds.

Stores the processed articles in Airtable for future use in newsletters or analytics.

This pipeline enables automated news monitoring and structured data storage for downstream applications like AI-powered newsletters or dashboards.

⚙️ Workflow Architecture

Main workflow stages:

Configuration Setup

Loads RSS source configuration from Google Sheets.

RSS Feed Collection

Fetches RSS feeds from multiple sources.

Content Processing

Extracts article metadata such as:

Title

Link

Summary

Publication Date

Source

AI-Based Article Scoring

Uses AI models to evaluate:

Importance score

Virality score

Filtering

Keeps only articles above defined thresholds.

Storage

Saves filtered articles in Airtable for structured storage.

🛠 Tech Stack

n8n – Workflow automation platform

OpenAI API – Article scoring and analysis

RSS Feeds – News ingestion source

Google Sheets – Source configuration

Airtable – Data storage

📂 Project Structure
ai-newsletter-automation-system
│
├── AI News #1_ Ingest & Store.json
└── README.md

The JSON file contains the exported n8n workflow that can be imported directly into n8n.

🔄 How to Use

Import the JSON workflow into n8n.

Configure required credentials:

OpenAI API

Google Sheets

Airtable

Add RSS feed sources in the Google Sheet configuration.

Execute the workflow to start ingesting and storing AI news articles.

👨‍💻 Author

Pankaj Manvani
