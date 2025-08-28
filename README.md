# Handy Prompts

A curated set of useful, ready-to-use prompts for a variety of AI models and productivity tools.

## Overview

Handy Prompts provides a growing library of prompts designed to help you get the most out of AI tools. Whether you need prompts for content creation, coding help, brainstorming, or automation, you'll find examples here.

## Contents

- Prompts for chatbots and language models
- Coding and debugging prompts
- Productivity and automation prompts
- Creative writing and brainstorming prompts
- Custom prompt templates

## Using YAML for Prompt Libraries
Handy Prompts is organized around YAML (.yml) files for storing and managing all Large Language Model (LLM) prompts. Each prompt lives in its own YAML file—so you can easily access, edit, version, and reuse them. This approach supports modern AI workflows, robust version control, and GitHub collaboration.

### Why YAML?
- Human-readable: YAML uses simple key-value pairs and indentation, making prompts straightforward to read and edit, even for beginners.
- Structured & Modular: Prompts, metadata (name, description, tags), parameters, and examples are grouped under logical parent keys. This keeps large prompt libraries organized and scalable.
- Collaboration: Handy Prompts uses standard YAML schemas for all prompts (name, description, model, messages, tags), enabling safe and predictable team contributions.
- Version control: YAML files are tracked like code using Git, making branching, reviews, and history seamless.
- Automation-ready: YAML is natively supported in leading AI frameworks and GitHub Actions, allowing prompts to be parsed, validated, and deployed automatically.
- Validation: Editors such as Visual Studio Code and Notepad++ offer built-in YAML linting to catch syntax errors before you commit changes.

### Best Practices
- Store each prompt in its own .prompt.yml file inside the /prompts/ folder.
- Use spaces (never tabs) for indentation.
- Standardize key names and schemas across all prompt files.
- Validate YAML syntax before committing changes.
- Document and link your YAML prompt files in this README to aid discoverability.
- Use pull requests and helpful commit messages for collaborative updates.

## Usage

Browse the /prompts/ directory to discover, copy, adapt, or contribute prompts for your LLM workflows. 

## Contributing

We welcome new prompts and improvements! Please fork the repo, create or edit .prompt.yml files, and submit a pull request. Check YAML formatting guidelines for reference.

## License

This project is licensed under the GNU General Public License. See the [LICENSE](./LICENSE) file for details.

## Contact

Questions or suggestions? Reach out to [benhanesdell](https://github.com/benhanesdell).