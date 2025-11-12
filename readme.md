# TDD Agent Plugin

The Vilosia TDD Agent is a ClaudeCode-based Software Development Tool for the complete dev cycle, from User Story Breakdown to Implementation Code. What's special is the **Test-Driven Development (TDD) methodology**, which results in high-quality and tested code from day one.

---

## ✨ Features

* **Full Code Scan:** Full context awareness (Architectural Structure & Patterns, Frontend/Backend Frameworks, etc.).
* **Implementation Planning:** Story Breakdown and automated Test Case generation.
* **Full Dev Cycle:** Complete journey from User Story breakdown to automated test generation.
* **Spec Driven Development:** Detailed, technical implementation with a clear definition of the feature's goal, Integrations & Dependencies, Success Criteria & Known Gotchas/Anti-Patterns.
* **Autonomous Code Generation:** Red-Green-Refactor Cycle until tests are successful.
* **Human-Readable Testcases:** Maintainable test cases in JSON format.
* **Your Environment:** IDE Plugin.

---

## Installation

```bash
/plugin marketplace add vilosia-ai/claude-plugin-marketplace
/plugin install vilosia-tdd-agent
````

> **Attention:** Restart Claude to access the new Slash Commands.

-----

## Usage

  * `/init` - Starts the code & repo scan.
  * `/storybreakdown/"userstory"` - Automatic decomposition into implementable features.
  * `/createtestcases/"feature_name"` - Creates `feature_name-test.md` with JSON Input/Output and test descriptions.
  * `/generate_spec/"feature_name"` - Creates a detailed, technical implementation guide that serves as the basis for automated code generation.
  * `/execute_spec/"feature_name"` - Initiates the self-regulating red-green-refactor cycle.

-----

## Example Workflow

See the video on our Landing Page: [https://www.tdd-agent.vilosia.com](https://www.tdd-agent.vilosia.com)

A typical workflow looks like this:

```
-> /init
  ->/storybreakdown/"userstory"
      -> /createtestcases/"feature_name"
          -> /generate_spec/"feature_name"
              -> /execute_spec/"feature_name"
```

-----

## Requirements

  * Claude Code CLI

-----

## License

This project is licensed under the MIT License.

-----

## Want to learn more?

  * **Website:** [https://www.tdd-agent.vilosia.com](https://www.tdd-agent.vilosia.com)
  * **Workshops:** Contact us on LinkedIn for a workshop which includes onboarding, agent adoption to your workflow, dev environment and architecture.
  * **Do you have Questions or want to give Feedback?** Feel free to jump into our Discord server. https://discord.gg/nHwbpKgt