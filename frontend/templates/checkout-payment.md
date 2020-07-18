---
description: Checkout step nr. 2
---

# Checkout Payment



```text
/shop/checkout/payment

/checkout/payment.antlers.html
```

We will show all the inserted data again. After accepting, the customer will be redirect to [Mollie](www.mollie.com) for his payment.

## Tags

| Options | Description |
| :--- | :--- |
| **customer** | Will empty the first time. After submitting the first form, it will contain all needed customer information. |
| **items** | All items from the bag the customer want to buy. |

## Functionality

### Remove non-sellable items

In case the user had some non-sellable items in his bag \(shopping cart\), because they were not available in his country, we will remove them as soon as we load this page. 

