# Cardano 360 Mid Month Development Update - April 2022

[00:00:00] **Tim Harrison:** So welcome to April's mid month development update. Now, before we start, make sure you like subscribe and hit that bell. So you can get alerted tool that I use is video content that we put out on the IHG channel. Now we'll have a regular update today, but as well as that, we've got some bonus content for you.

[00:00:16] We asked John to record a video and polluters and particularly what the vessel heartfelt will bring to the development of the platform. So that'll. A little bit later in the show. We'll also have Matthew on later talking to just some of the projects building on Cardona. This time we'll feature our Donna meld, muesli swap and ergo decks.

[00:00:33] That's all coming up later. But before all that let's have a quick check-in with a regular team. We'll almost regular team. Nigel is not here this week. He's having some well-deserved downtime before things really heat up. So John let's start with a network performance. How's it looking at the moment, Tim?

[00:00:48] It's looking really good. And I don't know whether a load has dropped or we've just made the network scale really well. But at the moment everyone's getting serviced in great time. All of the dabs are performing well and there's no backlog. So this is exactly what we want to see. And when I started looking at the metrics on the network, so I'm digging into how blocks are transiting, how long they're taking to reach 95% of the state car Dano or nodes or SPO is rather representing that.

[00:01:13] And how long blocks are taking to be adopted on today. These metrics are looking great around to 2.3 seconds. And this tells us that the network is healthy, performing well, servicing all of its users in a way that we want and ready to scale it further. So I think we're already happy with it. So Kevin, obviously a large part of this is SBOs upgrading the notes to the, to the latest version.

[00:01:33] How are we looking in terms of the network there? It's looking great. 10. So shout outs, all the SPS who are so on top of the game, what we're seeing from Hulu. Is about 69% on the latest release version month at 4.1, trench 2% on 1 33. And it's likely that the increasing adoption by the SPS is the cause for the bad performance that John has been reporting to you.

[00:01:58] We're expecting a new release soon, 1 35. We'll announce the exact date when it's ready, but there's absolutely no reason for SPS to hold off. 1 34 is absolutely the right version to be on for the time being. And looking ahead ahead of the vassal hard fork, there'll be a few changes. We're going to need operators to make to some of that scripting, just still with.

[00:02:19] Uh, tiny changes in the way the node is going to work. We'll announce that ahead of time. So nobody gets surprised by that. We'll, we'll call that out on discord, telegram, uh, et cetera. So keep an eye on that. Nothing particularly significant it's just to make sure everyone's node keeps working perfectly through the basil hard-fought and beyond.

[00:02:37] So John, the network's looking very healthy, but we're not stopping there. Are we just to quickly build on what Kevin said? We want people to be on the latest and greatest just like companies like apple and Google when they released their own. They want to make sure there's not fragmentation. If folks choose to use the latest version, they're getting the best and the network benefits as a whole, as more people adopt.

[00:02:55] So I'd encourage people to upgrade. We're not stopping there in terms of scaling of the network. So just a quick recap, we take them blocks from 64 kilobytes to 80 kilobytes. We've taken mem units from 10 million to 14 million. And most recently we took block level limits, um, to dismember units from 50 million to 62 million units.

[00:03:11] These are real materials. But coming up and, uh, I believe just signed off and we'll be posting, I think, next to the park we're taking the block sized ADA killer. So, again, this is a 10% increase in throughput on layer one. So these are real double digit increases. And I think we don't, we don't actually need it right now with the current load we're seeing and everything has been serviced well, but we're not waiting.

[00:03:34] We want, as I mentioned before, the network. As demand grows. So John, where we're looking good for the, for the vessel hard fork, um, perhaps you can just tell us a little bit about what's happening next and I believe we've got a date we can share as well. Absolutely. So just to remind people, we can make releases and we do all year round.

[00:03:52] When we have a hard fork. What we're saying there is the protocol is changing in a material way. We're leaving the old, uh, version of ledger behind and we're moving to a new version of the ledger. And this event requires all of our SBOs and all of our users to upgrade to the latest node so that they can fork together.

