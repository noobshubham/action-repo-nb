# action-repo-nb

This is a dummy GitHub repository used to trigger GitHub webhook events for testing.

## Purpose
This repository generates the following GitHub events:
- Push
- Pull Request
- Merge (optional)

These events are sent via GitHub Webhooks to a Flask-based webhook receiver.

## Webhook Configuration
- The webhook payload URL is exposed locally using **LocalTunnel**
- Content-Type: application/json
- Events enabled: Push, Pull Request

## How to Trigger Events
- **Push**: Commit and push changes to any branch
- **Pull Request**: Create a PR between branches
- **Merge**: Merge an open PR (bonus event)

## Backend Implementation
All backend webhook handling, MongoDB storage, and UI logic are implemented in the following repository:

👉 https://github.com/noobshubham/webhook-repo-nb/tree/setup

## Notes
This repository does not contain backend logic.  
It exists only to emit GitHub events for integration testing.

# Screenshot
<img width="1889" height="650" alt="image" src="https://github.com/user-attachments/assets/ee84be7d-3fc4-44f7-ac34-e699052cf78d" />
