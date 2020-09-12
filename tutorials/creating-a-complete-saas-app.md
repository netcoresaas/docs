---
description: We'll be creating a full SaaS app.
---

# Creating a complete SaaS app

## Context

I've seen a lot of [IndieHackers](https://indiehackers.com) asking to rate their landing page so we can use NetcoreSaas to build [ratemylanding.page](http://ratemylandingpage.com)

## Idea

A developer submits a page and its current version, a reviewer can upvote, review and comment landing page versions.

## **1. Prepare Domain and Integrations**

1. Domain
   1. [Buy a domain](http://www.namecheap.com)
   2. Setup DNS with [Cloudflare](http://dash.cloudflare.com)
   3. Create [Heroku app](https://dashboard.heroku.com/new-app) and add custom domain
2. Integrations
   1. Create [Stripe](https://dashboard.stripe.com/) account
   2. Create [Postmark](https://account.postmarkapp.com/) Server
      * Prepare email templates \(Welcome, Reset password and User invitation\)
   3. [Google OAuth 2.0](https://console.developers.google.com/)

## **2. Configure Codebase** \(.NET Core + VueJS + TailwindCSS\)

1. [Configure your project and download it](https://netcoresaas.com/generator)
2. Open project in VSCode and run
   1. `dotnet restore`
   2. `cd ClientApp & npm i`
3. Debugging
   1. Run debugger with _**.NET Core Launch \(web\)**_ configuration
   2. Configure _**/pricing**_ page
   3. Login as Admin
      * Generate prices in Stripe and Database
   4. Logout and Register as user
      * Activate account with welcome email
4. [Create a GitHub](https://github.com/new) repository
5. Deploy to [Heroku](https://dashboard.heroku.com)
   1. Adding **nodejs** + **jincod/dotnetcore** buildpacks
   2. Connect to GitHub for automatic deploys
   3. Deploy master branch

## **3. Frontend: Marketing side \(In construction\)**

1. Creating a simple logo \(Namecheap\)
2. Landing page \(Home\)
3. Landing pages \(Submissions to rate\)

## **4. Frontend: App side \(In construction\)**

1. My landing pages
2. My reviews
3. My profile

## **5. Backend \(In construction\)**

**Models...**

## 

## 

