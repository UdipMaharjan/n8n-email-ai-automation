# AI-Powered Email Automation & Classification

An automated email-processing workflow built with n8n, Gemini AI,
JavaScript, Gmail, Formspree, and Google Sheets.

## Overview

This project demonstrates how workflow automation and LLM-based
text processing can be combined to process incoming customer/contact
messages automatically.

The workflow receives emails generated from a Formspree contact form,
uses Gemini AI to analyze and classify the message, extracts structured
information, and records the result in Google Sheets.

## Workflow

Formspree Contact Form
        ↓
Gmail Trigger
        ↓
IF / Filtering
        ↓
Get Email Message
        ↓
Gemini AI Agent
        ↓
JavaScript Data Processing
        ↓
Google Sheets

## Technologies

- n8n
- Gmail
- Gemini AI
- JavaScript
- Google Sheets
- Formspree

## Key Features

- Automated email detection
- Conditional workflow filtering
- AI-powered email analysis
- Priority classification
- Structured information extraction
- JavaScript-based data transformation
- Automated Google Sheets record creation

## How It Works

### 1. Email Trigger

The workflow monitors the Gmail inbox for emails generated from
the Formspree contact form.

### 2. Filtering

An IF node checks whether the incoming message matches the required
criteria before continuing through the workflow.

### 3. Email Retrieval

The email message is retrieved so that its contents can be passed
to the AI processing stage.

### 4. AI Analysis

Gemini analyzes the incoming message and extracts relevant information.
It also assigns a priority based on the predefined classification
criteria.

### 5. Data Processing

A JavaScript node processes the AI response and prepares the extracted
information in a structured format.

### 6. Data Storage

The processed information is appended to Google Sheets for organized
record keeping.

## Example Use Case

A visitor submits a message through a portfolio contact form:

> "I would like to discuss a potential project and would like
> to schedule a meeting."

The workflow automatically receives the message, analyzes its
content, determines an appropriate priority, extracts the relevant
information, and records it in Google Sheets.

## Workflow Screenshot

![n8n Workflow](screenshots/n8n-workflow.png)

## Project Purpose

This project was built to gain practical experience with:

- Workflow automation
- Event-driven workflows
- LLM integration
- Text classification
- Data extraction
- API/service integration
- Structured data processing