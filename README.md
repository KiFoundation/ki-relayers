<p align="right">
    <img width=150px src="https://wallet-testnet.blockchain.ki/static/img/icons/ki-chain.png" />
</p>

# Ki Relayers

Dear KiChain Relayer Operators! Welcome to the KiChain! We are glad to have you all onboard!

This shared repository summarizes, in one place, all the technical aspects related to relaying the KiChain and connecting it to the Cosmos ecosystem. We would be very grateful if you continuously contribute to complete and update it when relevant.

**💡 Please do not create new channels before coordinating with the Ki Team [on discord](https://discord.gg/TGJbmKmc4E). Tag Tarek#5747🙏**

# Operators
## Shared Resources
Relayer operators can share their active relayer data by adding them to the `operators/inventory.json` file:
- Fork and clone this repository
- Add your relayer data following the format of the `operators/inventory.json` file.
- Commit and push to your branch
- Create a PR to this repository.    

Merged entries can be viewed in this [spreadsheet](https://docs.google.com/spreadsheets/d/1LxC5eFiudNIVRTalh1Ltu_XWYANq8rUPCBgiWEOeBn0/edit?usp=sharing). The spreadsheet is generated automatically. Please do not try to make changes in it directly.   

## Announcements and relayer discussions  
Please make sure to join the dedicated relayer channel [`#relayers-mainnet`](https://discord.gg/ppFE45EW) on our discord server. Operators who have provided their discord handle in the inventory file will be assigned the relayer role and given write access to the channel.

# Channels
## Currently connected chains

| Channel | Source | Destination | Counterpart | Opened by | Official |
| --- | --- | --- | --- | --- | --- |
| channel-0 | KiChain | Osmosis | channel-77 | Ki team | Yes |
| channel-1 | KiChain | Cosmos Hub | channel-223 | Ki team | Yes |
| channel-7 | KiChain | Sifchain | channel-40 | -- | No |
| channel-8 | KiChain | Juno | channel-58 | Ki team | Yes |
| channel-10 | KiChain | Omniflix | channel-9 | Omniflix Team | No |
| channel-11 | KiChain | Gravity-Bridge | channel-37 | -- | -- |


## Client configurations:

| Channel | trusting_period | unbonding_period | max_clock_drift | Gas source | Gas destination |
| --- | --- | --- | --- | --- | --- |
| channel-0  | 864000s | 1209600s | 2090s | 0.025uxki | 0.0000uosmo |
| channel-1 | 1209600s | 1814400s | 2090s | 0.025uxki | 0.0025uatom |
| channel-7 | 1209600s | 1209600s | 38s | 0.025uxki | 2000rowan |
| channel-8 | 1728000s |  2419200s | 1800s | 0.025uxki | 0.0025ujuno |
| channel-10 | 1209600s | 1814400s | 20s | 0.025uxki | 0.001uflix |
| channel-11 | 1209600s | 1814400s | 20s | 0.025uxki | 0 ugraviton |


## Node configurations

| Channel | Pruning keep recent | Pruning keep every | Pruning interval |
| --- | --- | --- | --- |
| KiChain | 362880 | 0 | 100 |
| Cosmos Hub | 362880 | 0 | 100 |
| Osmosis | 362880 | 0 | 100 |
| Juno | 420000 | 0 | 100 |
