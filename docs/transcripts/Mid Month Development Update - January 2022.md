# Mid Month Development Update - January 2022

[00:00:00] It's 20, 22 and time for the first mid month development update, where we have an opportunity to deep dive into what's happening on Cardona. Happy new year, everybody I'm joined as usual by Kevin, by John and also by Nigel. So let's dive straight in Kevin, let's start with you first. Happy new year. And it's a happy new note as well.

[00:00:24] Yeah. Happy new year to you too. Uh, Tim. So there's been a lot of work going on in the no team as I'm, as I know, you're very well aware of, um, we're very pleased to have, uh, just released a node version 1 33. And a really big improvement with this is to do with smoothing it, smoothing out the calculations that are performed by the ledger across the entire epoch.

[00:00:50] Uh, so we know that the SBOs have been waiting for this for some time. Uh, we've had. Various improvements in development. Uh, it's now been about seven or eight months. It's been quite a protracted process for us. We've been hoping to roll things out sooner. Uh, but what, uh, what we discovered as we were doing this was that one improvement uncovered something else that we needed to do.

[00:01:13] So there's been whole cycle of let's get things working better, but the, the good news for the end user, uh, is that we've announced smoothed out the. Competitional peaks the loop peaks in the nose, and we're no longer in a situation where the nose should take much longer to process, uh, blocks to include transactions at some points in the pot, finished others.

[00:01:38] And that's going to help us with block diffusion times, help us with the robustness of the network, the reliability of the network, which is paramount to us. Um, but it's also very, very important if for 20 minutes, I'm going to start moving forwards on, uh, various parameter improvements, increasing the block size, um, increasing the, um, CPU and script limits, et cetera, et cetera.

[00:02:03] So this is a really exciting, uh, and long way to development for us. And we're very pleased to have got this out as our belated Christmas present to the . And the improvements from this note also will start showing, I believe in the next version of Daedalus flights, which is sort of slated to be released next week, and then we'll show in the full Daedalus in time.

[00:02:24] But this, this improvement for the SBOs and in time, the improvement for Daedalus, that's really only the start of it. Isn't it. John, perhaps dig a little bit more into what Kevin's touched on there. It gives us more freedom. Doesn't it? It gives us more latitude. Absolutely. Tim, I like to compare it 1.33, our latest release of the Kodak.

[00:02:40] Uh, with what Steve jobs did at apple with Mako S years ago, uh, with snow leopard, uh, I'm a bit of an apple nerd. That's why I'm bringing that up. So Mako S obviously a fantastic operating system. We're leading operating system, just like windows and Lennox, but there was a point where they'd added so many features that they thought, okay, we're going to have to go under the hood here and tune things.

[00:03:00] And that's really what we did at 1.33, we took a feature. Cardinal node and we wanted to make it sing on every possible computer out there, not just the types of really high end machines that SPO will typically have. We want it to work great for it. So we took the opportunity at 1.33 to dive under the hood and make some, uh, elegant and efficient changes.

[00:03:20] Um, so that things, as Kevin already described, things will just work great ad, no matter what kind of computer you have. So this gives us the foundation to start making improvements again, to our layer one, uh, scaling. So with the advent of 1.3, We will now have a much more uniform response of block propagation across the epoch.

[00:03:42] And what I mean by that is simply, uh, the week have reliable, consistent times on how blocks propagate across the network, which of course is what we want. And when those times are nice and low, okay. Without any spiky behavior caused by the old way of doing reward calculation, which is now gone, uh, this gives us the room to start increasing parameters for plus.

[00:04:00] And, and increased block size. So that's going to be something that I'm going to be aiming to do in January. I want to start increasing the available resources that developers should have access to when they're building out applications on clues. But, um, that's just the first part of the story. 1.33 is really only the.

[00:04:17] Let me give you a list of things that I'd like to walk through, which kind of puts a frame on what we're trying to do this year. This year is about scaling layer one this year. I want layer one to be the fastest. Uh, it possibly can be the first one is node in Huntsman. So 1.33 was the beginning. We're not just stopping there and the next release, we're going to have a whole bunch of work done on how we manage and use memory.

[00:04:41] Memory of course is very important. It's another resource within your computer. Um, and we're looking at memory complexion and memory, memory sharing techniques, which are going to greatly reduce, uh, the memory usage of the Cardinal core node. And we expect improvements up, up to about 40%. So really. The changes that we're going to be dealing with the, with the efficiency on the node will also allow us to constantly be increasing the block size.

