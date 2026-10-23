# GenLayer Content Verifier

An Intelligent Contract built on **GenLayer** that performs automated web content verification using decentralized AI consensus.

## Overview
This project leverages GenLayer's ability to directly process natural language and access web data on-chain. It checks whether a specified Web page contains required keywords or promotional topics without relying on traditional centralized oracles.

## Features
- **On-Chain AI Web Scraping**: Evaluates external URLs directly using GenLayer's `gl.exec_prompt`.
- **Automated Verification**: Returns consensus-based boolean results for community tasks/content quests.
- **State Tracking**: Keeps track of total verified submissions on-chain.

## Contract Architecture
- `contract.py`: Main Intelligent Contract written in Python.
  - `verify_url_keyword(url, target_keyword)`: Evaluates web content against a prompt condition.
  - `get_stats()`: View function to query total verified count and latest URL.

## Tech Stack
- **Blockchain Network**: GenLayer Bradbury Testnet
- **Language**: Python (GenLayer SDK)
