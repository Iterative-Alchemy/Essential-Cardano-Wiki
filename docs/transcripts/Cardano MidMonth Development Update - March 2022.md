# Cardano MidMonth Development Update - March 2022

[00:00:00] Hello, and welcome to another mid-month development update, where we bring you the very latest news on Cardona development. Joining me today are Nigel, Kevin and John. But before we dive in, make sure you like subscribe and hit that bell to get the very latest alerts on what's happening. Now, February was a major release.

[00:00:20] John, perhaps you want to tell us what was in it and why? It was foundational for our June hard fork where we have some really exciting things coming in. I've touched on them before, uh, things like improvements for Plutus and. So just to recap on what we had in 1 34, this foundational release, we had node optimizations, Ram optimizations, computational optimizations.

[00:00:41] We had a new CDL format. We had a CLI tool to be able to, uh, figure out, uh, exact script costs, which has really helped devs. And we indeed had the new leadership schedule tool. So you could find that exactly when you're slipping. Um, and I'm happy to say we received quite a bit of feedback from the community.

[00:00:57] Um, and the slot leader schedule tool has been received a massive positive feedback, and indeed, um, the built-in calculator for cost seems to actually be more accurate than some of the third-party alternatives out there. So I think we've done a good job there. I'm excited for what's coming up. And Kevin, of course, since that node upgrade, we've pushed out another one, perhaps you can tell us about, so we've pushed out a node version, 1 34 0.1.

[00:01:20] We were so proud of the mentor tracing feature that we'd introduced, uh, that we enabled it by default for all our users. Uh, but it just turned out that actually some people didn't want mentor tracing. So we've released a new version of the node that has disabled. That by default, it gives these the option of choosing whether or not, or not to use our, this great new feature.

[00:01:43] And it also includes some additional node metrics that the SPS are wanted that were missing in the 1 34 0 release. So it's a solid improvement. It's got all the features or the benefits of node version month 34.0, just these two small changes. And we recommend that staple operators are upgrade to this version.

[00:02:06] And Nigel, of course only just out of the February release, but already the work has become for June. Hasn't it. Could you tell us more about that? I think a lot of work has been done already for the June, June hard fork. We're now getting to the point where we're code complete and we think, well, that's miles away.

[00:02:21] So what happens next? Well, we've got a hell of a lot of testing to be done, integration, testing, and QA testing, component testing. And then the next stage for us is to move into a public test. Now. Where we can then get our community members to help us test that release. And it's great because we've got a good selection of different, uh, duct developers and ducts are out there that can actually help us test and make sure that we are delivered on the benefits that we're expecting for the June home.

[00:02:53] Following that as we approach may we then get involved with our exchanges and there's a lot of other work that goes on with them to make sure that they're ready as well as are all of our other downstream company. And also before June, John we'll also be looking at further parameter changes to improve the performance of the network.

[00:03:11] One on horizon. I believe maybe we can just quickly recap on some of the things we've done already this year in terms of changing network parameters. So we've taken the block size from 64 kilobytes all the way up to 80 kilobytes, and that's a twenty-five percent. And on the Plutus side for our smart contracts, we've given 40% more memory resources.

[00:03:29] So used to be 10 million units and now 14 million units. And let's not forget as well as at a transaction level where we have limits around how much resources a Plutus transaction, a smart contract can use in memory and CPU. We also have block level limits. So it's important that we scale the block level.

[00:03:46] So that the transaction level increases we've already provided. We get the biggest bang for the book there. So we want to make sure that we expand the block level limits too. So we've already taken them from 50 million memory units for the block to 56. And I suspect in this coming epoch, we're going to post an update to take that to 60.

[00:04:03] We had wanted to do this earlier, but we released the node and we wanted to give that time to bed end to make sure everything was running optimally before we made any changes. Again, we're being cautious with these changes, but ultimately we are hitting an average of a change every three weeks. Um, so that's, you know, for a network as, I guess, as sophisticated as Cardinal, which has a global uptime approaching a hundred.