[00:05:02] So that's something that's going to be constantly increased over the course of the year as we have this headroom to do so the same, uh, Plutus um, uh, resource limits. So the memory and CPU that's available to a Pluto script that really contains or defines the types of things you can do in a play the script.

[00:05:17] And we want Plutus to be as articulate as possible. We want it to be as powerful as possible. So in order to do that, we need to give them. Uh, bigger resource limits. So again, these resource limits will be changing throughout the year on. Number four is probably the one I'm personally most excited about.

[00:05:32] It's a pipe-lining. So pipelining is a mechanism, uh, technically to coalesce validation of a block and propagation of a block. Um, so let me put it in, in more simple terms right now, a block has mended by an SPO. That's a new block in the blockchain. We have to validate it and we have to send it on to our peer.

[00:05:50] The problem is they also have to validate it and then send it off to their peer. And that's how the blocks diffuse across the network. That's fine. But. It takes time to do all of that validation, every hop, more validation, that's eating up time and it's eating up time that we would like to use for bigger blocks and more pleased limits.

[00:06:05] So what are we going to do? Well, we can kind of squeeze together this process of sending the block out and validating the block. So we're kind of doing them both in parallel or pipeline in that process. Now there are some technical implementation details have to be worked out in terms of how we're going to make sure that we.

[00:06:21] I have all of our corners covered when it comes to implications that may arise when you're doing this. Um, parallelized behavior, but it's, but pipelining is going to be something that's going to give us significant headroom to again, increase throughput on layer one. Um, and when I say significant, I'm hoping, uh, like an order of magnitude.

[00:06:42] Um, let's talk about number five, input endorsers. I don't want to go too deep into this one because unlike pipelining, which is now exiting architecture and beginning implementation app input, endorsers is still, uh, working in the architecture. Slash research kind of vertical, but input endorses is going to be the, I would say, a near end game solution for layer one scaling.

[00:07:04] So it's going to, it's going to put car down on the top of the pile when it comes to a throughput for their one. Um, it's a mechanism by which we've changed. Uh, quite rightly. The process for block production and block propagation. So rather than scoping transactions out of the men pool, which we currently do and forging a block and then sending it onto our peers, which is the current state of play instead blocks will be created on that hoc basis, signed and countersigned, and, and we'll be flying around the network, uh, on a New York.

[00:07:32] Um, second-by-second basis. So I'll do a deep dive technically on that later on, it's a little bit hard to expand at this point because the research is still working on it, but it's something that we're going to see towards the end of this year. So it really is going to come after pipeline and it's going to come after the changes I've already described.

[00:07:48] Of course, then we have enhancements for, uh, for Plutus. The increasing the resources available to include this developer. Uh, we're going to make it easier for Plutus developers. So number six is Pluto script and Huntsman. And I've talked about these before reference inputs. This idea that you can reference an input without creating, without destroying and recreating it, uh, inline datums.

[00:08:07] So you don't have to worry about bringing the data to the party when you're interacting with a script and then script references, similar to online datums at the moment you need to bring the script whenever you want to interrupt. But no longer you'll be able to appoint to a script on chain. So these are really about reducing the friction for developers and making transactions smaller and more elegant.

[00:08:27] Number seven is on disc storage. We're acutely aware again, going back to 1.3, three making, making the note. Great. We're acutely aware of that right now. The Cardinal node needs a lot of Ram when it's running. So we want to start moving things out around, out of that expensive, uh, you know, volatile. Into on disc storage, which is a very common pattern in computer science.

[00:08:45] Um, and on disc storage is something that will just be a, kind of a quality of life improvement for users of the Cordata note, eight and nine are kind of related side chains and hydro. At peer-to-peer channel. Okay. Which allows people to do peer to peer transactions, uh, in an offline channel and then settle into main chain.

[00:09:03] Hydra is a major part of our scaling plan, especially for certain types of interactions and transactions on, on, on Cardinal. But of course we have side chains too. And so I changed could be there's many, many different use cases. Uh, some examples are stable coins all the way through things like potentially having a side chain that can execute smart contracts from other platforms.

[00:09:23] So really excited about how that will let us take load off layer one. I mean that, and put it onto a side chain all the while enjoying the veracity. Uh, that's that's that's provided by that, uh, main net layer one. Um, we're even looking at off-chain computing, which is a potential way to do faster and cheaper transactions via a trust model.

