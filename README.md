# Community Hub Repository

The Community Hub serves as a collaborative platform for gathering and managing community-driven contributions. Whether you're proposing new content, requesting features, reporting issues, or ideation for dApps, this repo is your entry point. We use GitHub's built-in features like issues, projects, and automations to ensure ideas are triaged efficiently and turned into actionable tasks.

Key Features:

*   Public Boards: For transparency in triage and task management.
*   Automated Workflow (coming soon): Issues are automatically added to boards and moved based on labels.
*   Inclusive Contribution: Open to all, with guidelines for high-quality submissions.

This repo is part of the `midnightntwrk` organization.

## Create an Issue

<div align="center">

[![Report a Bug](https://img.shields.io/badge/Report_a_Bug-d73a4a?style=for-the-badge&logo=openbugbounty&logoColor=white)](https://github.com/midnightntwrk/Community-Hub/issues/new?template=bug.yml)
[![Request a Feature](https://img.shields.io/badge/Request_a_Feature-58a6ff?style=for-the-badge&logo=nebula&logoColor=white)](https://github.com/midnightntwrk/Community-Hub/issues/new?template=feature-request-suggestion.yml)
[![Suggest Content](https://img.shields.io/badge/Suggest_Content-3fb950?style=for-the-badge&logo=readme&logoColor=white)](https://github.com/midnightntwrk/Community-Hub/issues/new?template=content-proposal.yml)
[![Propose a dApp](https://img.shields.io/badge/Propose_a_dApp-9e7ce3?style=for-the-badge&logo=createreactapp&logoColor=white)](https://github.com/midnightntwrk/Community-Hub/issues/new?template=dapp-proposal.yml)

</div>

## Issue Templates

To standardize submissions and make it easier for contributors, we provide the following issue templates:

*   **Content Proposal**: For suggesting new content like articles, tutorials, or resources. Use this to propose ideas that educate or engage the community.
*   **Feature Request/Suggestion**: For proposing new features, enhancements, or suggestions to improve existing tools or processes.
*   **Bug**: For reporting defects, errors, or unexpected behavior. Include reproduction steps, environment details, and screenshots if possible.
*   **dApp Proposal**: For ideas related to decentralized applications, including concepts, integrations, or improvements for dApps in our ecosystem.

When creating an issue, select the appropriate template from the "New Issue" page. This auto-applies relevant labels (e.g., `bug`, `feature-request-suggestion`) for better categorization.

## Examples

Explore our starter kits and examples to kickstart your dApp development on Midnight.

### React Wallet Connection Starter Example

A minimal React application demonstrating how to connect to a Midnight-compatible wallet (like Lace) using the `@midnight-ntwrk/dapp-connector-api`. This example showcases:
*   Connecting/disconnecting from the wallet.
*   Displaying the connected wallet address.
*   Reading and displaying the tDUST balance.
*   Basic error handling.

This example is built with Vite/Create React App and TypeScript.

[**Get Started with the React Wallet Connection Example**](./examples/react-wallet-starter/README.md)

## Workflow

Our workflow ensures every submission is reviewed fairly and efficiently. Issues start in the Community Board for triage and, if approved, move to the Grab n Go Board for contributors to pick up. Both boards are public for transparency.

Columns (based on the "Status" field):

*   **New**: Entry point for fresh issues. Community members can view and comment.
*   **In Triage**: Active review by the triage committee (validity, priority, labels).
*   **Needs Discussion**: For issues requiring broader feedback or clarification.
*   **Rejected**: Invalid or out-of-scope issues, with explanations for transparency.

The triage committee meets periodically to review and move issues. If legitimate, they add a `triaged` label, triggering an automation to move it to the Grab n Go Board.

## Grab n Go Board

The Grab n Go Board showcases approved, ready-to-work-on tasks. It's a backlog for contributors.

Columns (based on the "Status" field):

*   **Ready**: Triaged issues awaiting pickup (e.g., labeled `good-first-issue` for beginners).
*   **In Progress**: Tasks being worked on (assign yourself and update via PRs).
*   **Done**: Completed issues (auto-moves on close).

Automations handle movement between boards and status updates for efficiency.

## Code of Conduct

We are committed to a positive, inclusive community. Please adhere to our [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).

## Contributing

We welcome contributions from everyone! Follow these steps:

*   **Fork the Repo**: Click "Fork" on the top right.
*   **Create an Issue**: Use templates to submit ideas or bugs.
*   **Work on Tasks**: Browse the Grab n Go Board, assign yourself to a "Ready" issue.
*   **Submit a Pull Request**: Want to improve Community-hub? Submit a PR and follow our [CONTRIBUTING.md](CONTRIBUTING.md) for details on code style, testing, and commits.
*   **Labels and Priorities**: Use labels like `priority:high`, `help-wanted`, or `good-first-issue` to guide contributions.

For non-code contributions (e.g., docs, proposals), submit via issues. All PRs require review by at least one maintainer.