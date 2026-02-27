# Yieldblox Incident Remediation

This is a simple repo to publicly note what has been done after the incident with the Blend Pool managed by the Yielblox DAO.

## The event

On Feb 22nd at 00:25:00 UTC, a price manipulation attack was executed against the Yieldblox V2 Pool in the Blend protocol.
This event was reported by multiple parties, including both [Script3](https://x.com/script3official/status/2025403423840141450) and [Reflector's](https://x.com/in_reflector/status/2025700358626877576) teams.

## Our message

Later that day, we posted on [X](https://x.com/xBullCorp/status/2025750411429241017) an update about how that event had affected our tokenized vaults and thus their liquid staking assets: \$bUSDC and \$bEURC.

In that message, we mentioned that we were going to take care of the loss and users will not experience any loss.

## Our actions

Our first action was done that same day; we froze both vaults because we saw that many liquidity providers hadn't updated their positions to target the new minting/burning rate.

Then, during the night of Feb 25th, we upgraded both vaults and we deposited enough funds in (transactions: [\$bEURC](898bc03e9415a26199dbca21f95fcb9128ee7f815e9046c2d9d18885db203058) and [\$bUSDC](https://stellar.expert/explorer/public/tx/d7a52c72ce20251b73f94e4ccf0c8d7b16a491dc4d909e91523e0e3dcc4d40be)) to make the minting/burning rate go back to the value we mentioned in our message (as if nothing had happened). At that point, both vaults were still frozen.

## YieldBlox V2's pool remediation efforts

On Feb 27th, the Script3 team published this [repo](https://github.com/script3/yieldblox-incident-remediation). They were coordinating the remediation efforts for users, and they refunded every implementation that was affected.

The admin of the vaults received the refund ([this](https://stellar.expert/explorer/public/tx/946c119ec1bc12899e0e268c8092308e53570a13934f66076e713d2f49475adb), [this](https://stellar.expert/explorer/public/tx/4d2ceca029f2ca7353125b512e95e0a798f2c5b122c9c2d37eb8a9431b944ba3) and [this](https://stellar.expert/explorer/public/tx/42cf690c93a0807513d4631fa0fc50da00ea9982fa681aefb6ef6b79d195f107)). After receiving the refund, we deposited the difference between what we had deposited and what we just received ([here](https://stellar.expert/explorer/public/tx/9dcd48df7a4fece2562d476537a0b73cc5b6c101b2d2dde5c24b32bd93d496bc) and [here](https://stellar.expert/explorer/public/tx/23875dc3d8e91634a9c0fd0e004a4db99b1955b76d703f4059b560d07cc40bbf)).

## Wrap up

As of today, Feb 27th, users of both vaults are fully compensated, and everything is as if nothing had ever happened. We donated the funds to restore the rate on both vaults before it was refunded by Scrip3, but all the merit should be given to the Script3 team because they coordinated a remediation for users.

It's also important to make it clear that we won't cover any future losses because the tokenized vaults are designed to just represent positions in something else, so if that goes down in value, then the tokenized vault's value will go down too. Users need to think about whether they are ok with that risk or not.