[00:09:42] And then finally, uh, number 11, uh, in my list of cool ways to enhance Gordano for 2022 is Mithril. Um, I'm not sure if we've talked about Mithril really before, uh, it's a technology using a pretty, uh, exotic crypto. Uh, I want to say Kryptonian crypto cryptography, non cryptocurrency. The Cola state-based threshold, multi signatures, but ultimately what Mithra lets us do is allow us a computer or a device that doesn't have a large computational capability such as a phone or a raspberry PI allow a computer like that, to be able to validate the entire chain.

[00:10:17] Now, of course they can't validate the entire Cardinal layer one chain block by block because that will be too computationally expensive. So Mithril does, is it effectively checkpoints the chain and it puts a stake in the ground and says, It's good to hear. And then it goes to me, maybe for another a hundred blocks, another steak.

[00:10:32] Hey, it's good to hear. And what we can do using some cryptographic magic is that we can have one of these lights before. Take the, all of the steaks out of the ground, check them quickly. And then they know that the chain is valid without having to do that work themselves. They're the kind of things we're thinking about, but ultimately 20, 22, it's about layer one scaling, and we're going to get carved out to be a really compare very busy year ahead of those optimizations, John.

[00:10:55] And of course, it's also going to be very busy on the network, at least in the early days, isn't it. We need to, we need to recognize that. Absolutely. And we're aware of this, uh, the things I mentioned from. The release 1.33 that we've just put out that gives us headroom to make the network parameter bump that I want to do this month.

[00:11:12] All the way to, uh, lay offs and input endorsers and side chain computing. We have a journey to go on and it's not going to take long. We're going to start seeing some of these things roll out in Q1, a major ones like pipelining and Q2. And then later on in Q3 and Q4, some of the other more exotic things I've talked about, like lay off on input endorsers, but ultimately Cardinals, a permissionless.

[00:11:34] Anyone can launch any application at any time. And additionally, um, there's a lot of excitement around Guardino, um, and a whole bunch of different, uh, different verticals from NFTs to Dobbs, to Texas. We are seeing an enormous number of projects who are nearing completion of development and are imminently going to launch.

[00:11:53] And if it so happens that in, in January or February, before we roll out some of these, these scaling changes, we see excitement and we see, uh, adopts rollout together concurrently. Yes, you can expect to see main net busy and yes, you may have to wait a couple of weeks. Uh, for your transaction to go through, uh, depending on, on how busy it is at a given time.

[00:12:14] However, we have a really, really solid plan for scaling. And we also believe that right now, the network is in a place where it is a secure, robust, and also act quite performance, but we're going to be making these changes to make sure that we grow as the. Thank you, John. So Nigel, a very busy year ahead and as a head of delivery for Cardona, a lot of this is going to be down to you.

[00:12:36] The beginning of the year has really been about setting new processes and systems up to help deliver these core capabilities and also our developer engagement sort of framework as well. Perhaps you want to tell us a little bit more about how your year is. We kicked off the air. Obviously the first thing we do is as John as alluded to is making sure that we're supporting the launches for, uh, the dApps coming online.

[00:12:58] So we've done a lot of work around the network infrastructure. We've pushed out a new node. That's more efficient on block propagation and all of these things that John's just, just touched on. Um, what we're doing on the opposite side of that is. Supporting the DAP developers. So we worked with lots of partners, but we're close to 200 now.

[00:13:20] And in partners that we're working with and all the things that are going on in the network, we're trying to reorganize ourselves and reorganize our processes. So that we can listen to what people want, the issues that they, that are arising, um, and then start to schedule it and prioritize them. Um, and so we've got to, we have got a different way of looking at 2022.

[00:13:42] Uh, last year it was about building the infrastructure is a much more, uh, entirely focused. Now it's much more market focused, listening to the community, listening to see how these innovative engineers want to change our network and what the kind of issues are that they're experienced. So we can support them in line with this.

[00:14:01] We've just kicked off a liaison with the Alliance, which is a collection of 15 different DAP companies or within the . They've got a particular collection of things that they want to see in terms of future innovations. So we're working with them to try and develop this, not just for ourselves to kind of do different things, to improve the infrastructure, but working with those guys to actually maybe support them, maybe help to fund them in terms of the things that's going to help other people as well.