[00:04:26] You know, we, we have to be careful around rolling out these changes, but I think we're doing so with a relatively aggressive cadence. And just to remind folks, you're going to see not only these changes we've done in these parameters, block size, block level, memory units, and transaction level memory units, but you're going to see other changes coming out.

[00:04:41] We're going to potentially look at. Not only increasing block size further, but look at, uh, maybe how big a transaction is allowed to be, how many CPU units are available to Plutus other economic parameters that we've discussed with the SPS. So there's a whole bunch of different things. We're going to be tweaking and we're going to get the platform to a place where we feel it's operating at an optimal level.

[00:05:01] And finally a reminder of why we're doing this stuff. Okay. We're doing it to scale the platform so that it has the bandwidth to contend with the demand that's placed upon it. So we want the credenza platform to scale in time with demand that it's seen. And these changes that we've put in up to this point in the year, and indeed the changes we're going to be making, uh, for the rest of the year and even into next year will allow us to, um, to grow out scalable.

[00:05:28] Uh, aggressively. And also when we add things like pipelining and layoffs or input endorsers on top, uh, it gives us even more scope to make further changes. So I think I'm feeling quite confident about scaling this out, to grow with demand. And of course that demand is indeed growing. Make sure you check out some of our recent infographics around all the projects building on Cardona.

[00:05:47] We've got one. 500 projects now building all the way from NFT marketplaces to, to Oracles, to liquidity solutions. So make sure you check out the latest and have a look at a central Cardona repo, which tries to map the entire ecosystem. Now, Kevin, 1.35 is the next node in the series. Oh, 1 35 follows up on the many new features.

[00:06:10] Uh, that we've introduced in 1 34, uh, by progressing a number of under the hood improvements that are going to be essential for the vassal hard-fought, but which are also essential to enable the parameter updates that John mentioned earlier. And we're keeping a very close eye on the performance of the node so that we still have plenty of headroom at rollout things like block size increases, et cetera.

[00:06:36] We're also hoping that we might be able to include some new features are that will help. Uh SBOs so keep your eyes peeled for that. But as I said before, don't hold off on your upgrades for no fashion month 35. Upgrade now to 1 34 0.1 is a great release. It's a solid, uh, versus. Lots of good features, lots of things.

[00:06:59] That will be great for SPO. So do that now, now alongside, uh, these more immediate changes and of course, heading into the, uh, the June vassal hard-fought Combinator event, there's also another longer-term project, uh, the UTX. So on this storage initiative, I caught up with Jack the product manager for that to hear more.

[00:07:18] So Jack as a project manager within the core card Dano team, a lot of your focuses around the node consensus. And of course the ledger, perhaps we can start by giving our viewers a bit of an overview of what the UTX HD project is. So the UTX O H D initiative is a complex project that is focusing on taking large parts of the ledger state from being kept in memory.

[00:07:42] To a non-US solution. The Cardona node keeps its legislative transactions within bolt-on memory. And as car continues to scale and grow with users and transactions, uh, the maintainability and sustainability of the ledger state is, is very important. And so to do this, it requires developing and integrating new infant structure within the ledger and the consensus layers.

[00:08:04] Uh, and this will enable large parts of the ledger states to be kept on date. So for those folks who aren't quite sure what UTX is exactly. Jack, can you explain that to us? Cardona uses unspent transaction outputs, think of a cash like model similar to Bitcoin, rather than an account-based model. Like Ethereum with smart contracts, we have developed what is known as the extended UTX.

[00:08:26] So which enables the functionality of Plutus scripts and complex arbitrary logic. Think of datums and the. And so as the network activity grows, so does the growth of UTX sows. Um, so it's important for us to focus on the resource requirements of the node and they need to remain reasonable. So that nodes running on end user systems and machines with data lists can maintain a smooth user experience as the network continues to.

[00:08:55] So that's really interesting. What's the progress been like so far? So far, we've added a new efficient data structures and these new data structures were in place as a version one dot 33. These new data structures change how we compact share serialize and de serialized data and how we store UTX sows.

