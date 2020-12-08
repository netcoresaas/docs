---
description: >-
  You don't need the project generator, you can directly download the Codebase
  on the /app/releases page and configure manually.
---

# Environment variables

## Backend

**Integration Tests**: tests/PRODUCT\_NAME.IntegrationTests/appSettings.Testing.json

**Development**: src/PRODUCT\_NAME.WebApi/appSettings.Development.json

**Production**: src/PRODUCT\_NAME.WebApi/appSettings.json

```text
{
  "App": {
    "Name": "PRODUCT_NAME", //
    "URL": "http://localhost:8080",
    "SupportEmail": "your@email.com",
    "LiveChatURL": "PRODUCT_NAME.com",
    "DocsURL": "PRODUCT_NAME.com",
    "CompanyName": "",
    "CompanyAddress": ""
  },
  "ProjectConfiguration": {
    "DatabaseProvider": "PostgreSQL",
    "MultiTenancy": "SingleDatabase",
    "MasterDatabase": "PRODUCT_NAME-dev",
    "EmailProvider": "Postmark",
    "SubscriptionProvider": "Stripe",
    "RequiresEmailVerification": "false"
  },
  "Jwt": {
    "Key": "pL5pFCi5Xvc2t1tD",
    "Issuer": "PRODUCT_NAME"
  },
  "ConnectionStrings": {
    "DbContext_PostgreSQL": "User ID=testing;Server=localhost;Port=5432;Pooling=true;Password=testing;Database=[DATABASE];",
    "DbContext_MySQL": "Server=localhost;Port=5432;Uid=testing;Pwd=testing;Database=[DATABASE];"
  },
  "SubscriptionSettings": {
    "PublicKey": "pk_test_...",
    "SecretKey": "sk_test_..."
  },
  "EmailSettings": {
    "SmtpMailServer": "smtp.gmail.com",
    "SmtpMailPort": "587",
    "SmtpSenderName": "PRODUCT_NAME",
    "SmtpSenderEmail": "noreply@PRODUCT_NAME.com",
    "SmtpPassword": "",
    "PostmarkServerToken": "...",
    "PostmarkSenderName": "PRODUCT_NAME",
    "PostmarkSenderEmail": "contact@PRODUCT_NAME.com"
  },
  "DefaultUsers": [
    {
      "Uuid": "e2b9a8de-2196-11eb-adc1-0242ac120002",
      "Organization": "Admin",
      "Subdomain": "admin",
      "Type": "Admin",
      "Email": "admin@gmail.com",
      "Password": "password"
    },
    {
      "Uuid": "eca8cd3b-0348-4dc7-90d9-9345b88f1f07",
      "Organization": "Tenant1",
      "Subdomain": "tenant1",
      "Type": "Tenant",
      "Email": "tenant1@gmail.com",
      "Password": "password1"
    }
  ],
  "Logging": {
    "LogLevel": {
      "Default": "Debug",
      "System": "Information",
      "Microsoft": "Information"
    }
  }
}
```

## Frontend

src/PRODUCT\_NAME.WebApi/ClientApp/.env.production

src/PRODUCT\_NAME.WebApi/ClientApp/.env.development

```text
VUE_APP_SERVER_URL=https://PRODUCT_NAME.com/
VUE_APP_API_URL=https://PRODUCT_NAME.com/api/

VUE_APP_LANGUAGE=en-US
VUE_APP_THEME=theme-bg-dark
VUE_APP_COLOR=theme-violet
VUE_APP_THEME_MARKETING_THEME=theme-bg-light
VUE_APP_THEME_MARKETING_COLOR=theme-violet

VUE_APP_GOOGLE_CLIENT_ID_OAUTH2=

VUE_APP_INTEGRATIONS_CONVERSATIONS_INTERCOM=
VUE_APP_INTEGRATIONS_CONVERSATIONS_DRIFT=
VUE_APP_INTEGRATIONS_ANALYTICS_GOOGLE=GTM-K284KTD
VUE_APP_INTEGRATIONS_ANALYTICS_MIXPANEL=
VUE_APP_INTEGRATIONS_ANALYTICS_HOTJAR=
VUE_APP_INTEGRATIONS_LOGGING_SENTRY=
VUE_APP_INTEGRATIONS_LOGGING_LOGROCKET=
VUE_APP_INTEGRATIONS_NEWSLETTER_MAILCHIMP=
VUE_APP_INTEGRATIONS_CONTACT_FORMSPREE=

VUE_APP_SOCIAL_FACEBOOK=https://facebook.com/PRODUCT_NAME
VUE_APP_SOCIAL_INSTAGRAM=https://instagram.com/PRODUCT_NAME
VUE_APP_SOCIAL_TWITTER=https://twitter.com/PRODUCT_NAME

VUE_APP_BLOG_GHOST_URL=
VUE_APP_BLOG_GHOST_CONTENT_API_KEY=

VUE_APP_SUBSCRIPTION_PUBLIC_KEY=pk_test_...
VUE_APP_SUBSCRIPTION_SECRET_KEY=sk_live_...
```

