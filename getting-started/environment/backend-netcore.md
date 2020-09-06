# Backend \(.NET Core\)

Create or download these 2 files at the root directory and update your environment variables.

Rename **`YourAppName`**

{% file src="../../.gitbook/assets/appsettings.json" caption="appsettings.Development.json" %}

{% file src="../../.gitbook/assets/appsettings.development.json" caption="appsettings.json" %}

{% tabs %}
{% tab title="./appsettings.Development.json" %}
```bash
{
  "App": {
    "Name": "YourAppName",
    "URL": "http://localhost:8080",
    "SupportEmail": "support@yourappname.com",
    "LiveChatURL": "help.yourappname.com",
    "DocsURL": "docs.yourappname.com",
    "CompanyName": "",
    "CompanyAddress": ""
  },
  "Logging": {
    "LogLevel": {
      "Default": "Debug",
      "System": "Information",
      "Microsoft": "Information"
    }
  },
  "Jwt": {
    "Key": "MUSTBEA16CHARACT",
    "Issuer": "TEST"
  },
  "ConnectionStrings": {
    "DbContext_PostgreSQL": "User ID=;Server=localhost;Port=5432;Database=[DATABASE];Pooling=true;Password=;",
    "DbContext_MySQL": "Server=localhost;Port=3306;Database=[DATABASE];Uid=root;Pwd=;"
  },
  "Stripe": {
    "PublishableKey": "",
    "SecretKey": ""
  },
  "SecretSignInKey": "RANDOMSECRETKEY",
  "EmailSettings": {
    "SmtpMailServer": "smtp.gmail.com",
    "SmtpMailPort": 587,
    "SmtpSenderName": "YourAppName",
    "SmtpSenderEmail": "no-reply@yourappname.com",
    "SmtpPassword": "",
    "PostmarkSenderName": "YourAppName",
    "PostmarkSenderEmail": "noreply-demo@yourappname.com",
    "PostmarkServerToken": ""
  }
}
```
{% endtab %}

{% tab title="./appsettings.json" %}
```bash
{
  "App": {
    "Name": "YourAppName",
    "URL": "http://demo.yourappname.com",
    "SupportEmail": "support@yourappname.com",
    "LiveChatURL": "help.yourappname.com",
    "DocsURL": "docs.yourappname.com",
    "CompanyName": "",
    "CompanyAddress": ""
  },
  "Logging": {
    "LogLevel": {
      "Default": "Debug"
    }
  },
  "Jwt": {
    "Key": "MUSTBEA16CHARACT",
    "Issuer": "TEST"
  },
  "ConnectionStrings": {
    "DbContext_PostgreSQL": "User ID=;Server=;Port=5432;Database=[DATABASE];Pooling=true;Password=;",
    "DbContext_MySQL": "Server=;Port=3306;Database=[DATABASE];Uid=;Pwd=;"
  },
  "Stripe": {
    "PublishableKey": "",
    "SecretKey": ""
  },
  "SecretSignInKey": "RANDOMSECRETKEY",
  "EmailSettings": {
    "SmtpMailServer": "smtp.gmail.com",
    "SmtpMailPort": 587,
    "SmtpSenderName": "YourAppName",
    "SmtpSenderEmail": "no-reply@yourappname.com",
    "SmtpPassword": "",
    "PostmarkSenderName": "YourAppName",
    "PostmarkSenderEmail": "noreply-demo@yourappname.com",
    "PostmarkServerToken": ""
  }
}
```
{% endtab %}
{% endtabs %}

