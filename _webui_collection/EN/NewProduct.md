---
title: How do I add a new product?
layout: default
tags:
  - Master Data
  - Product
lang: en
sequence: 10
ref: newproduct
---

## Steps
1. Open "Product" from the [menu](Menu).
1. [Add a new product](New_Record_Window).
1. Give the product a **Name**.
 >**Note:** This name will appear in documents such as sales order confirmations etc.

1. Choose a [**Product Category**](NewProductCategory).
 >**Note:** The product category can be used to control discounts, account assignments and attribute sets of products.

1. Choose a **Product Type**.
1. Choose a **UOM** for the product.
 >**Note:** This UOM is used for *inventory management* and ***must not be confused*** with the sales UOM defined when [adding a price](ProductPrice)!

## Next Steps
- [Record a purchase or sales price](ProductPrice).
- Configure the product for manufacturing.

## Further Information
- The field **UOM** (unit of measurement) specifies the unit in which the product is managed in stock (stock-keeping UOM).
 >**Note 1:** Once the first receipt is issued with this product, the stock-keeping UOM cannot be easily changed.<br><br>
 >**Note 2:** You can define a different sales UOM isolated from the stock-keeping UOM under the record tab "Price". In this case, you also have to define a [UOM conversion](Convert_UOMs).

- The field **Product Type** specifies the type of product.

  | Option | Meaning |
  | :--- | :--- |
  | Item | Material product, e.g., piece goods, packaging, etc. (default) |
  | Service | Immaterial product |
  | Expense type | Controls the account assignment |
  | Resource | Product that can temporally only be accounted for once, e.g., a machine |

- The checkbox **Stocked** specifies whether the product is in stock (provided the product type is set on "Item").
- The checkbox **Purchased** specifies whether the product is available in purchasing.
- The checkbox **Sold** specifies whether the product is available in sales.

## Example
<kbd><img src="assets/NewProduct.gif" alt="GIF: Add new product"></kbd>
