# GET STARTED
##### Inception by M2Tech - [Online playgroumd](https://inception.m2tec.nl/)
##### [tADA Faucet](https://docs.cardano.org/cardano-testnets/tools/faucet) - Once per 24hrs
##### [Examples from Gamechanger Repo](https://github.com/GameChangerFinance/gamechanger.wallet/tree/main/examples)
##### [Gamechanger Wallet - Old Website](https://gamechangerfinance.github.io/gamechanger.wallet/)
##### [Gamechanger Finance](https://gamechanger.finance)

- Navigate to `gamechanger.finance`
  - OPTIONAL `https://beta-preprod-wallet.gamechanger.finance/`
- In upper right-hand corner select `TRY BETA V2`
- At pop-up click arrows 3 times, then click `I Agree`
- At bottom left select Cardano Pre-Production Website
- On left menu select `Discover` then scroll to `Advanced`  then select `Workspaces`
  - [Current Direct Link](https://beta-wallet.gamechanger.finance/discover/advanced/workspaces)
- Select `Change Current Workspace` if there are none showing
- Then select `Add`
- Now select which official workspaces you would like and the number:
  - Hierarchical Deterministic
  - Anonymous
  - Multi Delegation
  - Anonymous Multi Delegation (autoset to 10x)
- Select `Apply`
- Select `Continue`
- Select `Continue`
- Select `Continue`
- Click `Advanced`
- Select `Code` and Copy
- 


## NOTES:
- can convert Express Wallet into Gift Wallet
  - Express -> advanced -> Gift
- test wallet: addr_test1qqdqa3hy0rdny0hyvl7cp99x2tqj3tuwxlm79zzma2n7skddqwj2u3djrag0mene2cm9elu5mdqmcz9zc2rzgq7c5g6qhaenlv 

- <img width="497" alt="image" src="https://github.com/user-attachments/assets/0297278a-8d39-48d6-b12e-3ff98a13dc7c" />


## Workspaces:
- multi-sig, multi-delegation



4 continues
after password error - as above
click go back
---

click artificats
select export
`forbidden`
select save
`forbidden`
Advanced
- full code

Return data
- select Default at top of page ->  MyFirstWallet / Default / Main Address
Select option
- Anonymous Multidelegation to 10 pools
Select Home (note: main address not yet used - yellow lettering)
- click Main Address at top
  - shows all multisig delegation wallets
  - select a wallet, click 'x' to close
  - click on Home on left menu
TO CHANGE WORKSPACE Click 2nd item from left on the Header path
Select workspace of choice
Click "x"


```
{
  "title": "Save wallet settings",
  "description": "Save on-chain on your default encrypted wallet settings GCFS DiskNFT. Settings can be derived child keys, built child addresses and others, all these inside different wallet workspaces. Workspaces are virtual groups of artifacts that allow users to have a specialized wallet experience like multi-delegation, multisig, or transact more anonymously.",
  "type": "script",
  "exportAs": "data",
  "isolateCache": true,
  "run": {
    "configuration": {
      "type": "saveConfig",
      "layers": [
        {
          "type": "Workspace",
          "items": [
            {
              "namePattern": "gc_hd_0",
              "titlePattern": "Hierarchical Deterministic",
              "descriptionPattern": "Access to your Yoroi, Daedalus or Eternl (HD wallets) child receiving (external) addresses"
            },
            {
              "namePattern": "gc_anons_0",
              "titlePattern": "Anonymous",
              "descriptionPattern": "Pure Enterprise child addresses, without staking rights, there is nothing in common between them. Don't combine with other workspaces to increase anonymity."
            },
            {
              "namePattern": "gc_anonpoolsHW",
              "titlePattern": "Anonymous Multi Delegation",
              "descriptionPattern": "Different spend and stake credentials, each address can be delegated to a different stake pool. Anonymous because there is nothing in common between them (opposite to HD wallets). Don't combine with other workspaces to increase anonymity. Compatible with hardware wallets"
            }
          ]
        },
        {
          "type": "Key",
          "items": [
            {
              "accountIndex": 0,
              "addressIndex": 0,
              "namePattern": "gc_spend_0_0",
              "kind": "spend",
              "workspaceIds": [
                "gc_hd_0",
                "gc_anons_0",
                "gc_anonpoolsHW"
              ]
            },
            {
              "accountIndex": 0,
              "addressIndex": 0,
              "namePattern": "gc_stake_0_0",
              "kind": "stake",
              "workspaceIds": [
                "gc_hd_0",
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_spend_1_0",
              "kind": "spend",
              "accountIndex": 1,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_stake_1_0",
              "kind": "stake",
              "accountIndex": 1,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_spend_2_0",
              "kind": "spend",
              "accountIndex": 2,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_stake_2_0",
              "kind": "stake",
              "accountIndex": 2,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_spend_3_0",
              "kind": "spend",
              "accountIndex": 3,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_stake_3_0",
              "kind": "stake",
              "accountIndex": 3,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_spend_4_0",
              "kind": "spend",
              "accountIndex": 4,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_stake_4_0",
              "kind": "stake",
              "accountIndex": 4,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_spend_5_0",
              "kind": "spend",
              "accountIndex": 5,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_stake_5_0",
              "kind": "stake",
              "accountIndex": 5,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_spend_6_0",
              "kind": "spend",
              "accountIndex": 6,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_stake_6_0",
              "kind": "stake",
              "accountIndex": 6,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_spend_7_0",
              "kind": "spend",
              "accountIndex": 7,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_stake_7_0",
              "kind": "stake",
              "accountIndex": 7,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_spend_8_0",
              "kind": "spend",
              "accountIndex": 8,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_stake_8_0",
              "kind": "stake",
              "accountIndex": 8,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_spend_9_0",
              "kind": "spend",
              "accountIndex": 9,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_stake_9_0",
              "kind": "stake",
              "accountIndex": 9,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            }
          ]
        },
        {
          "type": "Address",
          "items": [
            {
              "namePattern": "gc_hd_0_0",
              "spendPubKeyName": "gc_spend_0_0",
              "stakePubKeyName": "gc_stake_0_0",
              "workspaceIds": [
                "gc_hd_0"
              ]
            },
            {
              "namePattern": "gc_anon_0_0",
              "spendPubKeyName": "gc_spend_0_0",
              "workspaceIds": [
                "gc_anons_0"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_0_0",
              "spendPubKeyName": "gc_spend_0_0",
              "stakePubKeyName": "gc_stake_0_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_1_0",
              "spendPubKeyName": "gc_spend_1_0",
              "stakePubKeyName": "gc_stake_1_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_2_0",
              "spendPubKeyName": "gc_spend_2_0",
              "stakePubKeyName": "gc_stake_2_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_3_0",
              "spendPubKeyName": "gc_spend_3_0",
              "stakePubKeyName": "gc_stake_3_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_4_0",
              "spendPubKeyName": "gc_spend_4_0",
              "stakePubKeyName": "gc_stake_4_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_5_0",
              "spendPubKeyName": "gc_spend_5_0",
              "stakePubKeyName": "gc_stake_5_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_6_0",
              "spendPubKeyName": "gc_spend_6_0",
              "stakePubKeyName": "gc_stake_6_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_7_0",
              "spendPubKeyName": "gc_spend_7_0",
              "stakePubKeyName": "gc_stake_7_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_8_0",
              "spendPubKeyName": "gc_spend_8_0",
              "stakePubKeyName": "gc_stake_8_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_9_0",
              "spendPubKeyName": "gc_spend_9_0",
              "stakePubKeyName": "gc_stake_9_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            }
          ]
        }
      ]
    }
  }
}
```

Second Full Code Pull 

```
{
  "title": "Load wallet settings",
  "description": "Load this wallet settings on this device. Settings can be derived child keys, built child addresses and others, all these inside different wallet workspaces. Workspaces are virtual groups of artifacts that allow users to have a specialized wallet experience like multi-delegation, multisig, or transact more anonymously.",
  "type": "script",
  "exportAs": "data",
  "isolateCache": true,
  "run": {
    "configuration": {
      "type": "loadConfig",
      "updateId": "AccountsEditor_2025-02-18T12:07:13.558-05:00",
      "layers": [
        {
          "type": "Workspace",
          "items": [
            {
              "namePattern": "gc_hd_0",
              "titlePattern": "Hierarchical Deterministic",
              "descriptionPattern": "Access to your Yoroi, Daedalus or Eternl (HD wallets) child receiving (external) addresses"
            },
            {
              "namePattern": "gc_anons_0",
              "titlePattern": "Anonymous",
              "descriptionPattern": "Pure Enterprise child addresses, without staking rights, there is nothing in common between them. Don't combine with other workspaces to increase anonymity."
            },
            {
              "namePattern": "gc_poolsHW",
              "titlePattern": "Multi Delegation",
              "descriptionPattern": "Same spending key, different stake credential. Each address can be delegated to a different staking pool. Compatible with hardware wallets"
            },
            {
              "namePattern": "gc_anonpoolsHW",
              "titlePattern": "Anonymous Multi Delegation",
              "descriptionPattern": "Different spend and stake credentials, each address can be delegated to a different stake pool. Anonymous because there is nothing in common between them (opposite to HD wallets). Don't combine with other workspaces to increase anonymity. Compatible with hardware wallets"
            }
          ]
        },
        {
          "type": "Key",
          "items": [
            {
              "accountIndex": 0,
              "addressIndex": 0,
              "namePattern": "gc_spend_0_0",
              "kind": "spend",
              "workspaceIds": [
                "gc_hd_0",
                "gc_anons_0",
                "gc_poolsHW",
                "gc_anonpoolsHW"
              ]
            },
            {
              "accountIndex": 0,
              "addressIndex": 0,
              "namePattern": "gc_stake_0_0",
              "kind": "stake",
              "workspaceIds": [
                "gc_hd_0",
                "gc_poolsHW",
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_spend_1_0",
              "kind": "spend",
              "accountIndex": 1,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_stake_1_0",
              "kind": "stake",
              "accountIndex": 1,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_spend_2_0",
              "kind": "spend",
              "accountIndex": 2,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_stake_2_0",
              "kind": "stake",
              "accountIndex": 2,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_spend_3_0",
              "kind": "spend",
              "accountIndex": 3,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_stake_3_0",
              "kind": "stake",
              "accountIndex": 3,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_spend_4_0",
              "kind": "spend",
              "accountIndex": 4,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_stake_4_0",
              "kind": "stake",
              "accountIndex": 4,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_spend_5_0",
              "kind": "spend",
              "accountIndex": 5,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_stake_5_0",
              "kind": "stake",
              "accountIndex": 5,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_spend_6_0",
              "kind": "spend",
              "accountIndex": 6,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_stake_6_0",
              "kind": "stake",
              "accountIndex": 6,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_spend_7_0",
              "kind": "spend",
              "accountIndex": 7,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_stake_7_0",
              "kind": "stake",
              "accountIndex": 7,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_spend_8_0",
              "kind": "spend",
              "accountIndex": 8,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_stake_8_0",
              "kind": "stake",
              "accountIndex": 8,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_spend_9_0",
              "kind": "spend",
              "accountIndex": 9,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "addressIndex": 0,
              "namePattern": "gc_stake_9_0",
              "kind": "stake",
              "accountIndex": 9,
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            }
          ]
        },
        {
          "type": "Address",
          "items": [
            {
              "namePattern": "gc_hd_0_0",
              "spendPubKeyName": "gc_spend_0_0",
              "stakePubKeyName": "gc_stake_0_0",
              "workspaceIds": [
                "gc_hd_0"
              ]
            },
            {
              "namePattern": "gc_anon_0_0",
              "spendPubKeyName": "gc_spend_0_0",
              "workspaceIds": [
                "gc_anons_0"
              ]
            },
            {
              "namePattern": "gc_poolsHW_0_0",
              "spendPubKeyName": "gc_spend_0_0",
              "stakePubKeyName": "gc_stake_0_0",
              "workspaceIds": [
                "gc_poolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_0_0",
              "spendPubKeyName": "gc_spend_0_0",
              "stakePubKeyName": "gc_stake_0_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_1_0",
              "spendPubKeyName": "gc_spend_1_0",
              "stakePubKeyName": "gc_stake_1_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_2_0",
              "spendPubKeyName": "gc_spend_2_0",
              "stakePubKeyName": "gc_stake_2_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_3_0",
              "spendPubKeyName": "gc_spend_3_0",
              "stakePubKeyName": "gc_stake_3_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_4_0",
              "spendPubKeyName": "gc_spend_4_0",
              "stakePubKeyName": "gc_stake_4_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_5_0",
              "spendPubKeyName": "gc_spend_5_0",
              "stakePubKeyName": "gc_stake_5_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_6_0",
              "spendPubKeyName": "gc_spend_6_0",
              "stakePubKeyName": "gc_stake_6_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_7_0",
              "spendPubKeyName": "gc_spend_7_0",
              "stakePubKeyName": "gc_stake_7_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_8_0",
              "spendPubKeyName": "gc_spend_8_0",
              "stakePubKeyName": "gc_stake_8_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            },
            {
              "namePattern": "gc_anonpoolsHW_9_0",
              "spendPubKeyName": "gc_spend_9_0",
              "stakePubKeyName": "gc_stake_9_0",
              "workspaceIds": [
                "gc_anonpoolsHW"
              ]
            }
          ]
        }
      ]
    }
  }
}
```
