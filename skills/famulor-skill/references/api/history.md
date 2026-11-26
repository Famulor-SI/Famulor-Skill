# History API operations

Reviewed 2026-11-26. 40 public operations. [All areas](index.md) · [Execution guide](../api-and-sdk.md)

Paths are relative to `https://app.famulor.io/api/v1`. Each operation ID is also the typed SDK method `client.api.<operationId>`. Look up its exact request contract with the bundled `find-operation.py`; CLI help reflects the installed version.

Hidden CLI operations require an interactive/browser flow or `famulor api` where appropriate; do not assume the displayed generated name is an available command.

| Operation ID / SDK method suffix | HTTP endpoint | CLI command | Purpose |
| --- | --- | --- | --- |
| `addHistoryComment` | `POST /history/triage/{kind}/{id}/comments` | `famulor add-history-comment` | [Add an internal note](https://docs.famulor.io/api-reference/history/add-an-internal-note) |
| `archiveHistoryCategory` | `DELETE /history/categories/{id}` | `famulor archive-history-category` | [Archive an Inbox category](https://docs.famulor.io/api-reference/history/archive-an-inbox-category) |
| `createHistoryCategories` | `POST /history/categories` | `famulor create-history-categories` | [Add Inbox categories](https://docs.famulor.io/api-reference/history/add-inbox-categories) |
| `createHistoryRoutingRule` | `POST /history/routing-rules` | `famulor create-history-routing-rule` | [Create a routing rule](https://docs.famulor.io/api-reference/history/create-a-routing-rule) |
| `createHistorySlaPolicy` | `POST /history/sla-policies` | `famulor create-history-sla-policy` | [Create an SLA policy](https://docs.famulor.io/api-reference/history/create-an-sla-policy) |
| `createHistoryView` | `POST /history/views` | `famulor create-history-view` | [Create a saved History view](https://docs.famulor.io/api-reference/history/create-a-saved-history-view) |
| `deleteHistoryRoutingRule` | `DELETE /history/routing-rules/{id}` | `famulor delete-history-routing-rule` | [Delete a routing rule](https://docs.famulor.io/api-reference/history/delete-a-routing-rule) |
| `deleteHistorySlaPolicy` | `DELETE /history/sla-policies/{id}` | `famulor delete-history-sla-policy` | [Delete an SLA policy](https://docs.famulor.io/api-reference/history/delete-an-sla-policy) |
| `deleteHistoryView` | `DELETE /history/views/{id}` | `famulor delete-history-view` | [Delete a saved History view](https://docs.famulor.io/api-reference/history/delete-a-saved-history-view) |
| `dismissInboxLabel` | `POST /history/inbox-labels/{id}/dismiss` | `famulor dismiss-inbox-label` | [Dismiss a message label](https://docs.famulor.io/api-reference/history/dismiss-a-message-label) |
| `exportHistoryRecord` | `GET /history/triage/{kind}/{id}/export` | `famulor export-history-record` | [Export a History entry as Markdown](https://docs.famulor.io/api-reference/history/export-a-history-entry-as-markdown) |
| `getBusinessHours` | `GET /business-hours` | `famulor get-business-hours` | [Get the workspace business hours](https://docs.famulor.io/api-reference/history/get-the-workspace-business-hours) |
| `getEmailHistoryItem` | `GET /history/emails/{id}` | `famulor get-email-history-item` | [Get an email conversation](https://docs.famulor.io/api-reference/history/get-an-email-conversation) |
| `getHistoryRoutingRule` | `GET /history/routing-rules/{id}` | `famulor get-history-routing-rule` | [Get a routing rule](https://docs.famulor.io/api-reference/history/get-a-routing-rule) |
| `getHistorySlaSummary` | `GET /history/sla-summary` | `famulor get-history-sla-summary` | [Get the SLA summary](https://docs.famulor.io/api-reference/history/get-the-sla-summary) |
| `getHistoryTriage` | `GET /history/triage/{kind}/{id}` | `famulor get-history-triage` | [Get triage of a History entry](https://docs.famulor.io/api-reference/history/get-triage-of-a-history-entry) |
| `getHistoryTriageSettings` | `GET /history/triage-settings` | `famulor get-history-triage-settings` | [Get Milian triage settings](https://docs.famulor.io/api-reference/history/get-milian-triage-settings) |
| `getHistoryView` | `GET /history/views/{id}` | `famulor get-history-view` | [Get a saved History view](https://docs.famulor.io/api-reference/history/get-a-saved-history-view) |
| `getInboxLabelSettings` | `GET /inbox-labels/settings` | `famulor get-inbox-label-settings` | [Get message label settings](https://docs.famulor.io/api-reference/history/get-message-label-settings) |
| `getMessagingHistoryItem` | `GET /history/messaging/{id}` | `famulor get-messaging-history-item` | [Get a messaging conversation](https://docs.famulor.io/api-reference/history/get-a-messaging-conversation) |
| `listHistory` | `GET /history` | `famulor list-history` | [List conversation history](https://docs.famulor.io/api-reference/history/list-conversation-history) |
| `listHistoryCategories` | `GET /history/categories` | `famulor list-history-categories` | [List Inbox categories](https://docs.famulor.io/api-reference/history/list-inbox-categories) |
| `listHistoryRoutingFields` | `GET /history/routing-rules/fields` | `famulor list-history-routing-fields` | [List routing fields](https://docs.famulor.io/api-reference/history/list-routing-fields) |
| `listHistoryRoutingRules` | `GET /history/routing-rules` | `famulor list-history-routing-rules` | [List routing rules](https://docs.famulor.io/api-reference/history/list-routing-rules) |
| `listHistorySlaPolicies` | `GET /history/sla-policies` | `famulor list-history-sla-policies` | [List SLA policies](https://docs.famulor.io/api-reference/history/list-sla-policies) |
| `listHistoryViews` | `GET /history/views` | `famulor list-history-views` | [List saved History views](https://docs.famulor.io/api-reference/history/list-saved-history-views) |
| `removeAssistantRoutingRules` | `DELETE /history/routing-rules` | `famulor remove-assistant-routing-rules` | [Send an assistant back to the workspace rules](https://docs.famulor.io/api-reference/history/send-an-assistant-back-to-the-workspace-rules) |
| `reorderHistoryRoutingRules` | `PUT /history/routing-rules/order` | `famulor reorder-history-routing-rules` | [Set the order of a rule set](https://docs.famulor.io/api-reference/history/set-the-order-of-a-rule-set) |
| `reorderHistorySlaPolicies` | `PUT /history/sla-policies/order` | `famulor reorder-history-sla-policies` | [Set the order of the SLA policies](https://docs.famulor.io/api-reference/history/set-the-order-of-the-sla-policies) |
| `replyToHistoryConversation` | `POST /history/reply` | `famulor reply-to-history-conversation` | [Reply to a conversation](https://docs.famulor.io/api-reference/introduction) |
| `runHistoryActions` | `POST /history/actions` | `famulor run-history-actions` | [Run history actions on any channel](https://docs.famulor.io/api-reference/history/run-history-actions-on-any-channel) |
| `testHistoryRouting` | `POST /history/routing-rules/test` | `famulor test-history-routing` | [Test routing](https://docs.famulor.io/api-reference/history/test-routing) |
| `updateBusinessHours` | `PUT /business-hours` | `famulor update-business-hours` | [Set the workspace business hours](https://docs.famulor.io/api-reference/history/set-the-workspace-business-hours) |
| `updateHistoryCategory` | `PATCH /history/categories/{id}` | `famulor update-history-category` | [Update an Inbox category](https://docs.famulor.io/api-reference/history/update-an-inbox-category) |
| `updateHistoryRoutingRule` | `PATCH /history/routing-rules/{id}` | `famulor update-history-routing-rule` | [Update a routing rule](https://docs.famulor.io/api-reference/history/update-a-routing-rule) |
| `updateHistorySlaPolicy` | `PATCH /history/sla-policies/{id}` | `famulor update-history-sla-policy` | [Update an SLA policy](https://docs.famulor.io/api-reference/history/update-an-sla-policy) |
| `updateHistoryTriage` | `PATCH /history/triage/{kind}/{id}` | `famulor update-history-triage` | [Change triage of a History entry](https://docs.famulor.io/api-reference/history/change-triage-of-a-history-entry) |
| `updateHistoryTriageSettings` | `PATCH /history/triage-settings` | `famulor update-history-triage-settings` | [Update Milian triage settings](https://docs.famulor.io/api-reference/history/update-milian-triage-settings) |
| `updateHistoryView` | `PATCH /history/views/{id}` | `famulor update-history-view` | [Update a saved History view](https://docs.famulor.io/api-reference/history/update-a-saved-history-view) |
| `updateInboxLabelSettings` | `PATCH /inbox-labels/settings` | `famulor update-inbox-label-settings` | [Update message label settings](https://docs.famulor.io/api-reference/history/update-message-label-settings) |
