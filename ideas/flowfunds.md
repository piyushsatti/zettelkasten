# Flow Funds
> The idea behind flow funds runs on a simple premise: a wallet address's assets are secured only through a private key associated with said account. Losing access or public exposure of such a key is disastrous as people can siphon all funds using said key from the associated address.

> Current solutions like storing `seed-phrases` or using `tkey` only addresses the problem of securing your private keys but at the same time limits the amount of possibilities of blockchain technology.

> Users should be able to share a type of private keys that exposes limited assets associated with an address without affecting other aspects of the account. Such keys should be their own sandbox and should not be allowed to affect any assets other than those associated with the key. Enter `sub-key` structures.

> `sub-key` function like personal access token in GitHub in the sense that they are highly dynamic in nature. Multiple keys can be generated to point to a single asset pool or different keys can be generated to point to different assets. Asset allocation can be done like venn diagrams with intersections and unions etc.

> `sub-keys` can be managed by a simple user interface or using the `API`. All transactions are forwarded to the server along with the `sub-key` where the `transactionPolicies` are verified and if found to be 'ok', are then signed and forwarded.