[00:04:08] This is an upgrade event and it's a positive thing. We only need to do this when we're making significant changes to the ledger. We've just gone code complete for all of the stuff we're bringing into June basil hard fork. The thing to remember here is it's not just hard for guidance that we're bringing.

[00:04:21] We're also bringing a slew of new features and fixes and. But alongside those things that we'd have in a normal release. Anyway, we also have these hard fork items. So just to remind folks, it's stuff like enhancements, sip 31 32 and 33 reference script, inline, datums, and reference inputs. And I've talked about this before and, and, uh, I'll talk about it again.

[00:04:44] These are things that are going to make apps sing on Cardona. And these are things that are gonna make developer experience easier and better. We're also bringing pipelining, which is our enhancement to lock diffusion, which will allow us to scale even further. And as I've mentioned before, this is going to see us right up to the point where we released input endorses, which is our next generation.

[00:05:02] So we're code complete now. And what does that mean? It means that we've actually coded or not me, the smart people who work here have actually coded all of the changes that are required for these features. So they're in get hub there, you know, the code is complete, but what we now need to do, because that's, that's of course a great milestone, but it's not the whole picture when you're releasing something that has to be as robust and secure as.

[00:05:24] So we're now moving to a really deep QA. We're going to make sure everything is perfect. We're going to make sure there's no bugs, regressions, performance, slowdowns, et cetera. As we add all this stuff, we have to make sure we're just as good as we were before we edited. So we're in that process of QA right now, we're in the process of integration testing, which means we're.

[00:05:42] Disparate parts of the system like ledger and consensus meet each other with these changes for the first time, so that they can see if they're interacting correctly, which we're not anticipating any problems with. But at the same time, it's still a lot of work we have left to do. We've also reached out and talked to our partners and exchanges to make folks aware that this is happening as an end user.

[00:05:58] You're not going to see much friction in terms of user experience. You just download the new node, you fire it up and everything will be on. But exchanges and other businesses have to prepare for this because we need them to be upgraded on time so that there's no discontinuation of their service for their customers.

[00:06:12] We're going to have a test net ahead of time to help developers and exchanges play with this stuff so that they can, they can understand they prepare for it. And ultimately, just to remind people, these cool changes we're bringing for Plutus, you need to take advantage of them actively. This is not a passive thing.

[00:06:25] So your, your apps that are currently there are not just gonna, you know, use these features automatically. If you want to use references. And to make your app lighter. You've got to do that. If you want to use reference inputs, so you can do more reading of UTX cell bodies and datums concurrently. You've got to take advantage of that yourself.

[00:06:41] These are things that we want folks to use, and we're going to have lots of information around how to take advantage of them. So people get the best experience. And then finally, just to add, we're targeting a date in June, and I don't like giving dates because in engineering, it's one of those things.

[00:06:54] Whenever you give a date, it ends up being a mess, but we're looking at June 29th and some of you guys will be probably thinking, yeah, you know, they said June, and it's now June that the last possible day. And you're right. It is. So we're just giving ourselves as much time as possible to get all of this work done, but things are looking very positive there, John, thank you very much for that.

[00:07:13] Uh, for that update. Now, John, just before we let you go, you've actually been kind enough to record a video for us. You mentioned the sips, you mentioned the Plutus improvement. Provement. We'll run that video in just a moment, but what are we going to be? I realized, you know, when we were discussing things internally that we didn't really have a one-stop shop to understand flu's a single place, folks could go and kind of get the current state of play.

[00:07:34] So what I wanted to do was bring people on a journey, a relatively short video, I think it's 15 or 20 minutes where we've just walked through the entire ecosystem of polluters. And I tried to explain it from the roots, right. I tried to bring people on the journey of how do you create. Where does it start?

[00:07:49] What is the first process file new project? And you start writing your code. I then pretty quick bring people on the journey of how we get that to the blockchain, how you interact with it. And then I finish off the video, looking at some of these enhancements that are coming up and looking at some of the great reasons why building on a UTX soul-based based system, like Dardano brings, um, concurrency, parallelization, and other good things.

