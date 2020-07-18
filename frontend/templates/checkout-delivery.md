---
description: Checkout step nr. 1
---

# Checkout Delivery

```text
/shop/checkout/delivery

/checkout/delivery.antlers.html
```

We will ask our customer to type his delivery information.

## Tags

| Options | Description |
| :--- | :--- |
| **customer** | Will empty the first time. After submitting the first form, it will contain all needed customer information. |
| **countries** | All available countries to ship to. |
| **selected\_country** | The selected country or default country. |
| **items** | All items from the bag the customer want to buy. |

## Functionality

### Form validation

We will validate the form data and show an error in case something is wrong or missing.

### Selecting a new country to ship to

After selecting a new country, the customer will be redirected to this page again. 

This is important, in case some of his chosen products will not be available in his newly selected country.   
Changed shipping prices will become visible as well. 

### Item confirmation

We will always show what the customer did buy and what the total price will be.

