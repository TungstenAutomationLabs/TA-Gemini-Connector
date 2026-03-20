# TotalAgility: Gemini LLM Connector

## Overview
This package provides a standardized, reusable Custom Service Group for integrating Google Gemini 2.0/3.0 into TotalAgility workflows.

## Package Components
- **Category:** `LLM_Connectors`
- **Custom Service Group:** `Gemini_Package`
- **Web Service:** WS_Gemini_LLM - RESTful reference to `generativelanguage.googleapis.com`

## Setup Instructions
1. **Import:** In TotalAgility, go to *Packages > Import* and upload the `.zip` file provided in this repo.
2. **Configuration:** - Navigate to **Integration > Server Variables**.
   - Update `LLM_API_Key` with your Google AI Studio / Vertex AI key.
   - Enter System Prompt in `LLM_Prompt_Template`
   - (Optional) Update `LLM_Endpoint_URL` if using a specific region or model version.
3. **Usage:**
   - In your Process or Extraction group, call the `Gemini Agent` Custom Service.
   - Pass the `Input_Document_Text` as input and receive the `Output_JSON_Result`.

## Input/Output Schema
- **Input:** `Input_Document_Text` (String)
- **Output:** `Output_JSON_Result` (String/JSON)
