# Safe use checklist for AI coding agents

This companion note is a local addition to the fork of [Codebuff's Freebuff](https://github.com/CodebuffAI/freebuff). The original project remains credited to Codebuff and its contributors. Keep the upstream Apache-2.0 LICENSE and NOTICE files intact.

## Before you run an agent on a project

- Work in a git branch or a copy, so every change can be reviewed and reverted.
- Do not run an agent in a folder that holds secrets. Keep .env files, keys and tokens out of the project, or list them in an ignore file.
- Use test data. Do not point an agent at production databases or accounts.
- Read what the agent plans to run before approving shell commands, especially deletes, installs and network calls.

## Before you accept the changes

- Read the full diff. Do not merge changes you do not understand.
- Run the project's own tests and linters yourself.
- Check any new dependency: its name, publisher, license and recent activity.
- Remember that text ads support the free models, and that prompts may be sent to the model providers. Do not paste private code or personal data you are not allowed to share.

This note does not change how Freebuff works or claim that it is safer or more accurate. AI-generated code can be wrong, so review it like any other contribution.
