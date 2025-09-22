GitHub "Good First Issue" Notifier
An automated workflow built with n8n.io that monitors specified GitHub repositories for beginner-friendly open-source contribution opportunities and sends real-time notifications to a Telegram channel.

🎯 Problem Solved
For developers looking to start contributing to open-source, finding the right first issue can be a challenge. Manually checking dozens of repositories for issues labeled "good first issue" is time-consuming and inefficient. This project automates the entire discovery process, creating a streamlined, real-time feed of accessible contribution opportunities.

🔧 How It Works
The workflow runs on a regular schedule and executes the following steps:

Schedule Trigger: A CRON-based trigger fires the workflow at a set interval (e.g., every hour) to check for new issues.

Fetch Repository Issues: The workflow connects to the GitHub API to retrieve a list of all open issues from one or more target repositories.

Filter for "Good First Issues": It then loops through each issue, parsing the JSON data to identify and filter for only those that contain the "good first issue" label.

Format Notification: The relevant details for each matching issue (such as Title, Repository Name, and URL) are extracted and formatted into a clean, readable message using the "Edit Fields" node.

Send Telegram Alert: Finally, the formatted message is sent to a dedicated Telegram channel via the Telegram Bot API, immediately notifying subscribers of the new opportunity.

🚀 Workflow Visualization
Here is a visual representation of the workflow logic built on the n8n canvas:

🛠️ Technologies & APIs Used
Core Tool: n8n.io

APIs Integrated:

GitHub API (for fetching issues)

Telegram Bot API (for sending notifications)

Data Format: JSON

Core Concepts: Workflow Automation, API Integration, Webhooks, CRON Scheduling

⚙️ Configuration & Setup
To replicate this workflow, you will need:

An n8n instance (cloud or self-hosted).

A GitHub Personal Access Token with repo scope.

A Telegram Bot Token and a Channel/Chat ID.

The workflow .json file from this repository.

Import the JSON into your n8n canvas and update the credential placeholders in the GitHub and Telegram nodes with your own API keys.