[00:08:09] I think. So thank you. Uh, Jonathan, thank you, Kevin, as well for those updates. So let's run that video, but please stick around afterwards. We'll have some more updates from Matthew and some of the projects building on Caetano right after that let's play that video. Hi, I'm John Woods, director of credenza architecture at IOG.

[00:08:29] And today I'm here to tell you a little bit about Plutus. We're going to be rolling out some major changes in June to both the Cardinal platform and Plutus itself. Plutus is smart contracts. The changes we're bringing in June are going to mean huge enhancements for plutonium. And today what I wanted to do was bring it back to basics.

[00:08:50] I think many times when we're giving technical updates, we forget to give the fundamentals about how things work. And today we're going to look at the fundamentals of blues. So the content today is roughly as follows. I'm going to give some context on what food is actually is. I'm going to talk about EUT XO extended on spent transaction outputs and they are the heart of the flu.

[00:09:15] I'm going to talk about the Plutus architecture, how you interact with a Plutus script, our CIPS, our improvement proposals, and some improvements that are coming down the line. I'm going to talk about some of the virtues of Plutus determinism, parallelism, and concurrency. And then finally wrap it up with a quick conclusion.

[00:09:34] Okay. So Plutus is Cardinals smart contracts? Um, Plutus represents a range of technologies, but ultimately they empower the creation of depths or decentralized apps, apps on blockchain. They also enable NFTs non fungible tokens, which have been very popular this year. They opened up the door for a whole new range of collectibles and use cases.

[00:09:59] Blue. This is also how you launched native assets on Cardona. And what does that mean? It means your own coin, your own token, your own currency. Plutus is the gateway to launch anything you'd like in that context. And then finally Plutus. Arbitrary on chain, conditional logic. Now, what does that mean? Plutus enables effectively like Excel, if statements programmability on the Cardinal blockchain.

[00:10:26] So now let's talk about UT XO, UT XO or extended. UT XO is the difference between a standard UTX old model. And what we're achieving with Cardona EUT XO is how we do on chain programmability and smart contracts. So let's look at the components that make up EUT XO. We have the concept of a contract, a smart contract it's sometimes called a validator or a script.

[00:10:55] And you can think of this as a lock that locks up UTX, OHS, or ADA or. On the Cardinal blockchain, it can also be used to look NFTs or other native assets like your own coin that you launch. We also have the concept of a Redeemer and a Redeemer is like a key. And the key or the Redeemer in this case is the piece of data passed in by the user of the smart contract to try to unlock those funds in space.

[00:11:24] We have an item called datum and Dayton is some state that lives on the UTX output. And you can think of data as a place to store a high score or some metadata or some other data that's important to your app. Datum is kind of like the hard disk for the smartphone. And then finally we have a thing called context, which is really like metadata.

[00:11:45] You're able to inspect the transaction and say, Hey, who signed this? Um, what account is this spending to that kind of thing. So if you wrap these four items up together, This form is the heart of what we call and it turns out that is all we need to enable all classes of smart contract defy, or other web three application on Cardona.

[00:12:09] Let's talk now about the Plutus architecture. I think the Plutus architecture is really interesting and this slide walks you through the process of going from code to on chain. So we start a course with developers, developers write the source code to the DOP and all of the Plutus contracts are currently written in high school.

[00:12:32] We may support other languages in the future or allow DSLs to make things easier for certain use cases. But right now we do them in a functional programming language called Haskell. So let's look at how you start with user code and you end up with an on chain script. Well, it starts with the compiler.

[00:12:50] The Haskell code that's written by the developer is turned into a thing called Plutus Plutus I, or is an intermediate representation. And those of you who might be familiar with how things like LLVM work, we'll know this already. When you write code, of course, it goes through a pipeline in all contexts, whether that's a smart contract code that's destined for blockchain, or indeed a windows or Mac iOS or.

