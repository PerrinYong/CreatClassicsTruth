# Validation Boundary

Local validation code in this project should only cover:

- JSON schema validation
- required field checks
- enum checks
- naming and directory checks
- cross-file structural checks that do not require LLM reasoning

It should not implement agent logic or model calling.
