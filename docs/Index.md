## Shippo Docs

- API REference https://goshippo.com/docs/reference#transactions
- API Docs https://docs.goshippo.com/
- Github Page https://github.com/goshippo
- API Webhooks https://docs.goshippo.com/docs/tracking/webhooks/

## Plan

worker(hook, payload);

Where:

- worker is a CF function,
- hook, is a key (URL path), regarding the logic branch,
- and payload is the param of that logic invocation

1 Get Webhook notifications of new orders somehow
2 Parse order details
3 Propagate to Zoho Inventory

## Questions:

1: How to get notified of new orders

- Shippo has a webhook api to set up hooks.
  - The available hooks are:
    - Transaction (Label purchases)