[00:14:31] What we would like to do is just say, it's not just defies, you know, we would encourage, uh, To think about other alliances that might be suitable. Other areas of innovation, whether it's NFTs or Oracles or other kind of a useful ideas that they, they build their own communities in terms of actually the deliveries we've got this.

[00:14:54] Um, there are things Don's alluded to all the, the, the innovations we've got all of that going on. There'll be improvements to our police libraries. We'll be doing another education program on, on police sets, not just for the old stuff, but how the innovation works. Um, we've got more work going on within our wallet area.

[00:15:14] So there's more innovations going on there and we'll be keeping pace for the rest of the month. So, yeah. Nigel, you mentioned governance then our Kevin, you are very heavily involved in the, in the Voltaire, uh, work at the moment. Governance is going to be another massive theme for 2022. Perhaps you just want to give us a little bit of an overview here.

[00:15:31] We'll obviously deep dive into it later in the, uh, later in the year, but give us a little taste of what are you going to be looking. Yeah, so that thanks to him. So I've been spending a lot of time talking to the capitalist team and to the governance team. More generally, we've brought on a whole new layer of a product managers and project managers are, who are focusing specifically on Voltaire and capitalist issues, uh, in 2022.

[00:15:56] And what we're going to do is to move towards a system where the community is much more actively involved. In the governance of the blockchain, where we, uh, take a more active view of the steps that the community has been submitting. Ah, there've been a number of excellent steps that people have put forward.

[00:16:16] What we need to do is to make sure that these now go from the ideation stage are the stage where we set up looking at providing comments, checking through, uh, helping reform. The ideas are through an implementation phase, which could be through project catalyst, could be through some other funding source.

[00:16:37] And ultimately that the community accepts the ideas that it through some open process of, um, decision-making agrees that these SEPs and other, uh, actions should be carried forward, um, on Cardone. And then inactive for the overall benefit of the community. So, so it's going to be a big shift in the way things the time, uh, it's going to be a shift in the control of the, um, blockchain development, um, as a whole, it's going to be very significant of course, uh, for.

[00:17:13] Gentlemen. Thank you very much. And remember, there'll be more updates on the development side on Cardone 360, the last Thursday of every month. But before we go, Matt has been out and about again, meeting some of those DAP development projects we've been talking about just now. So this third iteration of the building on Cartano series, I had the opportunity to catch up with some of the amazing projects that are building on Cartano.

[00:17:37] Uh, I talked with meld men swap or codex Byron network and indigo protocol. Um, we heard updates on their development, their launch plans, uh, and their vision for the. Meld is a decentralized non-custodial protocol that makes it possible for us to lend and borrow crypto and most uniquely Fiat. So we are on the corner of blockchain and make it, we use smart contracts to make it possible for us to take cryptocurrency, lock it up into a smart contract.

[00:18:11] And then be able to borrow against that either borrowing Fiat or borrowing crypto, we are developing and cross chain exchange protocol called urban X, which includes AMM and order book functionality. So our company based on a three simple principles, distance or decentralization first, uh, open ends in transparency in everything.

[00:18:33] I mean, organizational operational technical aspects. And the third one is, uh, orientation for the user success. Well, there's a lot of advantages that we saw and decided early on to build on Cardinal, I think from my standpoint, as an entrepreneur, um, and consultant in technology space, I've kind of gotten to witness, uh, the infancy of new innovative spaces and see opportunity there.

[00:19:02] So, um, choosing Cardona was easy from. Uh, standpoint that the whole data ecosystem, uh, was very infant and its existence existence rather than I think it still is, as opposed to say a more saturated, uh, ecosystem, like what you see on the Ethereum. Also the ecosystem, I, I strongly believe, uh, is second to none.

[00:19:25] Uh, Very robust, passionate ecosystem, uh, in community following, oh, the whole Cardona space from a developer perspective, you know, we, we get the beauty of having formal verification written into, uh, very closely to Plutus and, uh, being able to integrate very closely between the off chain pieces and the on chain pieces using the prunus application backend, we chose Cardona.

[00:19:49] We chose it primarily because of the low transaction fee. And the high transaction rates. So that was the sort of initial thinking some, you know, year ago or so, but as we were working on it, we realized that while that was valuable, the more valuable component was the decentralization part, the proof of stake, and the way that proof of stake works on the platform.

[00:20:13] And also the fact that it has high capital-efficient. So the capital efficiency part and the, and the staking have actually proven to be a much bigger component or a much bigger benefit for us on cardamom. One of the main advantage of building on CareNow is, is by using the rotational model, which has local state and has a pure model that is within about, and we have to, we don't have to worry about things like the boat agency when we designed smart.

