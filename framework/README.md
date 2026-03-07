# Framework Overview

This directory contains the local framework that supports the host multi-agent workflow.

What lives here:

- `contracts/`: JSON schemas and structure contracts
- `prompts/`: role prompt baselines for execution sessions
- `runbooks/`: operating procedures
- `validation/`: local validation boundary notes
- `visualization/`: local visualization boundary notes

Current contract coverage includes chapter-level artifacts, book-level state, checkpoint artifacts, and book-level closeout outputs.

What does not live here:

- custom LLM client code
- custom agent orchestration code
- LangGraph workflows
- OpenAI SDK wrappers

Those execution responsibilities are delegated to the host multi-agent runtime.
