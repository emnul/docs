---
title: Webhooks
description:
  Locksmith implements websub for Unlock Protocol and allows you to send real
  time updates to registered endpoints.
---

# Webhooks

Locksmith implements [Websub](https://www.w3.org/TR/websub) which allows anyone to receive real time updates from the [Unlock subgraphs]. It is a _webhook_ system which many developers will be familiar with with built-in intent verification.

Currently, locksmith support sending updates on new locks and keys. To subscribe, an application will need to send a post request to the hubs located at `/api/hooks/[topic]`. The body needs to match the schema specified in the [Websub w3c spec](https://www.w3.org/TR/websub/#x5-1-subscriber-sends-subscription-request).

For examples on using the webhooks checkout the tutorial ["Using Webhooks with the Locksmith API"](../../tutorials/back-end/locksmith-webhooks).