[00:09:14] And these changes will reduce memory usage and make data structure. More efficient for storage and transport over the network. The implementation of the new data structures has actually given us about 40% savings in memory in a running node. And we've also included RTS. In version four.eight.zero. And these RTS flags are really for those low spec users, folks who have less than 16 gigs of Ram on their machine.

[00:09:40] So users who download the latest version of data lists will notice a splash page asking if they would like to enable these RTS flags for a smoother, more efficient user experience. An example of these improvements are improvements in chain replay, sync process, a full sync and stopping the cardiac.

[00:09:58] Great. Now, what does the first release entail? So the initial implementation is our MVP and on this storage component that we will include that has an in-memory backend via feature flag. And this enables users with enough memory to keep the entire UTX. So set in memory for better performance. And this is critical for state pool operators because they are on the critical path of lock propagates.

[00:10:22] It's important because we need them to mint validate and send blocks to their peers as quickly as possible. So in turn, those peers can extend the chain upon the previously minted block that they received in terms of SPO usage. A performance advantage is always received from running on the fastest possible storage mechanism.

[00:10:41] And in this case that's Ram. And what can we expect from the full release? So the engineering team is currently focused on the. But a more performance iteration of that is also, uh, to be expected very soon. This enhanced version of Utex OHD will transition away from using LM DB and move to a completely bespoke lock structure, merged tree LSM trees are one of the most performing data structures for use by applications like the Cardona node, uh, where we have a blockchain that demands a large number of.

[00:11:13] And so, um, LSM trees are data structures that are also widely used for right optimized key value stores. So this is really important. You can take Bitcoin as an example, Bitcoin uses LSM trees as the main mechanism of storing its UTX sows. And what are some of the benefits of that tree structure? So append only writes a cheap snapshotting mechanism, a cheap rollback mechanism and efficient Manoir will update operation.

[00:11:38] Our team anticipates the initial release of UTX OHD within quarter two of this year and the full spec release in the latter half of 2022. I also want to give a huge shout out to our engineering team, the consensus ledger, benchmarking QA teams. Everyone's been doing a tremendous job getting this across the line, and we're super excited to getting this out to the public.

[00:12:01] So, uh, just a huge shout out to the, all the incredible work that they're doing right now. So, thank you very much, Jack for that update. So we're nearly done for this month. Remember to join us on the last Thursday of this month for car Darnold 360. Uh, we're going to play out now just to hear some updates from some of the projects building on Cardone.

[00:12:24] So this has been a while since you were last on, give the community a quick refresher on who you are and what your. So my name's Calvin, I'm one of the co-founders of ADA handle. I have my partner, uh, and other co-founder Mr. Goose on here as well. Um, and just a quick summary of what a handle is, is where a unique, um, naming and identity solution for car Dano.

[00:12:46] So each handle is issued as an NFL. And that takes the place of like a complicated address house. And while we are genome sealed, it's a Cardinal based different platform that combines an order book decks with an AI powered liquidity management system. Um, we believe that that's the first, uh, such solution in the industry.

[00:13:05] Um, Has it been built from the ground up to combine decks and liquidity management system? Uh, our mission is to simplify and democratize defy for everyone. The platform unlocks both advanced algorithmic trading strategies and yelled optimization opportunities in a very straightforward and a hustle freeway.

[00:13:25] Um, long I'm one of the co-founder and the lead engineer I may swap. I may swap is a community focused, decentralized, extra, and on Canada. And you can go there to buy and sell your favorite. Okay. So my name is Joss I'm one of the co-founders of and we're a subscription management company. What that means is that we want to help our users manage seasonality for all of their subscription products.

[00:13:50] So primarily services like Netflix, Spotify, HBO. Uh, what do we do is we create virtual debit cards, one free subscription that they have, and we enable them to subscribe control and pay with crypto from when we last spoke, how things been going and what are some milestones that you've ticked off? Since the last time we were on building with Cardona, we were able to launch our beta sale, uh, which was a massive success for our platform.

