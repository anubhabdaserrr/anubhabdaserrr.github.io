---
layout: page
permalink: /experience/
title: Experience
description: A reverse-chronological overview of my industry experience across software development, backend engineering, AI, and data-driven projects.
nav: true
nav_order: 1
---

<!-- For now, this page is assumed to be a static description of your courses. You can convert it to a collection similar to `_projects/` so that you can have a dedicated page for each course.

Organize your courses by years, topics, or universities, however you like! -->

## <img  src="../assets/img/textify.jpg"  alt="Textify Logo"  style="height: 1em; vertical-align: middle; border-radius: 10%; margin-right: 10px;"  />Textify Analytics

*Formerly Textify AI, Registered as CRCJ Technologies Private Limited*

*Indore, Madhya Pradesh, India (Remote) · Dec 2022 - Jul 2026*


### Software Development Engineer 2 (SDE-2)
Apr 2026 - Jul 2026

Tech Stack: *Python, FastAPI, MongoDB, Redis, Firebase, Amazon SES, S3, EC2, Voice AI & Telephony*

**Traveltalk24: AI-assisted itinerary generation for your next trip**

1. Built the core trip registration endpoint for scratch-built and email-sourced trips, supporting OTP assignment, document linking, edit history, and asynchronous GPT-4.1 enrichment; used to create 200+ trips.

2. Designed a 6-digit OTP system routing one endpoint to three flows: joining a friend's trip, cloning influencer or trending itineraries, and claiming email-generated trips, with single-claim locking and auto-linked pre-uploaded documents.

3. Built shareable document upload feature (text extraction, ChatGPT-powered classification, privacy controls) and a bill-splitting engine with an on-the-fly ledger, plus a streaming AI chatbot with Redis and MongoDB chat memory that answers using the trip's itinerary, documents, bills, and other trip details.

4. Built a streaming (SSE) trip component cost estimator that fans out per-activity flight, hotel, and ground-transport lookups concurrently, using an asyncio semaphore to cap parallel third-party API calls and stream partial results to the client as they complete.

5. Developed a portal where travel agencies view user itineraries and quote requests and send targeted offers (hotels, packages, bookings) via push notification or email fallback, with reusable ad templates and click analytics.

6. Integrated third-party APIs (Aviasales, Booking.com, Google Routes and Places) for flights, hotels, trains, buses and places, including async polling and merging of flight results, INR conversion, affiliate booking links and click tracking.


<img  src="../assets/img/tt24_ss.jpeg"  alt="tt24_ss"  style="max-width: 100%; height: auto; box-shadow: 0 4px 16px rgba(0, 0, 0, 0.15); border-radius: 4px; margin-bottom: 20px;">

### Software Development Engineer 1 (SDE-1)
Apr 2023 - Mar 2026

Tech Stack: *Python, FastAPI, JavaScript, Node.js, MongoDB, Redis, Supabase, Azure VMs, Document Intelligence API*

**Analytx: RAG-based charts search platform**

1. Developed a RAG-based charts search engine using Azure OpenAI API, MongoDB Atlas vector search, LangChain, to retrieve relevant charts, matching user query, from a database of 3 million+ charts.

2. Architected an automated data collection and transformation pipeline using Azure Document Intelligence API and OpenAI Batch API, cutting costs by 50% by shifting from immediate to asynchronous processing.

3. Implemented index-level pre-filtering for the Charts Search API's vector search (chart type, category, quality, date), assigning and validating filter attributes across 3M+ charts and benchmarking response times across filter combinations.

4. Engineered a suite of XGBoost models to predict news-success indicators, with MLflow-driven tracking, Docker-based deployment, and capabilities for real-time single-point inference and asynchronous batch inference.

5. Configured auto-deployments for multiple Python-FastAPI backend APIs to Azure VMs using GitHub Actions CI/CD, with basic Nginx reverse-proxy configuration to serve production websites.

6. Successfully migrated test and production deployments for multiple backend platforms from Azure to GCP, across our core product as well as separate client projects

