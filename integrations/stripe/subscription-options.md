---
description: NetcoreSaas Demo implements out of the box these types of pricing.
---

# Subscription Options

### Subscription with Trial

![](../../.gitbook/assets/screen-shot-2020-08-22-at-18.27.31.png)

### Subscription without Trial

![](../../.gitbook/assets/screen-shot-2020-08-22-at-18.27.43.png)

### One payment

![](../../.gitbook/assets/screen-shot-2020-08-22-at-18.27.52.png)

### Customize

However you can implement your custom pricing and styles with these files:

* **Your products:**
  * ./ClientApp/src/store/modules/pricing/default-pricing.Development.ts
  * ./ClientApp/src/store/modules/pricing/default-pricing.ts
* **Styling \(yourapp.com/pricing\)**:
  * ./ClientApp/src/views/marketing/Pricing.vue
* **Models:**
  * ./ClientApp/src/app/models/pricing/Product.ts
  * ./ClientApp/src/app/models/pricing/Price.ts
  * ./Models/Administration/DTO/StripePricingDTOs.cs
* Controllers:
  * ./Controllers/Subscriptions/StripeController.cs



