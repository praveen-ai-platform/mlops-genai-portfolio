# GenAI + Reliability Portfolio

This repository contains two small, production-minded Python projects focused on
privacy-safe observability and reliable alert operations.

## Projects

### Alert Noise Reduction POC

A FastAPI proof of concept that turns a batch of raw alerts into actionable
events. It suppresses alerts below a selected severity and deduplicates repeated
service, alert-name, and severity signatures inside a configurable cooldown.

Folder: `alert-noise-reduction-poc/`

### PII Detection and Remediation Pipeline

A privacy-aware log-processing pipeline that detects PII entities and masks
sensitive values before the records reach observability tools.

Folder: `pii-comprehend-remediation-pipeline/`

## Technology

- Python and FastAPI
- Pydantic request validation
- Amazon Comprehend-aligned PII detection
- Alert deduplication and severity-based suppression

## Purpose

The projects demonstrate a practical reliability workflow: prevent sensitive
data from leaking through logs and reduce alert fatigue before incidents are
escalated to responders.