[00:13:14] When we get the intermediate representation, it gives us an opportunity to mold and make more efficient. The source code that was written by the developer. And this is really important because how we represent the application and machine language that's going to be executed at runtime is really important.

[00:13:32] So by taking the Haskell source code and by driving it through and number of optimizations to. Whilst it's in this intermediate representation, it yields really fast performance. From that intermediate representation, we then go to type Plutus core. Now type Plutus core is just before the roll ones and zeros that get executed on chain.

[00:13:56] So why do we have it? Well, it's a handy item for developers type Plutus core is really low level, but it still has some extra information that developers can use to. Finally, then we moved on type Plutus core, which is a Lambda calculus, variant. I'll let you Wikipedia that, but it's basically a logical way to express the app on type Plutus core gets executed on chain.

[00:14:21] So how does that on polluted core or compiled app get on chain? Well, after all those optimization stages, Scripts get on chain with toolkits and other Plutus apps. We have a whole suite of applications to help you take that compiled application and inject it on. Of course, it's really important to mention off-chain code.

[00:14:45] So even when the Ancienne code is written and has been compiled and is ready to go on chain, we still need an off-chain component. The off-chain component is the application that will correctly form transactions to interact with that. So the on chain app can be great, but we still need something that helps us build and form correct transactions that provide the inputs to that app inputs like the Redeemer and the data that we talked about in the previous.

[00:15:12] So I think this is painted really well. We start with user source code. We move through the compiler pipeline to make it as efficient as possible, taking that human code and bringing it down to the roll ones and zeros. We then end up with Plutus core scripts. We use our tools to inject that in a transaction on chain where that on chain script will be processed by our ledger.

[00:15:37] And ultimately executed and rung by the Plutus core evaluator in a decentralized. And of course, just to mention the off-chain or contract monad, as some of you developers will know is a way that you can then interact with this on chain component by forming the right transactions. So let's move on now to a Plutus interaction.

[00:15:59] So I'm drilling into how it looks when you're actually using one of these scripts. And you're a user who wants to interact with a Dex or another. So, how do you interact with the Plutus contract? I think this is an interesting one because it differs from how it works on Ethereum. And it's going to change what are upcoming updates in June.

[00:16:19] So right now you interacted with Blue's contract in the following way. You write the code, compile the code, generate the transaction. You then use Edwards 2, 5, 5 1 9, which is an elliptic curve. When we use a signature called it's a signature algorithm to sign the transaction with. That transaction is then submitted off onto the chain and then it's executed by the ledger API.

[00:16:43] But I think there's an important thing to realize here Plutus depths or Plutus scripts. Don't go onto the chain until you're interacting with them. So you include the Plutus script in the transaction that you're submitting to the chain each time you want to interact with it, but this is going to be changing.

[00:17:01] Let's look at some of the sips and the improvements that. So we're making fluid is better. Sip 31 defines a thing called reference inputs and reference inputs is going to make a huge change to how developers deal with interacting with UTX owes. I talked earlier about the data, the data, or the hard disk for the script where you can store data like high scores, et cetera.

[00:17:27] Right now, if you want to read your high score in your DOP, you have to consume the UTX and then recreated after you've read the data. Well, that's changing sip 31, which is coming in June will allow you to read the data or the data that's stored at UTX. So without consuming it and recreating it, and this means that multiple depths can read from the same data at the same time.

[00:17:51] I think the benefits are obvious. So 32 defines a thing called inline datums. So right now that high score, that data that I've talked about, we don't actually store it on chain. We store a hash of it on chain or a fingerprint of it on chain. And it's up to the developer or the user to include it. When they're interacting with the script.

[00:18:09] Well, no longer, you're going to be able to actually store the data on chain, moving much closer to a truly decentralized architecture, sip 33 reference scripts, another critical one. On Ethereum, the contracts live on the chain and you talk to them by a reference. Well, in Cardona, as I've described in the previous.

