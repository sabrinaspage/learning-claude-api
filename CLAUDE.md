# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Learning repo for building with the Anthropic Claude API. Contains Jupyter notebooks that progressively explore Claude's Messages API using the Python SDK.

## Setup

- Python 3.11 (Homebrew)
- Dependencies: `pip install anthropic python-dotenv`
- API key loaded from `.env` via `python-dotenv`

## Conventions

- Each notebook is numbered sequentially (e.g., `000-`, `001-`, `002-`) and builds on prior concepts
- All notebooks use the same base pattern: initialize `Anthropic()` client, define helper functions (`add_user_message`, `add_assistant_message`, `chat`), then exercise the API
- Model is set to `claude-sonnet-4-0` across all notebooks
- The `chat()` function wraps `client.messages.create()` and returns `message.content[0].text`
