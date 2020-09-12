---
description: Chat with your customers with Drift.
---

# Drift

![Drift](../../../.gitbook/assets/screen-shot-2020-08-21-at-23.28.11.png)

## Environment variables:

* [Frontend]()
  * `VUE_APP_INTEGRATIONS_CONVERSATIONS_DRIFT`

### Marketing side

Uncomment line on file `ClientApp/srs/views/marketing/Index.vue`

```text
this.$drift.show();
```

### App side

Uncomment these lines on file `ClientApp/srs/components/layouts/AppLayout.vue`

```text
 this.$drift.identify(this.$store.state.account.user.id, {
        name: this.$store.state.account.user.firstName,
        email: this.$store.state.account.user.email,
      });
this.$drift.show();
```

Example:

![](../../../.gitbook/assets/screen-shot-2020-08-21-at-23.39.52.png)