[00:18:29] We don't yet do that. We have to include the script and the transaction. Every time we're interacting with it. Well, sip 33 changes that you can now push a script onto the chain or a contract onto the chain, and then you can interact with it via a reference. So this is a very lightweight way to interact with smart contract.

[00:18:47] Think of it this way, rather than having all of the app logic in your transaction. You now just have a small address, like an email address that you include in the transaction. And it points to the script that already exists on chain. Really. We're also bringing some other cool geeky things around crypto.

[00:19:02] So Bitcoin and other chains can use different elliptic curves than we do on cardamom. We use, uh, as I mentioned before, Edwards 2, 5, 5 1 9, which is the same as other cryptocurrencies like Monero, but Bitcoin, Ethereum and others use , which is a Cublets type elliptic curve. So we're going to bring.

[00:19:21] Built-in support in-car Dano. So you can interact with signatures from those that are blockchains, and this could be done before if developers want them to do it manually, but this is going to be a hell of a lot easier because it's built in. So it's a one-liner to interact with those signatures. Now we're also bringing some really exotic stuff we're being pairing based cryptography.

[00:19:40] Now pairing base crypto, that was beyond the scope of this presentation, but we're going to bring support for fundamental primitives and extension field, um, for BLS 1230. Which is a pairing friendly elliptic curve. So this is going to open whole new classes of app with pairing based crypto. You'll be able to use homomorphic, additive signatures to do some very cool stuff.

[00:20:03] We're making food as faster, the core interpreter, the thing that executes the untied Plutus core that I described earlier on, or the ones and zeros, the raw app, that interpreter is being made faster and more performance. And this helps in a number of. It helps ensure that validation of blocks is quick and efficient.

[00:20:20] It helps ensure that the overall blood propagation times are low and indeed it helps ensure apps get executed quickly. So we've made the script size or the Lambda representation, 20% smaller in our next. Our interpreters ablazing 40% faster and non evaluation processing. So this is not running the code, but other things that it has to do, like data munging and cost modeling, that's 80% faster.

[00:20:46] So we're not resting on our laurels. We're making things better. Even at core level would include is one of the things that we've had some issues with has been collateral outputs whenever you're interacting with. You have to have some collateral as part of your transaction to cover the unlikely event that the script fails in phase two validation, what's phase two validation.

[00:21:11] Normally when you have a flutist script, we check before we submit it to the chain that it can definitely run to completion correctly. This is determinism and it's one of the virtues of Plutus over other contract platforms. Like. Well, that's great. But what happens if someone who maybe shouldn't be doing things like this created a transaction that they knew would fail phase one validation and submitted it to the chain.

[00:21:34] These things have happened with some bad implementations in certain wallets and certain hardware wallets. Well, in those scenarios, Nothing too bad what happened, but ultimately the collateral will get taken. So you'd lose your collateral. It's like an overcharging of a fee. We didn't feel this was a great user experience.

[00:21:52] We wanted the user experience to be really great. So we found a way to submit a transaction, including collateral, where the collateral that you include is just enough to cover what you need. And if you include more by actual. Like a million ADA, you get back everything that's not required. So we now have a much better way to deal with collateral.

[00:22:13] This is all part of a journey and get included to be a great user experience. So even if people make mistakes, they don't get. Let's talk now about determinism, parallelism and concurrency. These are virtues of the Plutus platform, and this is the unique selling point. This is what's different about building on Cardona versus other platforms.

[00:22:32] And I think you're going to find it pretty great. So determinism and validation, parallelism. I'm glad I said that. Right? So. I not sure of how many users we'll have we'll have come across this, but there's a concept called a directed acyclic graph. And it's this idea that data can be thought of sometimes like a spider weapon.

[00:22:51] So you've got these little nodes circles and have lines to the next one lines to the next one. It's a big web grows and we call this web or graph and directed acyclic graph, especially if it goes in one way. And it turns out that the Cardinal ledger forms a graph of transactions. Well, graphs are great for parallel processing.

