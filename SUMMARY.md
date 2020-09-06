# Table of contents

* [Introduction](README.md)

## Getting Started

* [Getting started](getting-started/getting-started.md)
* [Environment variables](getting-started/environment/README.md)
  * [Backend \(.NET Core\)](getting-started/environment/backend-netcore.md)
  * [Frontend \(VueJS\)](getting-started/environment/frontend-vue.md)
  * [Project Configuration](getting-started/environment/project-configuration.md)
  * [Pricing](getting-started/environment/pricing.md)
* [Integrations](getting-started/integrations.md)
* [Debug](getting-started/debug/README.md)
  * [ClientApp](getting-started/debug/clientapp.md)
  * [Backend](getting-started/debug/backend.md)
* [Deploy](getting-started/deploy/README.md)
  * [Initialize git repository](getting-started/deploy/initialize-git.md)
  * [Publish to heroku](getting-started/deploy/publish-to-heroku.md)

## Features

* [Authentication](features/authentication.md)
* [SignalR](features/signalr.md)

## Integrations

* [Stripe](integrations/stripe/README.md)
  * [Subscription Options](integrations/stripe/subscription-options.md)
  * [Getting the API Keys](integrations/stripe/getting-the-api-keys.md)
  * [Creating Stripe Products](integrations/stripe/creating-subscriptions.md)
  * [Creating the Customer Portal](integrations/stripe/creating-your-customer-portal.md)
* [Email](integrations/email/README.md)
  * [SMTP](integrations/email/smtp.md)
  * [Postmark](integrations/email/postmark.md)
* [Social Login](integrations/social-login/README.md)
  * [Google Sign In](integrations/social-login/google.md)
* [Conversations](integrations/conversations/README.md)
  * [Intercom](integrations/conversations/intercom.md)
  * [Drift](integrations/conversations/drift.md)

## Requirements

* [Installing](requirements/installing.md)
* [1. Install VSCode](requirements/vscode.md)
* [2. Install .NET Core SDK](requirements/.net-core.md)
* [3. Install Node.js](requirements/node.js.md)
* [4. Test installation](requirements/test-installation.md)

## Project Structure <a id="structure"></a>

* [API Controllers](structure/api/README.md)
  * [Administration Controllers](structure/api/system-controllers/README.md)
    * [AdminController](structure/api/system-controllers/admincontroller.md)
    * [AuthenticationController](structure/api/system-controllers/authenticationcontroller.md)
    * [TenantController](structure/api/system-controllers/tenantcontroller.md)
    * [TenantUsersController](structure/api/system-controllers/tenantuserscontroller.md)
    * [UsersController](structure/api/system-controllers/userscontroller.md)
  * [Subscription Controllers](structure/api/subscription/README.md)
    * [StripeController](structure/api/subscription/stripecontroller.md)
    * [StripeAdminController](structure/api/subscription/stripeadmincontroller.md)
  * [Core Controllers](structure/api/core/README.md)
    * [TransactionCategoriesController](structure/api/core/transactioncategoriescontroller.md)
    * [ExpensesController](structure/api/core/expensescontroller.md)
* [Frontend](structure/frontend.md)

