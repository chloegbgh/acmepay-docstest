# Concepts

AcmePay uses a small set of core concepts. Learn these first.

### Workspace

A workspace is your main account boundary.

It contains your settings, users, docs, and API configuration.

Use it to separate teams, environments, or business units.

### Customers

A customer represents the person or business you charge.

Store customer details once. Reuse them across payments and reporting.

### Payments

A payment is a single attempt to collect money.

Payments move through a lifecycle such as `pending`, `succeeded`, or `failed`.

Treat each payment as an auditable record. Do not overwrite its history.

### Payouts

A payout moves settled funds to your bank account.

Payments and payouts are related, but they are not the same object.

One payout can include many successful payments.

### Environments

Use separate environments for testing and live traffic.

Keep your sandbox data isolated from production data.

Never reuse live credentials in test flows.

### API credentials

Every API request must be authenticated.

Use the right credentials for the right environment.

See [API authentication](../developer-guide/api-authentication.md) for setup details.

### Webhooks

Webhooks notify your system when an event happens.

Use them for asynchronous updates such as payment confirmation or payout completion.

Design webhook handlers to be idempotent.

### Access control

Control what users can manage with roles and permissions.

Use roles for internal access.

Use audience rules when you need targeted visibility in docs.

* See [User roles](../admin-guide/user-roles.md).
* See [Audience permissions](../admin-guide/audience-permissions.md).

{% hint style="info" %}
Start with concepts, then move to [Quickstart](quickstart.md) to set up your first flow.
{% endhint %}