[00:23:11] Hydro does this chain revalidation does this Cardona enables by definition, parallel processing with the way UT EXOS work. And this means that because Plutus core is deterministic and because scripts only have access to local information, we can affect. Parallel process, many things during both validation of the Plutus script and indeed validation of the ledger.

[00:23:38] Let's look now at contention and application concurrency. So you take, so it's going to be spent once applications. Or depths that are built where multiple entities or actors try to spend the same UTX. So simultaneously we'll contend on that UGA XO or ultimately be blocked so we can achieve better than this.

[00:23:58] When you're building on Cardona, you have to remember better. Concurrency can be achieved by using multiple UTX, sows, and exploding. The parallelism that I described in the previous slide. And you can build with this style, a scaling. That's massively parallel and allows you to service all of your users at the same time, as well as that coming in June reference inputs, as I described earlier, will allow, read only access to datums that live on UTX owes to multiple apps at the same time.

[00:24:29] Let's wrap it up now a quick conclusion. So this is powerful and what's different in execution to other platforms. Plutus is just as capable if not better than the company. Plutus is about to get even better than that, though. Both in terms of user experience with things like collateral, that puts that I described and performance, as we've looked at with the enhancements that we're bringing to the Plutus interpreter.

[00:24:54] I hope you enjoyed this. Look into some of the fundamentals around Plutus and I hope you'll enjoy building on what is going to be the greatest smart contract platform for the next five years. Thank you.

[00:25:07] So, John, thank you for that. And I do make sure you leave any comments and questions below and indeed, any future videos that you'd like to see. You never know if we ask him nicely, John might do some more for us in the future. Let's talk about billing and Caetano. Next. Matt's going to meet a few more projects in a moment.

[00:25:23] And if you want to try and stay up with all the incredible activity happening across the system, make sure you follow us on Twitter. We put out our regular thread. They're trying to capture at least. Of all the activity across the ecosystem, you can also try subscribing to our new essential Cardona newsletter.

[00:25:38] The link is below for the latest updates on what's happening also below you'll find a link where we're asking you about Caetano 360. We want to give it a bit of a spring spruce up. So please let us know what you'd like to see on that show. I'll leave Matt to close the show out now with some of the projects building on Cardone.

[00:25:54] We'll see, on the last Thursday of the month for Cardona 360. Thanks a lot. I was glad this week to get a chance to speak with a few of the projects that have been on the show. In the past, we spoke with melt, ergo decks, musically swap. So Ken, tell us how things have been at meld since you were on last.

[00:26:12] Now it is a lending and borrowing protocol on the, on a blockchain. And what we're trying to do is we're trying to create a full banking stack on Cardinal, and that includes crypto to crypto lending and borrowing. And it also includes crypto to Fiat lending and borrowing algorithmic, stable coins, and other features and functions, uh, connected to banking, but more in the defy side of things.

[00:26:35] So we're working exclusively in defy and we're working exclusively with non-custodial and decentralized technologies. So since I was on last time, we've had our token event. People are now able to. Have and use the meld token. They can stake it in our app. You can use our app and connected to the NAMI wallet.

[00:26:54] Since the token launch, we've been sort of had our head down and focused all of our attention on actually building the applications and tools. So we're building things like a bridge to be able to bring assets across from. Blockchains. We are building, uh, frameworks to be able to show real-time graphs directly off of the Cardinal blockchain.

[00:27:15] So we're doing a lot of things, um, on the tech side, but we're also doing a lot on the legal side because we're touching Fiat. Uh, we're dealing with regulations. We're applying for several licenses right now. We have a couple of really interesting announcements. They'll come out various. So, if you're interested in knowing more and sort of keeping up, then you can come to our telegram or discord channel.

[00:27:36] Um, there you'll be able to find out a lot of details on a sort of last note. We're also in the process of announcing some really interesting NFT stuff. Thanks for the update, Ken. So over to you, Yasha, how things been at Iridex I would go next is a non-custodial decentralized exchange, which we are building on top of ergo, anchor a blockchain.

