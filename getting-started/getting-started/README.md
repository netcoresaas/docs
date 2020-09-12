# Getting started

## 1. Generate a project

Go to the [project generator page](https://netcoresaas.com/generator), configure and download your project.

## 2. Open in VSCode

Drag the folder into VSCode

## 3. Install

Open the terminal:

```text
cd ClientApp
npm i
```

## 4. Debug

Run ".NET Core Launch \(web\)" debug configuration

Open localhost:8080

## 5. Login as Admin

If you configured a valid database \(for development\) you shouldn't get any error when you login with your admin user.

## 6. Configure Products \(Stripe products/subscriptions\)

Open [localhost:8080/admin/products](http://localhost:8080/admin/products), click "Go to pricing page" and configure your prices by modifying the file: **src/store/modules/pricing/default-pricing.Development.ts**

Once you like the [localhost:8080/pricing](http://localhost:8080/pricing) page, go to [localhost:8080/admin/products](http://localhost:8080/admin/products) and click "_Click here to generate these prices in Database and Stripe_".

## 7. Register new Tenant

The admin user is not a tenant, and it's the only user who has access to /admin pages.

Try to register with another email and ensure you get the Welcome/Verification email.

## 8. Create an Expense

Navigate to [http://localhost:8080/app/expenses](http://localhost:8080/app/expenses) and add, edit and delete an expense.

## 9. Start building your own entities

Take the example of [http://localhost:8080/app/expenses](http://localhost:8080/app/expenses) and [http://localhost:8080/app/expenses2](http://localhost:8080/app/expenses2) to see how you can create a simple CRUD.



\*\*\*\*



