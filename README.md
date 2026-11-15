# AI Support Copilot

An AI-powered customer support copilot demonstrating tool use, multi-step investigation, and human-in-the-loop decision-making to streamline customer service workflows while keeping critical actions under human control.

## Project Overview

This project simulates an AI-assisted customer support environment for an e-commerce company.

Support agents can review incoming customer tickets, investigate order histories, retrieve relevant support policies, and receive AI-generated recommendations for resolving customer issues.

The application uses Claude's tool-calling capabilities to interact with mock business data and assist with multi-step investigations. Proposed actions require explicit human review and approval before execution.

The goal is to demonstrate how AI can integrate with existing business systems to streamline operational workflows without removing human oversight.

## Project Objectives

- Integrate an LLM with an application through an API.
- Implement AI tool use (function calling) for accessing business data.
- Build a multi-step investigation workflow.
- Stream AI activity and tool execution status to the frontend.
- Implement human-in-the-loop approval for proposed actions.
- Validate AI-generated recommendations against backend business rules.
- Handle errors, unexpected inputs, and prompt injection attempts.

## Technology Stack

| Category        | Technology                         |
| --------------- | ---------------------------------- |
| Frontend        | React, TypeScript, Vite            |
| Backend         | Node.js, Express, TypeScript       |
| AI Integration  | Anthropic TypeScript SDK           |
| Styling         | SCSS                               |
| Communication   | REST API, Server-Sent Events (SSE) |
| Testing         | Vitest                             |
| Code Quality    | ESLint, Prettier                   |
| Version Control | Git, GitHub                        |

## Prerequisites

- Node.js (LTS)
- npm
- Git
- Anthropic API account and API key
- Anthropic API credits

### Anthropic API Requirements

This project uses the official Anthropic TypeScript SDK to communicate with Claude.

**Important:** An Anthropic Claude subscription (including Pro) does not include API usage credits. API access is billed separately through the Anthropic Console.

To use the AI functionality:

1. Create an account in the [Anthropic Console](https://platform.claude.com/).
2. Purchase API credits.
3. Generate an API key.
4. Configure the key in your local environment.

The API key must remain server-side and must never be committed to version control.

## Development Milestones

- [ ] **Milestone 1: Project Foundation**
  - [ ] Initialize client and server structure
  - [ ] Configure TypeScript
  - [ ] Configure ESLint and Prettier
  - [ ] Configure development scripts

- [ ] **Milestone 2: Mock Business Data**
  - [ ] Create sample customer support tickets
  - [ ] Create mock order records
  - [ ] Create refund and replacement policy data

- [ ] **Milestone 3: Backend API**
  - [ ] Implement ticket retrieval
  - [ ] Implement order lookup
  - [ ] Implement policy retrieval
  - [ ] Add request validation and error handling

- [ ] **Milestone 4: AI Integration**
  - [ ] Integrate Anthropic SDK
  - [ ] Define Claude tools
  - [ ] Implement tool-calling workflow
  - [ ] Validate proposed actions against business rules

- [ ] **Milestone 5: Frontend Experience**
  - [ ] Build support ticket inbox
  - [ ] Build investigation activity panel
  - [ ] Display retrieved order and policy information
  - [ ] Display AI-generated recommendations

- [ ] **Milestone 6: Human-in-the-Loop Workflow**
  - [ ] Implement refund/replacement proposal card
  - [ ] Display drafted customer response
  - [ ] Implement edit and approval actions
  - [ ] Simulate approved actions

- [ ] **Milestone 7: Testing and Hardening**
  - [ ] Test missing and invalid order references
  - [ ] Test policy violations
  - [ ] Test invalid AI tool arguments
  - [ ] Test prompt injection attempts
  - [ ] Test API and model failures
  - [ ] Review security and error handling

- [ ] **Milestone 8: Documentation**
  - [ ] Add application screenshots
  - [ ] Document application architecture
  - [ ] Finalize setup instructions
  - [ ] Document known limitations

## Getting Started

Installation and configuration instructions will be added as the project develops.

## Application Architecture

Architecture documentation and diagrams will be added as the application takes shape.

## Screenshots

Screenshots will be added once the application UI is implemented.

## Project Scope and Limitations

This is a demonstration project using fictional customer data and mock business systems.

- No real payment processing.
- No actual customer emails or external communications.
- No production customer database.
- Refunds and replacements are simulated.
- Human approval is required before any proposed action is executed.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