[00:27:54] Uh, we also committed to breach these two blockchains via our protocol to make it available, to transfer liquidity among them. So we implemented that or talking out to the pub, the framework, which allows us to programmatically create sign and submit. The framework is based on Cardona note code base and has a good interoperability with the blood test data model.

[00:28:16] We also implemented our good ex smart contracts in blue tar a low-level language with the writing Pluto's validators, which give developers, find gradients, uh, control over performance. Uh, we also cover it all of the code base with tests. Uh, we implemented AMM bots in Haskell, and we set up to test all of the Testnet net infrastructure.

[00:28:38] At Exxon Cardona, we also implemented a scalable service for querying Cardona blockchain state, uh, implemented ergo decks is the key, uh, in TypeScript to create a good X transactions in the browser enzyme. Glad to announce that we have repaired everything necessary for the launch of the. Uh, and we will provide you more information about that.

[00:29:00] So if you want to find the target X community, you have to simply go to ergo dex.io website, and there you will find all of these social media links and all of the communities. Oh, I ended up, I would like to add that currently we're working on a ergo maintenance and also we are working on, uh, Cardona Testnet, but, uh, the Testnet is private.

[00:29:25] Uh, and within one week or one and a half week, we will open it to public. And the next month we will launch it in main net. Thanks for that Yasha. I think the community will be really excited to see our codex on Cardona net. So over to you, Samuel, uh, how things Bennett music swap. Hi. So I'm Samuel from useless swab for those who don't know yet.

[00:29:47] And muesli swap is a decentralized exchange on Cardinal. And in fact it has been the first decentralized exchange to launch at the end of last year. So at the end of last year, we launched a. Order book decks. And since then we've progressed quite a lot. So we've been able to really gain the support of the community.

[00:30:05] And then our big, last three accomplishments are that we've released staking for the merch token, which is the governance token of muesli swap. Then we've also got our version two contract audit, so we will soon release muesli of version two. And then most recently we've also launched muesli swap glucometer.

[00:30:25] This is a decks on become Commodore, which just says tight chain of Cardone. So, what you should look out for in the near future is muesli swap version two. We are right now working full-time on it, and it will be a decentralized exchange. Like your used it from maybe you need swap. So it will be automated market-maker style.

[00:30:43] That will be liquidity pools, and you'll be able to stop using those liquidity pools and also earn a passive income by providing liquidity there. So there's already a version on the test net. And we'll release the version on maintenance very soon. So stay tuned for that. Glad to hear that Samuel, we look forward to seeing.

[00:31:04] So Ryan, how things been at Ardhana? Hi, I'm Ryan Metova, founder and CEO here at Ardhana Ardhana is a stable coin ecosystem beyond just being a defy protocol built on Kardex. So we're building D USD, which is a over collateralized asset backed stable coin. And this is backed by Cardona native assets itself, a stable coin backed by ADA.

[00:31:31] And we're also working on a decentralized exchange for highly capital efficient swaps between stable coins and stable assets. So it's really building both the stable coins. Um, and having that as a provision for the ecosystem, but also the infrastructure to transact and swap between stable coins in a highly efficient manner.

[00:31:54] We have been under development for over a year now. And, uh, so far the focus has been really working on smart contracts and, um, bringing in interesting functionality beyond the stable coins, such as users being able to. Stay stick to their original state pool once they deposit ADA collateral. So this is, uh, a move by us to help, you know, support the state pools and allow people to continue that relationship.

[00:32:26] So going forward, our focus has really been on scalability. For the system that's for the stable coin and how we handle liquidations, the decentralized exchange, you know, and to the number of transactions that we can, you know, batch in the, you know, to a single operation on chain and really pushing that forward and anticipating the upcoming scaling improvements that we're going to see on Cardona and making sure that our solution can leverage, uh, all of those benefits, um, you know, in the most efficient.

[00:33:00] Thank you guys for being on the show today and for giving us your updates and thank you to the community for watching. Join us next time for more building on Cardona.

