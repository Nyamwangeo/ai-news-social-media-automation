# AI News and Social Media Automation

An AI-powered n8n automation system that researches current news, verifies sources, removes duplicate stories, ranks content by relevance, generates platform-specific posts and manages publishing across LinkedIn, Facebook and X.

![Workflow Overview] https://github.com/Nyamwangeo/ai-news-social-media-automation/blob/main/docs_screenshots_complete-workflow.png 

## Project Overview

This project automates the complete content lifecycle, from discovering relevant news to preparing and distributing posts across multiple social-media platforms.

The system combines scheduled workflows, RSS feeds, web research, AI models, APIs and Google Sheets to create a structured content research and publishing pipeline.

## Key Features

- Automated news collection from RSS feeds
- Web search integration for additional sources
- Recent-content filtering
- Duplicate detection within and across workflow runs
- AI-powered relevance screening
- Multi-source story verification
- Article text extraction and validation
- Content ranking and selection
- Platform-specific content generation
- LinkedIn personal and company-page publishing
- Facebook page publishing
- X post publishing
- Scheduled execution and queue management
- Publishing-status tracking
- Error handling and retry logic
- AI model and API cost optimisation

## Workflow Architecture

The solution contains two main automation pipelines.

### 1. Research and Content Generation

```text
Schedule Trigger
→ Read RSS Feeds
→ Filter Recent Stories
→ Remove Duplicates
→ Screen for Relevance
→ Search Supporting Sources
→ Download Candidate Articles
→ Extract and Validate Content
→ Verify Claims
→ Rank Stories
→ Generate Platform-Specific Posts
→ Add Approved Content to Queue

### 2. Multi-Platform Publishing
Schedule Trigger
→ Read Content Queue
→ Select Approved Posts
→ Check Selected Platforms
→ Publish to LinkedIn, Facebook and X
→ Merge Publishing Results
→ Update Queue Status

### Technologies and Integrations
n8n
Large language models
Prompt engineering
RSS feeds
Web search APIs
Google Sheets
LinkedIn API
Facebook Graph API
X API
HTTP and REST APIs
JavaScript code nodes
JSON data processing
