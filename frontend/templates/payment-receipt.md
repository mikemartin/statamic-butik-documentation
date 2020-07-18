---
description: Our last checkout step.
---

# Payment Receipt

```text
/shop/payment/{order}/receipt

/checkout/receipt.antlers.html
```

Mollie will redirect to this page after the payment.

### Reloading Page

We will receive the actual payment status directly from Mollie. 

The page will be reloaded via Javascript every few seconds, to show the newest information. 

## Security

This is a signed route, which will only be valid for 5 minutes after the purchase regarding security issues. 

To make sure that nobody can do funky stuff with this information, the receipt link will invalidate itself.

## Tags

| Options | Description |
| :--- | :--- |
| **customer** | Contain customer information. |
| **order** | The order information |

