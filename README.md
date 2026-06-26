# Nemo Guardrails Demo

This repository contains an interactive **Jupyter Notebook demo** for building a progressively guarded Enterprise IT Assistant using `Nemo Guardrails`, `LangChain`, and related tooling.

**What I built:** A progressively guarded Enterprise IT Assistant — starting from a raw, unprotected LLM, and adding layer after layer of safety rails.

The notebook is designed to show how to:

- start with a raw LLM baseline and expose the problem without protection
- add input and output guardrails to protect the assistant
- layer jailbreak shields, sensitive-topic blockers, dialog control, and custom Python actions
- experiment with conversation flows, PII detection, and response sanitization
- integrate `Nemo Guardrails` into a notebook-driven prompt workflow

## Experiments and Concepts

| Experiment  | What I Built               | New Concept              |
| ----------- | -------------------------- | ------------------------ |
| 🔴 Baseline | Raw LLM, no protection     | The problem              |
| 🟡 Exp 2    | Topic restriction rail     | Input guardrails, CoLang |
| 🟡 Exp 3    | + Jailbreak shield         | Intent classification    |
| 🟡 Exp 4    | + Sensitive topic blocking | Multi-rail stacking      |
| 🟢 Exp 5    | + Dialog control           | Conversation flows       |
| 🟢 Exp 6    | + Custom Python actions    | PII detection, urgency   |
| 🟢 Exp 7    | + Output rail              | Response sanitization    |

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Tools and Technologies](#tools-and-technologies)

## Introduction

This demo uses `guardrails.ipynb` to demonstrate how to build a simple LLM safety and orchestration prototype with Nemo Guardrails.

It is notebook-first and intended for interactive experimentation with:

- guardrail enforcement for prompt sanitization and response filtering
- integration with LangChain for structured prompt workflows
- provider-agnostic model calls via a unified interface
- local environment configuration using `.env`

## Features

- **Guardrail enforcement** with `Nemo Guardrails` to prevent unwanted or unsafe responses
- **Interactive notebook demo** for step-by-step experiments in `guardrails.ipynb`
- **LangChain support** for chaining prompts and building simple agent flow

## Installation

1. Clone the repository:

```bash
git clone https://github.com/srijosh/Nemo-Guardrails-Demo.git
```

2. Navigate to the project directory:

```bash
cd Nemo-Guardrails-Demo
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Set up environment variables by creating a `.env` file from `.env.sample`.

## Usage

Open the notebook and run the cells sequentially:

```bash
jupyter notebook guardrails.ipynb
```

## Tools and Technologies

- **Nemo Guardrails**: safety and policy enforcement for LLM outputs
- **LangChain**: prompt orchestration and workflow construction
- **python-dotenv**: environment variable loading from `.env`
- **Jupyter Notebook**: interactive experimentation and demo execution
