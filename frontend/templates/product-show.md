---
description: Will show a specific product
---

# Product Show



```text
/shop/{product}

/shop/show.antlers.html
/livewire/product-variant-section.blade.php
```

## Livewire

We did add a Livewire component for you, so if your customer does select a variant, it will be loaded without a reload of your page. 

This is how we do implement the livewire component

```text
{{ livewire:butik.product-variant-section :product="product" }}
```

## Tags

### Main View

| Name | Description |
| :--- | :--- |
| **product** | Will return the chosen product  |

### Livewire View

{% hint style="warning" %}
It's not possible to use Antlers inside Livewire components.
{% endhint %}

Checkout how we did write the templates. You will see, that they are nearly similar and that you can adjust the template as easy as you can with Antlers.

## Functionality

### Variant existing?

If a product has a variant, it's not allowed to visit the parents product route. 

Don't worry about, it, we will take care of it and redirect directly to a belonging variant. 

### Product unavailable?

If it is, we will redirect directly to our overview page.



