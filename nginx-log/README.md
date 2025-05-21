# aimiox Nginx Log Analyzer

This tool analyzes nginx access logs, extracts IP information, and generates a comprehensive markdown report with AI-powered analysis of visitor behavior.

## Features

- Parses nginx access logs to extract information
- Identifies unique IP addresses in the logs
- Fetches geolocation data for each IP
- Uses OpenAI's LLM to analyze visitor behavior and detect potential security threats
- Generates a detailed markdown report with findings

## Installation

1. Clone this repository or download the files on Ubuntu 22.04 or later

2. Copy `env.sample` to `.env` and edit with your OpenAI API key or enable other LLM providers


## Usage

Run the agent (requires Ubuntu 22.04 or later) with the path to your nginx access log file:

```bash
aimiox_nginx_log_agent access.log
```


## Output

The generated markdown report includes:

- Summary statistics
- Per-IP analysis including:
  - Geolocation information (country, ISP)
  - AI-generated summary of visitor behavior
  - Request methods used
  - HTTP status codes received
  - Potential security concerns

