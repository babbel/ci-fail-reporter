# CI Fail Reporter
Github Action to report default branch CI fails to the slack channel.

## Overview
The **CI fail Reporter** is a GitHub Action designed to report to Slack when CI fails on the main (or another default) branch.

## Inputs

### `slack_webhook_url`
- **Description**: The Slack webhook URL where notifications will be sent.
- **Required**: Yes

## Usage
In your CI workflow add the following line
```
- name: Report to Slack
    uses: babbel/ci-fail-reporter@1.0.0
        with:
          slack_webhook_url: ${{ secrets.slack_webhook_url }}
```
