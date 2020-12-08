# Getting started

## 1. Generate a project

Go to the [project generator page](https://netcoresaas.com/generator), configure and download your project.

## 2. Open .sln in Visual Studio

Open ORGANIZATION\_NAME.PRODUCT_\__NAME.sln

## 2. Open ClientApp \(frontend\) in VSCode

Drag the src/PRODUCT\_NAME/WebApi/ClientApp folder into VSCode and install packages

```text
npm i
```

## 3. Debug

Run Visual Studio configuration "PRODUCT\_NAME"

Open localhost:8080 or localhost:5000

## 4. Login as Admin

If you configured a valid database \(appSettings.Development.json\) you shouldn't get any error when you login with your admin user.

## 5. Configure Products \(Stripe products/subscriptions\)

Open [localhost:8080/admin/products](http://localhost:8080/admin/products), click "Go to pricing page" and configure your prices by modifying the file: **src/store/modules/pricing/default-pricing.Development.ts**

Once you like the [localhost:8080/pricing](http://localhost:8080/pricing) page, go to [localhost:8080/admin/products](http://localhost:8080/admin/products) and click "_Click here to generate these prices in Database and Stripe_".

## 6. Register new Tenant

The admin user is not a tenant, and it's the only user who has access to /admin pages.

Try to register with another email and ensure you get the Welcome/Verification email.

## 7. Create an Expense

Navigate to [http://localhost:8080/app/transactions](http://localhost:8080/app/transactions) and add, edit and delete an expense.

## 8. Start building your own entities

Take the example of [http://localhost:8080/app/transactions](http://localhost:8080/app/transactions) and [http://localhost:8080/app/transactions2](http://localhost:8080/app/transactions2) to see how you can create a simple CRUD.



\*\*\*\*



