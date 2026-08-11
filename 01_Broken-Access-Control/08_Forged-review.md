# Forged Review

## Objective

Post a product review as another user or edit any user's existing review.

## Solution

Post a review and investigate what information is being sent to the server.

The server fetches the review of a product from **URL** `/rest/product/2/reviews` where `2` is probably product ID.

![Reviews of Product](img/get-reviews.png)

When you post your review to that product, the application issues a **PUT** request with payload `message` and `author`.

```json
{"message":"This is a review","author":"admin@juice-sh.op"}
```

![Post Review](img/post-review.png)

Let's change the author email to check if we can forge review. You can find emails of other registered users in the [admin section](./admin-section.md).

![Forged Review](img/forged-review.png)

![Challenge Solved](img/forged-review-solved.png)
