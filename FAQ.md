## What is AdEx? 
[AdEx](https://www.adex.network/) originated in 2017 as a decentralized ad exchange for digital advertising, and subsequently evolved into a full protocol for decentralized digital advertising.

The AdEx protocol facilitates trading of advertising space/time, as well as the subsequent verification and proof that it actually occurred. Essentially, it covers all interactions between publishers, advertisers and end users. The protocol combines traditional peer-to-peer technology, cryptography and blockchain.

## What problems does AdEx solve? 
AdEx addresses some of the most prominent inefficiencies of the contemporary advertising landscape: ad fraud, unclear and misleading campaign reporting, exuberant fees, many middlemen and compromised end user privacy. 

## How does AdEx compare to BAT? 
The Basic Attention Token (BAT) aims at bringing back the souls lost to ad blockers by rewarding people who opt in to see ads in the Brave browser. We, on the other hand, are focused on improving the existing advertising marketplace and let advertisers and publishers transact with each other, while respecting the end users’ privacy. 

## What can I use AdEx for? 
The AdEx protocol is intended mainly for display advertising, however its use is not limited to that. It can be applied to a number of different use cases - for example influencer marketing; content micropayments; affiliate marketing; product placement; and so on.

The revenue model could be CPC, CPM, CPA or time-based ad property rentals. This makes the protocol usable for physical world advertising (billboards, point-of-sale advertising, guerilla installations, etc.) as well. 

## What fees do I pay to use AdEx?
We charge absolutely no fees or commissions for using the AdEx platform/protocol. However, you may be required to pay a tiny fee for the validators that you use. 

The way the validator consensus works implies that channel validators have to represent opposite sides; if they don't, the channel should not be used. This means that at one point or another you may end up using a third-party validator. 

Running the validator stack requires computational resources and the third-party validator may require [a small fee](https://github.com/AdExNetwork/adex-protocol#validator-fees). 

## What wallets can I use to create an AdEx advertiser or publisher account? 
You can sign up for AdEx with Trezor, Ledger or Metamask. 

## What is the purpose of the ADX token
The ADX token is used for staking if you're running an [AdEx validator](https://github.com/adexnetwork/adex-protocol#validator-stack-platform). Staking your ADX will register your validator in a global registry where your visibility will be proportional to your staked amount.

The staked amount will be slashed if your validator misbehaves (i.e. an economic punishment will be applied to the misbehaving validator).

We are currently working on the specification of this, however you can [track the progress here](https://github.com/AdExNetwork/adex-protocol/issues/7).

## How can I get ADX tokens? 
If you haven’t acquired ADX tokens during our token generation campaign, you may do so at a number of exchanges such as Binance and Bittrex for example. 

## How do you ensure campaign reporting transparency? 
The information that marketers get about their campaigns generally comes from the same source - the ad serving network - and is not objectively verifiable. This means that there is no mechanism to protect marketers and advertisers from [losses caused by bugs or even by malicious intent](https://www.nytimes.com/2016/11/17/technology/facebook-acts-to-restore-trust-after-overstating-video-views.html). 

In order to avoid this, we are introducing real-time tracking and reporting where the exact same data is easily accessible by each advertiser or publisher. The reporting data is derived directly from the users from the SDK to the publisher's validator(s) (publisher platform) and the advertiser's validator(s) (advertiser platform), and this guarantees reporting transparency.

## How do you ensure end user privacy? 
All of the information that AdEx uses for user targeting is collected through the [AdEx SDK](https://github.com/AdExNetwork/adex-protocol#sdk) into the user’s local storage. This information never leaves the device of the user, and they are able to clear it at any time.  

In the future, end users will be presented with the AdEx Lounge - a user-facing part of AdEx that will allow them to see what type of data has the SDK collected about them and modify it.  Once again, it's important to note that all of the targeting data resides in the user's browser and never get sent to anyone as an additional layer of privacy.  The end result of this is minimizing the possibility of user data/metadata sales to third parties; of exploiting information about consumer purchasing habits; etc.

## What are validators and validator stacks? 
[OCEAN](https://github.com/AdExNetwork/adex-protocol#off-chain-event-aggregation-ocean)/[OUTPACE](https://github.com/AdExNetwork/adex-protocol/blob/master/OUTPACE.md) validators are responsible for tracking ad impressions/clicks and signing the state. The validator set (can also be called a committee) is defined by the OUTPACE channel. Validators receive data from the AdEx SDK. 

A majority of validators is required in order to achieve a valid signed state. 

A [validator stack](https://github.com/AdExNetwork/adex-protocol/blob/master/components/validator-stack.md) is a collective term for all off-chain components responsible of handling events, managing OUTPACE channels and generating analytical reports.

## What are custom events? 
[Custom events](https://github.com/AdExNetwork/adex-protocol#custom-events) are events defined by the advertiser or by the publisher. For example: an advertiser who is an online retailer may wish to set a purchase of a product as a conversion goal, rather than pay for clicks or impression; setting this as a conversion is a custom event.

## What is OCEAN?
[OCEAN](https://medium.com/the-adex-blog/introducing-ocean-alternative-layer-2-scalability-7d24bb22ebe4) stands for “off-chain event aggregation”. This is a [Layer 2](https://github.com/AdExNetwork/adex-protocol#layer-2) scalability solution that helps us handle a high number of events off-chain while retaining all the benefits of a trustless consensus. 

## What is OUTPACE?
[OUTPACE](https://github.com/AdExNetwork/adex-protocol/blob/master/OUTPACE.md) is a unidirectional payment channel based on OCEAN. OUTPACE allows for creating a simple one-to-many payment channel, where each participating party can withdraw their available balance (advertising budget or ad earnings) at any time. The withdrawn amounts are accounted for on-chain.

## Does AdEx offer real-time bidding?
No. However, AdEx advertisers can take advantage of header bidding, which is quickly replacing real-time bidding anyway. 

Header bidding is the process of pulling all the bids in the browser, evaluating them and then sending the preferred bids to the ad exchange. In AdEx, there is no classic ad exchange, but what we do is even more convenient: we pull all information about demand (campaigns, bids) in the browser, and directly select the bid depending on what we know about the user, therefore implementing targeting without revealing the user's profile.

## Do you have a bug bounty? 
Yes, we do. We offer rewards for security vulnerabilities that coders discover after every major release of the AdEx dApp. [Read more about the AdEx bug bounty.](https://medium.com/the-adex-blog/announcing-the-adex-bug-bounty-a5a6e0621094)

## Where can I meet the AdEx team? 
We attend a number of various events around the world. Follow us on social media to see which conferences, meetups or hackathons we are going to (we usually announce at least a couple of weeks in advance of each event). 