7. Built an API access portal (HTML/CSS/JS) with sign-up, API-key-gated endpoints, tiered rate limits and usage analytics, enabling external companies to consume the Charts Search API.

8. Developed a real-time AI voice calling agent using FastAPI, Twilio, OpenAI speech-to-text, ElevenLabs text-to-speech, and Redis, integrating a pre-existing knowledge base with an LLM-powered response pipeline, asynchronous audio processing, low-latency filler responses, and conversational turn-taking; persisted audio recordings and responses in Azure Blob Storage.

<img  src="../assets/img/analytx_ss.jpeg"  alt="analytx_ss"  style="max-width: 100%; height: auto; box-shadow: 0 4px 16px rgba(0, 0, 0, 0.15); border-radius: 4px; margin-bottom: 20px;">

**Textify AI App & Builder Platform: Web platform for building no-code AI mini-apps**

1. Optimized app platform homepage load times by implementing Redis-based caching for personalized and non-personalized app recommendations serving 20,000+ users across categories including Top, New, Discover Peer Favourites, You Might Also Like, and Textify Curated.

2. Re-architected app execution from individual endpoints per app to a single reusable endpoint, dynamically resolving the app and user tier from each request, fetching its prompts and developer-configured data, and assembling the required context at runtime to generate the app-specific response.

3. Designed a tiered response architecture using Redis and Python RQ, asynchronously queueing requests for regular users while bypassing the queue for Pro users; implemented real-time, end-to-end streaming of text responses from OpenAI through our backend server to the client for Pro users, reducing time to first token by an estimated 60% compared with waiting for the complete response.

4. Built a data-integrated AI builder that lets developers enrich AI-generated responses with their own files (PDF, DOCX, TXT, MD) and outputs from a curated catalogue of 50+ third-party APIs, dynamically combining this data with user inputs within predefined prompts to generate richer, more current responses at runtime.

5. Added a modular AWS S3 storage layer for managing user and developer files, app animations, icons, and other application-level assets across separate buckets.

6. Integrated rich-output capabilities, including top-N image triggering based on developer-defined keywords using in AI-generated responses and customizable Markdown/HTML/CSS templates injected into system prompts to control output structure.

7. Supported biweekly hackathons by preparing workshop slide decks, building detailed submission forms, and reviewing app submissions from college students.

8. Designed dashboard app cards, alert screens, custom app UIs, pop-up forms in Figma

9. Published 500+ blogs across multiple WordPress sites through an automated pipeline, utlizing Wordress REST API & GPT-4o to assign categories, tags and excerpts, with featured image upload, SEO slugs, and batch publishing.

<img  src="../assets/img/textify_app_platform_ss.jpeg"  alt="textify_app_platform_ss"  style="max-width: 100%; height: auto; box-shadow: 0 4px 16px rgba(0, 0, 0, 0.15); border-radius: 4px; margin-bottom: 20px;">

### Software Development Intern

Dec 2022 - Mar 2023

Tech Stack: *Python, Flask, MongoDB, Redis, Hugging Face, scikit-learn*

**Textify AI App Platform (Initial Phase)**

1. Built API endpoints to implement app-specific request queueing using SSE (Server-Sent Events) & Redis

2. Deployed 24 GB GPT-J model with 6 billion parameters on an AWS EC2 instance for classifying complaints

3. Implemented basic CI/ CD pipelines using GitHub Actions for deploying backend APIs.

<img  src="../assets/img/dev_textify_biz_login.png"  alt="dev_textify_biz_login"  style="max-width: 100%; height: auto;">

**Client project & demos**

1. Built multiple demos for client projects spanning Text summarisation, Translation & Question answering.

2. Prepared technical documentation covering model workflows, APIs, and integration details.

3. Deployed machine learning models as production-ready APIs for client applications.

<img  src="../assets/img/complaint_classif_ss.jpg"  alt="complaint_classif_ss"  style="max-width: 100%; height: auto; box-shadow: 0 4px 16px rgba(0, 0, 0, 0.15); border-radius: 4px; margin-bottom: 20px;">

----