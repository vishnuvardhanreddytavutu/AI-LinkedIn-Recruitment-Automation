# AI-Powered LinkedIn Recruitment Automation Pipeline

An AI-powered recruitment automation pipeline built using n8n, JavaScript, Apify, PhantomBuster, OpenAI, and Google Sheets.

## Overview

This project automates multiple stages of the recruitment workflow, including candidate sourcing, profile enrichment, LinkedIn outreach, job-search scraping, and candidate status tracking.

## Workflow

Job Role + Location
        ↓
AI Search Query Generation
        ↓
LinkedIn Candidate Sourcing
        ↓
Candidate Profile Data
        ↓
Candidate Enrichment
        ↓
Google Sheets
        ↓
LinkedIn Outreach Automation
        ↓
Connection / Reply Status
        ↓
Candidate Tracking

## Workflows

### 01 - LinkedIn Sourcing

Automates candidate sourcing based on job role, experience, and location.

**Technologies:**
- n8n
- OpenAI
- Apify
- JavaScript
- Google Sheets
- Webhooks

### 02 - LinkedIn Enrichment Callback

Receives candidate profile information through a webhook and updates candidate records.

**Technologies:**
- n8n
- Webhooks
- JavaScript
- Google Sheets

### 03 - LinkedIn Auto Connect

Triggers LinkedIn outreach automation using a candidate's LinkedIn profile URL.

**Technologies:**
- n8n
- PhantomBuster
- HTTP APIs
- Webhooks

### 04 - LinkedIn Status Tracker

Processes candidate status information and tracks recruitment stages such as:

- Invitation sent
- Request accepted
- Replied

Candidate information is stored and updated in Google Sheets.

### 05 - LinkedIn Profile Scraping

Experimental workflow for LinkedIn profile-search automation using AI, JavaScript batching, and HTTP requests.

**Technologies:**
- n8n
- OpenAI
- JavaScript
- HTTP APIs

### 06 - Job Search Scraping

Experimental job-search scraping workflow using Apify to collect job-search results based on configured search criteria.

**Technologies:**
- n8n
- Apify
- HTTP APIs
- Scheduled workflows

## Tech Stack

- n8n
- JavaScript
- OpenAI
- Apify
- PhantomBuster
- Google Sheets
- REST APIs
- Webhooks
- JSON

## Security

All API keys, authentication tokens, private webhook URLs, private Google Sheet identifiers, and other sensitive credentials have been removed or replaced with placeholders in the public workflow files.

## Project Structure

```text
AI-LinkedIn-Recruitment-Automation/
│
├── README.md
│
└── workflows/
    ├── 01-linkedin-sourcing.json
    ├── 02-linkedin-enrichment-callback.json
    ├── 03-linkedin-auto-connect.json
    ├── 04-linkedin-status-tracker.json
    ├── 05-linkedin-profile-scraping.json
    └── 06-job-search-scraping.json
