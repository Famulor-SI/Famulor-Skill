# Milian Missions API operations

Reviewed 2026-11-27. 26 public operations. [All areas](index.md) · [Execution guide](../api-and-sdk.md)

Paths are relative to `https://app.famulor.io/api/v1`. Each operation ID is also the typed SDK method `client.api.<operationId>`. Look up its exact request contract with the bundled `find-operation.py`; CLI help reflects the installed version.

Hidden CLI operations require an interactive/browser flow or `famulor api` where appropriate; do not assume the displayed generated name is an available command.

| Operation ID / SDK method suffix | HTTP endpoint | CLI command | Purpose |
| --- | --- | --- | --- |
| `createRoutine` | `POST /routines` | `famulor create-routine` | [Create a mission](https://docs.famulor.io/api-reference/milian-missions/create-a-mission) |
| `createRoutineTestCase` | `POST /routines/{id}/tests/cases` | `famulor create-routine-test-case` | [Create a mission test case](https://docs.famulor.io/api-reference/milian-missions/create-a-mission-test-case) |
| `createRoutineVersionDraft` | `POST /routines/{id}/versions` | `famulor create-routine-version-draft` | [Save a mission draft](https://docs.famulor.io/api-reference/introduction) |
| `decideMissionApproval` | `POST /mission-approvals/{id}/decision` | `famulor decide-mission-approval` | [Approve or deny a Mission action](https://docs.famulor.io/api-reference/introduction) |
| `deleteRoutine` | `DELETE /routines/{id}` | `famulor delete-routine` | [Delete a mission](https://docs.famulor.io/api-reference/milian-missions/delete-a-mission) |
| `deleteRoutineTestCase` | `DELETE /routines/{id}/tests/cases/{caseId}` | `famulor delete-routine-test-case` | [Delete a mission test case](https://docs.famulor.io/api-reference/milian-missions/delete-a-mission-test-case) |
| `estimateRoutineTestRun` | `GET /routines/{id}/tests/estimate` | `famulor estimate-routine-test-run` | [Estimate a mission test run](https://docs.famulor.io/api-reference/milian-missions/estimate-a-mission-test-run) |
| `getRoutine` | `GET /routines/{id}` | `famulor get-routine` | [Get a mission](https://docs.famulor.io/api-reference/milian-missions/get-a-mission) |
| `getRoutineTestRun` | `GET /routines/{id}/tests/runs/{runId}` | `famulor get-routine-test-run` | [Get a mission test run](https://docs.famulor.io/api-reference/milian-missions/get-a-mission-test-run) |
| `getRoutineWebhook` | `GET /routines/{id}/webhook` | `famulor get-routine-webhook` | [Get mission webhook setup](https://docs.famulor.io/api-reference/introduction) |
| `listMissionApprovals` | `GET /mission-approvals` | `famulor list-mission-approvals` | [List Mission approvals](https://docs.famulor.io/api-reference/introduction) |
| `listMissionTemplates` | `GET /mission-templates` | `famulor list-mission-templates` | [List mission templates](https://docs.famulor.io/api-reference/milian-missions/list-mission-templates) |
| `listRoutineRuns` | `GET /routines/{id}/runs` | `famulor list-routine-runs` | [List mission runs](https://docs.famulor.io/api-reference/milian-missions/list-mission-runs) |
| `listRoutineTestCases` | `GET /routines/{id}/tests/cases` | `famulor list-routine-test-cases` | [List mission test cases](https://docs.famulor.io/api-reference/milian-missions/list-mission-test-cases) |
| `listRoutineTestRuns` | `GET /routines/{id}/tests/runs` | `famulor list-routine-test-runs` | [List mission test runs](https://docs.famulor.io/api-reference/milian-missions/list-mission-test-runs) |
| `listRoutineVersions` | `GET /routines/{id}/versions` | `famulor list-routine-versions` | [List mission versions](https://docs.famulor.io/api-reference/introduction) |
| `listRoutines` | `GET /routines` | `famulor list-routines` | [List missions](https://docs.famulor.io/api-reference/milian-missions/list-missions) |
| `pauseRoutine` | `POST /routines/{id}/pause` | `famulor pause-routine` | [Pause a mission](https://docs.famulor.io/api-reference/introduction) |
| `publishRoutineVersion` | `POST /routines/{id}/publish` | `famulor publish-routine-version` | [Publish a mission version](https://docs.famulor.io/api-reference/introduction) |
| `retryRoutineRun` | `POST /routines/{id}/runs/{runId}/retry` | `famulor retry-routine-run` | [Retry a mission run](https://docs.famulor.io/api-reference/introduction) |
| `runRoutine` | `POST /routines/{id}/run` | `famulor run-routine` | [Run a mission now](https://docs.famulor.io/api-reference/milian-missions/run-a-mission-now) |
| `setRoutineTestVerdict` | `PUT /routines/{id}/tests/runs/{runId}/results/{resultId}/verdict` | `famulor set-routine-test-verdict` | [Review a mission test result](https://docs.famulor.io/api-reference/milian-missions/review-a-mission-test-result) |
| `setRoutineWebhookSecret` | `POST /routines/{id}/webhook` | `famulor set-routine-webhook-secret` | [Set or rotate mission webhook secret](https://docs.famulor.io/api-reference/introduction) |
| `startRoutineTestRun` | `POST /routines/{id}/tests/runs` | `famulor start-routine-test-run` | [Start a mission test run](https://docs.famulor.io/api-reference/milian-missions/start-a-mission-test-run) |
| `updateRoutine` | `PATCH /routines/{id}` | `famulor update-routine` | [Update a mission](https://docs.famulor.io/api-reference/milian-missions/update-a-mission) |
| `updateRoutineTestCase` | `PATCH /routines/{id}/tests/cases/{caseId}` | `famulor update-routine-test-case` | [Update a mission test case](https://docs.famulor.io/api-reference/milian-missions/update-a-mission-test-case) |
