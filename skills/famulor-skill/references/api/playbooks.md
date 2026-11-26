# Playbooks API operations

Reviewed 2026-11-26. 7 public operations. [All areas](index.md) · [Execution guide](../api-and-sdk.md)

Paths are relative to `https://app.famulor.io/api/v1`. Each operation ID is also the typed SDK method `client.api.<operationId>`. Look up its exact request contract with the bundled `find-operation.py`; CLI help reflects the installed version.

Hidden CLI operations require an interactive/browser flow or `famulor api` where appropriate; do not assume the displayed generated name is an available command.

| Operation ID / SDK method suffix | HTTP endpoint | CLI command | Purpose |
| --- | --- | --- | --- |
| `activatePlaybook` | `POST /playbooks/{id}/activate` | `famulor activate-playbook` | [Activate a playbook version](https://docs.famulor.io/api-reference/playbooks/activate-a-playbook-version) |
| `archivePlaybook` | `POST /playbooks/{id}/archive` | `famulor archive-playbook` | [Archive a playbook](https://docs.famulor.io/api-reference/playbooks/archive-a-playbook) |
| `createPlaybookDraft` | `POST /playbooks` | `famulor create-playbook-draft` | [Create a playbook draft](https://docs.famulor.io/api-reference/playbooks/create-a-playbook-draft) |
| `getPlaybook` | `GET /playbooks/{id}` | `famulor get-playbook` | [Get a playbook](https://docs.famulor.io/api-reference/playbooks/get-a-playbook) |
| `listPlaybookVersions` | `GET /playbooks/{id}/versions` | `famulor list-playbook-versions` | [List playbook versions](https://docs.famulor.io/api-reference/playbooks/list-playbook-versions) |
| `listPlaybooks` | `GET /playbooks` | `famulor list-playbooks` | [List playbooks](https://docs.famulor.io/api-reference/playbooks/list-playbooks) |
| `updatePlaybookDraft` | `PATCH /playbooks/{id}` | `famulor update-playbook-draft` | [Update a playbook draft](https://docs.famulor.io/api-reference/playbooks/update-a-playbook-draft) |
