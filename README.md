# DynamicDividend
Dynamic Dividend: A smart contract-mediated participation in Ethscape’s “GDP”

THE IDEA
The basic idea for the Dynamic Dividend ("DD") is a "social dividend" rather than a Universal Basic Income, as no minimum is guaranteed.

However the original idea goes back to Thomas Paine (1795) and Georgists/Commons theorists.It has since been developed in paralell with the thinking on a Universal Basic Income and its socio-political justifications are broadly the same:
- Practical freedom means freedom from want
- Society benefits from some degree of equalisation (e.g. Alaska Permanent Fund)
- Market production benefits from existence of commons but does not internalise its cost
- Non-market production (arts, literature, research, open source software, “passion projects” etc) should increase
- “AI/robot argument”: jobs in industry and most services will disappear anyhow as result of AI and robotisation

BASIC IMPLEMENTATION
In a basic implementation, the DD smart contract would periodically rebalance all individual wallets as follows:
- By looking up each individual wallet’s balance at the end of the period;
- Then, calculating the individual dividend as a fix % (x) over the sum of all wallet balances before adjustment; 
- Finally, adjusting the dividend sent to each wallet for the individual wallet’s weight in the total wallet balance (i.a.w for how much each individual wallet contributed to Ethscape’s “GDP” before adjustment) 

The variables are:
x = Dividend rate e.g. 5%
ITx(t) = Total Individual Tx over Period
TWB(t-1) = Previous Total Wallet Balances
TWB(t) = New Total Wallet Balances: (TWB(t-1) + ∑ITx(t)
D = Dividend over Period: ∑ITx(t) * x
Individual Wallet Balance IWB(t)*
* before DD adjustment

A basic formulation would be:




Further research:
Game theoretic: e.g. incentive to reduce wallet to level where wallet becomes “subsidised”
Economic e.g. difficult to exclude non-esc holders from accessing non-scarce non-market produced goods
Technology: smart contract layer and scaling