[00:14:15] Since then, we've moved on to making optimizations and improvements, uh, for our main net launch. Uh, we were also able to secure funding through catalyst during fund seven, which was a huge success for us. It showed us that, you know, we have the community support that we were vying for. Um, it also showed positive growth towards the adoption of our new naming standard.

[00:14:33] And lastly, we were able to see the handle standard adopted, um, and used in a few of interfaces from dApps that have launched. Recently. We have a few more that we haven't announced yet, and we have a ton more partnerships with depths that just haven't launched yet, but it's definitely exciting to see, you know, more and more dabs utilize the new standard.

[00:14:50] Um, my drug that is that our ASPO turned out to be, um, an amazing. All our four pools are already situated and due to a huge interest expressed by our community. Uh, we currently discuss how we could address it. All I can confirm is that the different options are on the table. So, um, stay tuned. Secondly, we released our genius decks, a white paper, and this is what our community has been waiting for a long time.

[00:15:15] Currently we'll prepare a series of educational explanatory, videos, and articles to sort of translate. Technical terminology, uh, into simpler language and last but not least, we launched our unique accelerator program. Genius X, uh, GeniusX provides early stage gardener based startups with basically everything they need to get attraction and scale, not only by connecting them to investors, but also by supporting creation of fundraising strategies.

[00:15:46] Um, by offering legal support and so on. And of course these startups will be also integrated into the junior sealed ecosystem. We launched our Testnet. We started our audit and complete the audit we'll launch a liquidity bootstrapping event. Polio this month and we launched our net. Yes, we had quite a few milestones.

[00:16:07] The biggest one is, uh, reaching 350 K users for our mobile app. Um, the second one is creating 55,000, uh, native mobile wallets that we've created. Our specialty is really keeping everything mobile. The friendly. And the third is that our staking center is live. So you have the opportunity to stay in farm, which offer quite interesting and competitive yields.

[00:16:34] So we would invite anyone. Who's interested to check those out. So what do you have going on at the moment and where is your project headed next? So right now our main net is running. Uh, so that means that you can go to eight handled.com and meant to handle at any time you want, obviously, assuming that it's.

[00:16:49] And that's kind of like just where things are at right now in terms of our, our, uh, platform, uh, things that we're working on in terms of high priority. It's one, as goose said, we got our fund seven funding that was specifically for wallet, authentication, support, and open sourcing that software for the community to use.

[00:17:08] So. Definitely a high priority on our list. Next one is going to be smart contract minting. So converting our centralized infrastructure to actually utilize in mint handles via smart contracts. And then we're also just doing some additional research on cross chain support with protocols like ergo, um, and then also eventually converting to.

[00:17:27] So currently priority for genus sale is of course the launch of the genius decks in Q2 2022, uh, lately we signed an agreement with a smart contract security that. To run a third-party smart contract complete. Also we are in the process of intense internal tests and are gearing up for a public Testnet launch.

[00:17:49] Another priority for us is a genius academy and it's an educational and mentorship platform that teaches different concepts and helps to make a better informed decision. And basically achieve financial freedom, publishing articles, videos, podcasts for beginners, intermediate users, and also crypto experts.

[00:18:12] Uh, you, the shorter we launch, you found me on March 14th and we are going to release our SP in April so that other developers can build tools and other stuff to interact with me subjects. And in a longer term, we will start building. Let me stop the IO and community governance, and we will release with a more optimized and decentralized smart contract.

[00:18:37] So it's a very active research and development phase for us. Uh, we're preparing for a really big push in this coming quarter. We'll have quite a few updates. The biggest one is really getting our FinTech part, uh, live. So we'll be having an active license from a year old. Um, nation that we'll be able to passport for Eurozone.

[00:18:58] So we will be issuing virtual debit cards. We also have some interesting defy, uh, related, uh, surprises for our community, which we're not allowed to announce quite yet, but it will all be alive by the end of June this year. We'll see you next time.

