# Architecture & System Explanation

## Overview
This system includes a deployed serverless API endpoint that receives quiz evaluation requests. The endpoint was created using the Lovable platform and deployed automatically to Supabase Edge Functions. It processes input data and returns structured JSON responses.

## Flow Diagram (simple textual format)
User request → API endpoint → Supabase Edge Function → Logic execution → JSON response returned

## How It Works
1. A POST request is sent to the Supabase Edge Function endpoint.
2. The function receives the payload and processes the quiz task.
3. The logic processes the input using predefined evaluation rules or LLM interaction.
4. A result is constructed and returned as JSON.

## Endpoint URL
https://qbzjakjzpkqkdodnwcxq.supabase.co/functions/v1/quiz

pgsql
Copy code

## Why Supabase + Lovable
- Easy deployment of serverless functions
- No need to manage servers or backend infrastructure
- Rapid development environment
- Automatically generates HTTPS endpoint

## Notes
This repository does not contain the implementation code, as the logic was built visually in Lovable and deployed directly to Supabase. This repo serves as architecture and documentation for evaluation as required by the assignment.
