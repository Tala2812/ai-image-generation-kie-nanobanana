# AI Image Generation via Kie.ai API (Nano Banana / PRO / Nano Banana 2)

Production-ready Python functions for AI image generation and editing via Kie.ai API.

Designed for real-world integrations: Telegram bots, automation workflows and external platforms.

---
![Python](https://img.shields.io/badge/Python-3.11-blue)
![AI](https://img.shields.io/badge/AI-Image%20Generation-purple)
![Kie.ai](https://img.shields.io/badge/API-Kie.ai-green)
![Automation](https://img.shields.io/badge/Automation-Workflows-orange)
---

## 📌 Overview

This case demonstrates the development of Python functions for working with Kie.ai image models:

* Nano Banana
* Nano Banana PRO
* Nano Banana 2

The implemented solutions support both image generation and image editing scenarios and are designed for integration into real-world products.

---

## 🚀 Key Features

- Unified interface for image generation and editing  
- Support for Nano Banana / PRO / Nano Banana 2  
- Asynchronous task polling with timeout control  
- Strict parameter validation (including tool-based rules)  
- Structured and predictable API responses  
- Production-ready architecture for integrations  

---


## 🎯 Task

The goal was to create reusable and production-ready functions for AI image generation and editing via API, with:

* clear parameter validation
* safe API key handling
* asynchronous task polling
* predictable response structure
* compatibility with platform-specific requirements

---

## 💡 Solution

A set of Python functions was developed to interact with Kie.ai models through task-based API requests.

The implementation covers:

* text-to-image generation
* image editing workflows
* prompt handling
* polling until task completion
* structured error handling
* usage calculation and reporting

---

## ⚙️ Implemented Features

### Nano Banana

* text-to-image generation
* prompt preprocessing
* support for different output settings

### Nano Banana PRO

* improved generation quality
* enhanced control over output behavior
* support for advanced image generation scenarios

### Nano Banana 2

* `image_generation` mode
* `image_edit` mode
* input validation depending on tool type
* support for image URLs in editing mode
* polling with configurable intervals and timeout
* robust API response parsing
* structured success / error responses

---

## 🧠 Architectural Highlights

* all imports are placed inside the function for platform compatibility
* all inputs are passed through a single `arguments: dict` interface
* no temporary local file storage
* safe handling of secrets via environment variables
* usage block is returned in a standardized format
* error handling is designed to fail gracefully

---

## ✅ Production-Ready Aspects

* strict validation of required parameters
* enum validation for tool modes and options
* safe JSON parsing of API responses
* timeout-aware polling logic
* support for asynchronous task processing
* compatibility with external platforms and bot integrations

---

## 🔒 Integration Notes

The functions are designed to be easily integrated into:

* Telegram bots
* AI automation tools
* external SaaS or marketplace platforms
* internal business workflows

They are especially suitable for environments with strict packaging and runtime requirements.

---

## 🛠 Tech Stack

* Python
* REST API / `requests`
* Kie.ai API
* JSON response parsing
* polling / async-style task waiting

---

## 🚀 Use Cases

* image generation bots
* image editing assistants
* AI content production workflows
* automated creative tools
* multimodal user scenarios

---

## 💬 Result

The project resulted in a flexible and scalable integration layer for AI image generation and editing.

---

## 💎 Why this matters

This project demonstrates practical experience in building real AI integrations:

- working with external AI APIs  
- handling asynchronous processing  
- designing reusable function interfaces  
- ensuring production-level reliability  

It reflects the ability to turn raw AI capabilities into structured and usable solutions.

---

## 💡 Example Usage

```python
arguments = {
    "prompt": "A cinematic sunset over mountains",
    "tool": "image_generation",
    "aspect_ratio": "16:9",
    "resolution": "2K",
    "output_format": "png"
}

result = nanobanana2_function_call_new(arguments)
print(result)
```

It helps transform raw API capabilities into structured, reusable functions that are ready to be embedded into real products.
