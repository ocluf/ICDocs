---
description: >-
  This page explains how to use the built-in canister called CandidUI to
  interact with your canisters.
---

# CandidUI

In the previous section you deployed your first canister and called a function on it through the command line. Calling a function which just takes a single `Text` value as argument might be fine, but it quickly gets bothersome as your arguments get more complex.

Luckily `dfx deploy` automatically deploys a canister called `CandidUI` that enables you to call functions easily from your browser. To use Candid UI follow these steps:

First we need to lookup the canisterID of Candid UI. Run the following command:

```
dfx canister id __Candid_UI
```

This should give you an id similar to something like: `r7inp-6aaaa-aaaaa-aaabq-cai`

Now go to the following URL in your browser replacing `CANDID-UI-CANISTER-IDENTIFIER` with the id you just got in the terminal.&#x20;

```
http://127.0.0.1:8000/?canisterId=CANDID-UI-CANISTER-IDENTIFIER
```

This should show a very basic user interface with a text input field for a canister id. We want to fill in the canister id of our hello canister here. To find this id run the command:

```
dfx canister id hello
```

And copy-paste the id to the text field. You should now see the `greet` function and be able to call it with your own input or let Candid UI call it for you with random values.\
\
