---
description: Antlers is a simple and powerful templating engine provided with Statamic.
---

# Antlers Tags

If you are familiar with Statamic, you will know the Antlers template engine. This is why we do provide Antlers tags for you. 

In case you never worked with Antlers before, [read the Statamic introduction](https://statamic.dev/antlers). 

## Bag

A bag is the shopping cart in _butik_

### Items

```text
{{ bag }} // short syntax

{{ bag:items }}
```

Will return all items from the actual bag \(shopping cart\).

| Value |  |
| :--- | :--- |
| **sellable** | Is this item available in the selected country?  |
| **available\_stock** | How many are available |
| **slug** | The unique identifier of the product / variant |
| **images** | Belonging images |
| **name** | The name |
| **description** | A short descriptioin  |
| **single\_price** | The price for a single item |
| **total\_price** | The price for all items |
| **quantity** | How often is this item in the bag    |

### Total Items

```text
 {{ bag:total_items }}
```

 Counting the total amount of items in the bag.

### Total Price

```text
{{ bag:total_price }}
```

 The total amount of all items including shipping.

### Total Shipping

```text
{{ bag:total_shipping }}
```

Summing the total shipping costs for all items in the shopping bag 

## Butik

The _butik_ tag does provide the most important routes.

### Shop

```text
{{ butik:shop }}
```

Will return the shop overview route.

### Bag

```text
{{ butik:bag }}
```

Will return the route to the butik bag \(shopping cart\). 

## Categories

This tag is handy to fx create a menu for exisiting categories, wherever you need them on your page.

### Default

```text
{{ categories }}
```

This will return all existing categories with the following information: 

| Values | Description |
| :--- | :--- |
| **name** | Category name |
| **slug** | Category slug |
| **url** | Category url |

### Count

```text
{{ categories:count }}
```

Will return the total number of created categories

### Example: Create categories menu

```markup
{{ if {categories:count} > 0 }}
    <a href="{{ butik:shop }}">Overview</a>
    {{ categories }}
        <a href="{{ url }}">{{ name }}</a>
    {{ /categories }}
{{ /if }}
```

## Currency

Get currency information from your shop

### Symbol

```markup
{{ currency }} // short syntax

{{ currency:symbol }}
```

Will return the currency symbol

### Name

```markup
{{ currency:name }}
```

Will return the currency name

### Iso

```markup
{{ currency:iso }}
```

Will return the currency iso code

### Delimiter

```markup
{{ currency:delimiter }}
```

Will return the currency delimiter.  

## Products

### Products

```markup
{{ products }}
```

Will return all existing products