[00:20:47] And kind of know also have a big and helpful community that are very nice. Another feature I really like in a Cardona and arrogant as well, ecosystem, uh, is eroding some model. It allows us as a developers to build composable product. Uh, such a way of development allows us to combine and reuse different pieces of protocols code, uh, in different places.

[00:21:12] For example, it is possible to create a stable coin based on our current AMM, uh, pool protocol, uh, and vice versa from the. A stable coin. If it's implemented tolerating, uh, you can easy, uh, based on these protocol, I mean, stable coin, you can create amen pool or some kind of other protocols. Uh, they do. So what a EOD XO model brings to us, the advantages of building on the current dyno is essentially at the beginning, it was, uh, learning, uh, cool stuff.

[00:21:51] That was the, the, the, the biggest thing for us. And, uh, we are, uh, we are great grateful for that. And today as we are moving forward and we can see, uh, what for, we can use. No w what we can use it for it, then we have more and more ideas. So for example, I was an operational guy in a software development agency.

[00:22:12] And after I just resigned from operations, I started my own startup called . And this is a startup for central and Eastern Europe. Within the FinTech. We are integrating, uh, banks with an open banking. So Cardinal right now looks like the best choice. To build a buck. And for that, uh, I really strongly believe that we could create once we integrate with, uh, banks, then, uh, we could use and Cardinal as a registry, uh, similar to the registers that are around the ward to, to, to compare, uh, banking, uh, registries.

[00:22:52] Well, along with our development, uh, we've been building since may of this. Um, our engineers are some of the top food contributors to date. Um, and we have multiple merged. Uh, we have actually completed our initial audit with external third party from a tweak who I'm sure you're familiar with out of one of the few at this point, who are capable of audit included.

[00:23:17] So we're really excited to be at that stage at this point, you know, we're, we're really focused on contributing. Um, integrated in closely with the Plutus application backend and, uh, working on finalizing our design and spec, you know, we're working on opening up a private Testment for a closed, uh, our partners and, uh, uh, people close to our protocol within the ecosystem.

[00:23:43] Um, Point afterwards, we will open up to a public test that, and the main that after, uh, we are hoping to fit a lot of this into Q1 of 2022. And if anything needs to be push back to Q2 development is going well. We're making good progress. We'll be launching the protocol on the 31st of Jan. And then we'll be launching lending and borrowing in Q2 and we'll be launching, um, the Fiat side of things in Q3.

[00:24:16] We are currently working with twig and a couple of other development teams that are also collaborating and some researchers to build some tools. Called hace for doing auditing on the Catano blockchain. So you can go into these smart contracts and you can use our tooling to do security audits. Um, so those tools that we're collaborating to build are also being used against our own smart contracts on our, in our own audit, which twig is doing for us.

[00:24:46] The progress has been moving very smooth lately. And as of today, uh, we are official, complete, and we are prepared. Well, the audit we're already finished with the smart contracts. Now we're just have a, uh, the easily as the gate, uh, testing and a formal verification of AMM contracts, uh, left to finish it.

[00:25:07] Uh, we are designing, looking at things in accordance with our basic principles and trying to accommodate the interests of all parties. Uh, we're preparing a total economics release, uh, in the first quarter next year. We're excited as well about the Cardona defy Alliance. You know, having a, a member Alliance of defy for us, I think is a very, uh, powerful tool, um, and consortium so that we can work together, collaborate on innovative ideas.

[00:25:38] Some of the things that we need, uh, for. Um, our defy Dobbs to function and co-exist certain technology innovative, um, things that we can look at together as a collective and share that information and insight. So as to empower really every protocol. Um, so we're really excited about that. Thank you so much to each of the projects that presented today.

[00:26:01] Uh, we are really excited for what you guys are doing, and we're excited to see the future of your projects on Cardona. So thank you, Matt, for that. And lots more videos like that to come. If you want a deeper dive into some of those projects, make sure you check out community resources like Caetano cubed, like built on car Dano and building on Cardona.

[00:26:21] You'll find the links below and for a full directory of the Cardona ecosystem. Check out the essential Cardona repo it's open source and open to your contributions, but together let's try and map this whole exciting. Thanks very much for joining us and we'll see you on the last Thursday of the month for the next Cardona 360.

