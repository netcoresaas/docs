---
description: Setup your preferences.
---

# Project Configuration

Go to `./Helpers/ProjectConfiguration.cs` and change your database name, and your preferences.

{% tabs %}
{% tab title="ProjectConfiguration.cs" %}
```bash
...
internal static DatabaseProvider DatabaseProvider = DatabaseProvider.PostgreSQL;
internal static MultiTenancy MultiTenancy = MultiTenancy.SingleDatabase;
internal static EmailProvider EmailProvider = EmailProvider.Postmark;
internal static string Database = "netcoresaas-demo";
...
```
{% endtab %}
{% endtabs %}

### Database Provider

* PostgreSQL
* MySQL
* _More comming soon_

### MultiTenancy

* SingleDatabase: Every tenant on the same database
* DatabasePerTenant: Each tenant has its own database \(you need a root database user to create databases\)

### Email Provider

* [SMTP](../../integrations/email/smtp.md)
* [Postmark](../../integrations/email/postmark.md)

### Database

Set main database



