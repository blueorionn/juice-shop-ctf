# View Basket

## Objective

View another user's shopping basket.

## Solution

Investigate what information is being sent to the server when the `“View Basket”` link is clicked. The URL `/rest/basket/1` seems to be fetching the basket information in JSON format. Hmm, maybe the number `1` is associated with `user ID` or something. Change the value of `1` to any other number to check if we can fetch other users' basket data.

![View Basket Data](img/view-basket.png)

We are successfully able to fetch other users' basket data.

![Challenge Solved](img/view-basket-solved.png)
