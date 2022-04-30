# IOHK _ Cardano whiteboard; overview with Charles Hoskinson

[00:00:00] Hi, I'm Charles Hoskinson chief executive officer of input-output Hong Kong. And I'm here today to talk a little bit about car Dano. So to understand car Dano first, you have to understand where Cardinal came from. So let's talk about the first generation of cryptocurrencies. So. First gen is Bitcoin. And the problem that Bitcoin was trying to solve was really, could we create a decentralized money?

[00:00:31] Could we create some sort of token that lives on some sort of decentralized blockchain maintained by people all around the world? And that token would be scarce and tradable. So when Alison Bob want to send value to each other, There would be a mechanism for doing that did that did not require a trusted third party, a trusted intermediary.

[00:00:54] Now this was kind of a really cool and interesting idea. It had very old roots starting from the 1980s and beyond, but Bitcoin was really the first to bring this all together and it was a tremendously successful. After just a few years, Bitcoin not only accrued thousands of users, but also started being worth real money.

[00:01:14] Tokens went from less than a penny to actually a dollar to eventually a hundred dollars. And right around that time period, we saw a huge influx of people saying, boy, this is really interesting. However, the issue is that the transaction between Alice and Bob. Has more than just the act of moving money associated with it.

[00:01:34] There's a story behind that transaction there's terms and conditions. For example, what if Alice says the Bob I'll give you the money, if, and only if you mow my lawn, I'll give you the money. If, and only if you repair my roof, this is a contract. This is the story. So generation of technology wasn't really well suited for this.

[00:01:55] Every single time someone wanted to make a change. Bitcoin they'd have to build another cryptocurrency or they'd have to figure out how to install some sort of cumbersome, overly protocol like master coin or color coins. So back in 2014, metallic Buterin, myself and many others came together and we launched the first, second generation blockchain.

[00:02:16] And this is a theory from now, Ethereum. It's kind of like when JavaScript came to the web browser, we went, went from these static, simple pages that were not terribly functional, but at least they did something to pages that were fully programmable, that this then enabled us to build the Facebooks, the Googles, the Gmails, the experiences we've come to know and love.

[00:02:40] So a theory, I brought a programming language to a blockchain. So this programming language paradigm allow. Smart contracts to be written, to have customizable transactions. So when Alice sends that value to Bob, all those terms and conditions could then be embedded within the transaction and it can be bespoke to her particular needs.

[00:03:02] Now this paradigm like Bitcoin also took off and now Ethereum is among the largest of cryptocurrencies and has a huge developer community. Unfortunately just like Bitcoin, we're starting to enter into a new. We're going into the third general.

[00:03:22] Where we've realized that a theorem can't scale to millions of users to billions of users, the theory doesn't really have a good developer experience. Ethereum and all cryptocurrencies have really a bad governance experience right now. Where every single time there's a major disagreement instead of finding a way to resolve it.

[00:03:39] We end up usually seeing things like a theory and a theory of classic or things like Bitcoin and Bitcoin cash. Furthermore, there are big sustainability problems in the space. Namely, after the ICO money is out for a project that's funded this way, or let's say the venture capital runs out who will fund to grow the chain who will fund to actually build out an ecosystem.

[00:03:59] These are big open questions. So the third generation. It's all about three topics. One is scalability.

[00:04:09] Two is interoperability.

[00:04:15] And finally there's this notion of sustainability.

[00:04:22] So the Cardona project is really our philosophy, our vision on how to solve each of these catheters. In a way that we feel it's going to inherit the best features and lessons learned from generation one generation two, but also add a lot of new concepts and technology for the specs. And this project is built with some really good principles, namely to first off all the science that guides the solutions to these problems go through some notion of period.

[00:04:53] So we go to conferences, we write proper scientific papers. We engage universities and all the engineering, we have the goal to eventually implement as high assurance code,

[00:05:08] which means the same types of techniques. One would see with the shin constant or a jet engine where when the failure of the system results in. Death, uh, we can apply those techniques to a, uh, to our protocols, to engineering and development so that we have a much higher belief in the quality of the code, this avoids events, like the Dow, the parody hack, and other, such things as we've seen in the space.

[00:05:31] So let's go through each of these in more detail, starting with scalability. So scalability is kind of a loaded term and it has a heck of a lot of meanings, but. Uh, cryptocurrencies perspective, you can really think of scalability in three different perspectives. So one is scalability in terms of transactions per second.

[00:05:58] So you'll often hear people say, well, Bitcoin has seven transactions per second, or a theory. Them has 10 or 20 transactions per second. And this new protocol has 200 transactions or 300 transactions per second. This is this notion of how many transactions I able to get into a block within some finite period of time.

[00:06:17] But it's not the only thing that you have to concern yourself with transactions carried out. And as you get more transactions, you require more network resources. So there's also this notion of bandwidth or a network where for a system to scale, if it's going to go to millions and billions of users, that system could require hundreds of megabytes to gigabytes per second of bandwidth, to be able to support all the data flowing through it.

[00:06:42] This is very common in the enterprise world, but not quite where we need to be in the peer-to-peer world. And then finally, there's this notion of data scale. So blockchains. Store things, hopefully for us. And so every time you put a transaction in, regardless if it's relevant or not, it ends up in the log.

[00:07:00] And as you have more and more transactions per second, you need more and more data. And as a consequence, blockchains will grow from megabytes to gigabytes, to terabytes, to petabytes, and potentially even. Again, this is okay in the network world. But when we talk about a replicated system whose security model relies upon each node, having a copy of the blockchain, this is not tractable for consumer hardware devices.

[00:07:24] So carnal, what we're trying to do is figure out ways to solve these problems in a very elegant. Namely that as we add people to the network, we naturally get more transactions per second. We get more network resources, and eventually we'll get more available overall data storage without compromising our security model.

[00:07:44] So let's talk a little bit about some of the innovations we've already brought. Namely with the throughput, we have developed a peer reviewed white paper for a provably secure proof of stake protocols.

[00:08:05] called aura, Boris and aura. Boris is among one of the most efficient consensus protocols in the cryptocurrency space. And it's the first to actually be proven, secure in a very rigorous cryptographic way. The magic of oral Boris is that it's been designed in a modular way and it's been designed with future-proofing and it's the.

[00:08:26] So namely how world wars works is aura. Boris breaks the world into epics.

[00:08:42] It takes a look at the distribution of total. And it grabs from a source of random numbers. It's able to hold an election and create slot leaders. Now, these slot leaders functionally do the exact same thing that a miner would do in Bitcoin. So this is basically the same as a person who discovers a block, wins a block and Bitcoin, but the difference is that it doesn't require the extensive computational resources that Bitcoin requires to construct a block.

[00:09:09] And as a consequence, this system is considerably cheaper to run, even though. We still have similar security guarantees that Bitcoin currently enjoys. So it's a major advancement, but the other really interesting thing is that these slot leaders don't have to just maintain a single block and a single chain.

[00:09:28] They can actually maintain other blocks and other chains.

[00:09:36] Because the cost of constructing a block is so low. It's actually now tractable to talk about consensus over a range of blockchains instead of a single chain. Furthermore, epics perhaps could even be run in parallel. So instead of having one epic run and then another epic. One could develop a system using or a Boris were epics run in parallel and transactions are partitioned to court.

[00:10:05] What this effectively means is as you gain more users and your users gain more capabilities, these slot leaders will be able to maintain more types of blockchains and also run transaction processing for blockchains in parallel. This is a major advancement. The other cool thing is that, or Boris has very rigorous security standards in terms of its theoretical foundations, as well as its implementation.

[00:10:27] So as a consequence, as we develop new capabilities for the protocol, these product capabilities are somewhat compelling. Meaning that these capabilities will also be secure. Whereas other systems, one has to prove these things on a case in case basis, in some cases make major modifications or changes to their system.

[00:10:45] In addition to this, we intend on aura Horace, actually being quantum resistant sometime in 2018. Where, when the slot leader signs these blocks, there'll be using a quantum resistant signature scheme so we can get even more future-proofing into the system. So that's kind of the first view is how do we construct a way of maintaining the network that doesn't cost $300,000 an hour, which is what Bitcoin currently calls.

[00:11:08] At the current market rate of 5,000 per coin. And how do we build a system that allows us to go parallel and also allows us to potentially maintain multiple chains concurrently. This is the heart of war of Boris. Now, as we mentioned before, uh, one of the most important things when one develops new cryptography is to make sure that this cryptography is developed in a very rigorous peer reviewed way.

[00:11:32] So, or a Horace actually was accepted at crypto 17. Where our team went there and to present it and future versions of the protocol, continue to go through more rigorous peer review, giving us a high assurance that the conceptual design of the system is correct. The other side of it is we're actually modeling a formal specification of aura, Boris using psychiatry.

[00:11:56] Which is a wonderful, formal modeling language that's machine understandable that eventually we're going to be able to connect to the Haskell code in our GitHub repo, and actually show that we've correctly implemented the protocol. This is a standard that actually does not exist in our space, and we're very excited to be the first to bring it to the space, but that's not the only thing required for scalability.

[00:12:18] You also need the ability. To move large amounts of data at the same time as our network grows from a few hundred transactions per second to thousands, to tens of thousands, to hundreds of thousands of transactions per second, you cannot maintain a homogeneous network topology. In other words, you cannot have a situation where every node has to relate every minute.

[00:12:42] Because there are will be nodes that don't have those capabilities, especially as they grow. So we're actually looking at a new type of technology called Rena. And this stands for recursive

[00:12:58] internet work

[00:13:02] architecture.

[00:13:07] And so Rena is basically a new type of structuring networks using policies and, uh, clever engineering principles, mostly conceived by John DEI. Who's based out of Boston university. And the goal here is to build a heterogeneous network that gives you similar types of privacy guarantees, transparency, guarantees, scalability, guarantees that you would expect to get from a network protocols like TCP IP.

[00:13:38] I do so in a way where you can actually reason about how the network is going to compose in a formal capacity. So in other words, Rena is a major step forward that will give us a way to very naturally tune and configure Cardinal as it grows from hundreds to thousands, to tens of thousands of transactions per second, and something that will very seamlessly connect and inter operate with TCP IP.

[00:14:00] We're very excited to bring this in part to the Cardinal ecosystem in 2018 and in completely. Around 2019 and we think it will be a big solution to a lot of the network overhead issues that we have. Finally, we have this notion of data scaling. So this is among the hardest of the problems. And it's one that we're still examining and looking at.

[00:14:23] But the reality is that not everybody requires all the data and the transactions that Allison's, the Bob are not necessarily relevant to even Jane and. If there are only relevant from the context that these people are able to infer from them, the total ownership of the money and know that the tokens they receive are legitimate and correct.

[00:14:47] So you have techniques like pruning, you have techniques like subscriptions

[00:14:57] and some form of compression, which when applied in a sec, In a very intelligent way can actually reduce substantially the amount of overall data. One user has to have. There's also the idea of partitioning

[00:15:18] partitioning is where a user doesn't actually have a full copy of the blockchain. Rather they have some chunk of. As opposed to many other chunks. And there's some notion that you can put all of these things together. So what are the goals of the Cardinal project is to study this in a very rigorous way and to come up with new blockchain architectures as they become necessary, uh, that will allow people to have much smaller amounts of data, but overall, uh, still get the same level of assurance and security that the transactions they've received, the computations that are performed are.

[00:15:52] Uh, so part of this research also involves some of our ideas about side chains and we'll get to that actually, when we get to the interoperability section. But as a brief mention, all a side chain really is, is two components. First, it's the notion of creating a compressed representation of a blockchain.

[00:16:14] And it's the notion of creating interoperability between chains. I, a way of translating transactions between chain. So some of the proofs that we've come up with with some of our recent side chains, research gives us a lot of hope that we can create compress representations of a blockchain as it grows from gigabytes to terabytes to petabytes.

[00:16:33] And that these proofs can give us high level of certainty that the transactions we're seeing, the history we're seeing is correct. Even though these proofs are quite small megabytes to kilobytes. So this is kind of our solution to data is to approach it in a, both a pragmatic way where we see.

[00:16:50] Restricting in some cases, what people see in a very intelligent case-by-case basis, we partition things where, and when we can, and we find out really intelligent cryptographic ways to compress history, which gives us the same level of confidence. Even though we don't have. But do all of this in a way where we don't remove the original replicated security guarantee that Bitcoin has, has endowed the space with the other fortunate thing as well, TPS tends to grow quite a bit and network resources also tend to grow quite a bit.

[00:17:21] Storage is still relatively. And available. So we believe that the data scaling side of Cardona will be something that we don't have an urgency to resolve until late 2018 to mid 2019. The research has just started at a university of Edinburgh and we intend to continue it. And we believe we will have our first approaches probably by the middle part of 2018 and eventually have a total solution to this problem by the end of 2019 for the system.

[00:17:49] This is kind of the first component. Let's build a protocol that allows us to scale up the T uh, transactions per second. So as we gain more people into the ecosystem, we get more throughput. Let's create a network stack developed by one of the early internet pioneers that has learned from some of the issues that TCP IPA has and other.

[00:18:11] And is a bit less fragile and a bit easier to configure and tune so that it can handle a large heterogeneous network based upon real life scenarios. And let's come up with some clever ways of handling the use of data in our system without compromising our security guarantees. And also when a partitioning is done.

[00:18:28] So much like BitTorrent, you actually gain a lot more resources for overall storage. So if we don't have to replicate the database, rather we can distribute it. There is some hope that we can build a large distributed, uh, uh, file system for Cordato and thus actually have total available petabytes of data, even though any particular user only has to have a small amount.

[00:18:48] So that's the first pillar, this notion of scalability, but the third generation demands to more and therefore for the Cardinal project, we will do the. First it was this idea of interoperability. So interoperability is this idea that there will not be one token to rule them all. So, sorry, Bitcoin, you're going to have many networks like a theorem and Bitcoin and ripple and legacy systems.

[00:19:23] Like the traditional bank network. Running on older protocols like swift and older settlement networks, like ACH and so forth. And these systems all speak their own languages. And these systems all have their own business, logic and rules. So currently as it stands, it's very difficult for a theorem in Bitcoin to understand each other substantially more so for the old banking networks, which have the added requirement of metadata and attribution to the transactions.

[00:19:57] So the problem is that if you don't have a single standard, and if you don't have a canonical way of communicating with these systems, then you run into a situation where value gets very fragmented. So regardless of how decentralized any one of these particular ecosystems happened to be the king maker will be the small on and off boarding hubs that control the movement of value between these systems.

[00:20:23] Currently, we're seeing those as exchange. But there are others who could come and these exchanges are very Frank. They're subject to being hacked. They're subject to draconian regulation. Occasionally they get shut down because of unwise regulatory policy or in some cases wise regulatory policy. And this is really not a good situation to be in for a supposedly decentralized permissionless ecosystem to have a small group of actors control, whether one can convert their value from one system to another system.

[00:20:55] Furthermore, when people do business in this world, If these businesses are regulated or ease, even semi regulated, they usually do have to interface and interact with the traditional financial world. For example, let's say that you're a cryptocurrency company and you issue an ERC 20 token.

[00:21:17] Okay. So that ERC 20 token, let's say you have a crowd sale and you raise millions of dollars worth of. And as a actual company with a bank account in a legal jurisdiction, you begin selling that ether and deposit millions of dollars into your bank account. Well, then bank is a regulated entity there. And the first question they're going to ask is where did you get these millions of dollars from and the bank.

[00:21:45] Then ask you to, to explain, to provide some, uh, data and details. You'll say, oh, well, I had a crowd sale and I sold an ERC 20 token, and I got a bunch of ether. They say, okay, well, who did you get it from? Who are your customers? And you respond people over the internet. And unfortunately that's really not a good answer.

[00:22:06] Yeah. This entity has a regulated business entity that has to file suspicious activity reports that has to deal with, uh, people on their side, like the treasury department, or maybe a European union and so forth. These entities feel that this is a very risky proposition and this is the unfortunate reality that we tend to live in in our world.

[00:22:26] We have fragile interlinks throughout cryptocurrencies, as well as, uh, the legacy financial system. And there's really no way to escalate transactions in a very natural way so that when one wants to do business with the legacy world, that metadata, that attribution, the compliance information that one would want to have is not present.

[00:22:47] And as a consequence, anybody doing business here automatically becomes a high risk business. This is an unfortunate situation. So the idea of a third generation cryptocurrency with respect to interoperability, It's a cryptocurrency that has the capacity of being able to understand and watch other cryptocurrencies, a cryptocurrency that when it sees the Ethereum and an event occurring here can actually verify if that event is true or false.

[00:23:13] For example, if Alice says she has ether and sends ether to Bob, this cryptocurrency ought to be able to actually know that that's a legitimate transaction. If it's something in the concern of the third generation cryptocurrency. So cross chain transfer. Are reliable and they should be able to do this without needing a trusted third party.

[00:23:35] That's the single most important thing, because we want to create an internet of blockchains and internet of value that flows around just as easily as Bitcoin flows around or ether flows around. We want to move cross chain. So the first component of that is to have some notion of site. No, this is not a new idea.

[00:23:53] Atomic cross chain swaps or side chains. These things have been around for a long time. They've been proposed since as early as 2012, perhaps even sooner. But the basic concept is that there is some way of structuring information. From one chain to another chain, such that when a transaction is sent that compressed structuring of information gives you the ability to know if that transactions legitimate or not.

[00:24:21] In other words, the person sending it to you actually has that value. And also this value is not a double spend. It's a very important concept. The other side of it is that you have to have the ability to do this in a very compressed way. There are over a thousand cryptocurrencies in. And cryptocurrencies are becoming larger and larger.

[00:24:40] So you can't say, well, the only way to understand the other system is to have a copy of the entire blockchain of the other system. This is not a scalable solution. You have to be able to look at these systems and a very compressed way. So Cordato has started its side chains effort. We recently published a paper with Andrew Miller Dennis's syndrome analysis.

[00:25:00] And this paper contains a very well thought out, uh, approach for how to generate proofs in the proof of work world called noninteractive proofs of proof of work. And we're very hopeful that this approach can also be adapted in the proof of stake setting. And then these two things together combined with some clever engineering should allow us to have a pretty deep and detailed understanding of what's going on amongst other cryptocurrencies, which are here to stay.

[00:25:28] However, this is only part of the story. Even if we can create a utopia where all blockchains can talk to each other and be seen and heard, and they go from blind, deaf, and dumb to very intelligent and verbose. The issue is that this world is still incompatible with this world principally because of three factors.

[00:25:49] One is the notion of metadata. Two's the notion of attribution and three is the notion of compliance. So metadata is the story behind a transaction. It's not that you've spent $50 that matters. It's where did you spend it? What did you spend it on? Uh, to whom did you give it to these types of things?

[00:26:15] That's metadata. It's really not well provisioned in the cryptocurrency space. However, it's the bread and butter of the legacy financial world. There's an enormous amount of value in the metadata of transactions. And in some cases, the metadata of transactions allows transactions to be put into a hierarchy of.

[00:26:33] Certain types of transactions are tremendously risky. For example, if there's a wire transfer between two American banks based in New York, amongst large companies, this is very common and happens all the time. If there's a wire transfer from a small American company to a small Russian institution, which in turn, then goes to Iran, which in turn, then goes to South Africa, this is a totally different city.

[00:26:57] Even if the amounts are the same, the amount of hops, the people who've touched it, the nature of the organizations, how long they've been doing business, this is all metadata. The problem is that metadata is incredibly personal. It's incredibly private, and it has a big difficulty in the cryptocurrency space because all the transactions here are permanent.

[00:27:20] They live on a blockchain they're transplant. And the minute that we would attach metadata to a transaction here, we'd run into a situation where we could be potentially exposing very sensitive information to the general public. So what are the goals of the Cardinal project is to figure out where, when and how we can put metadata on a blockchain and benefit from some of the factors that we really care about such as auditability, as well as immutability and.

[00:27:47] Because temporary with metadata is a very, uh, very risky thing. Uh, it's very important in cases to have this, but at the same time, posting metadata to a blockchain in a responsible way, perhaps encrypted or perhaps with a special scheme that only allows certain people to see it. Whereas others cannot.

[00:28:06] Attribution is about identity. It's about the naming. Of, uh, actors involved in transaction. It's a subset of metadata, but it's so important. It deserves its own consideration. It's not just good enough to know the story behind the transaction. You have to know where the money came from and where the money's going.

[00:28:23] That's Alice to Bob, JP Morgan, chase the Wells Fargo and so forth. This is so incredibly important that we've decided to try to construct a way where if one desires to add attribution to a transaction. It can be done in a pretty streamlined and easy way, but the difficulty is establishing a web of trust or some sort of identity hierarchy.

[00:28:49] One of the reasons why we live in an internet with passwords and usernames is because we actually don't have a good way of identifying the people on the internet. It would be great if everybody had a public key and there was an easy way to distribute these things in an easy way to verify. Bob's public key was actually Bob's public key.

[00:29:07] And this was one of the goals of the PGP project. It was never realized as a consequence, the second constellation prize that we've had to deal with on the internet has been this terrible dystopia where one has a username and a password, usually easy to guess, usually easy to hack and usually reuse amongst many different websites and cause a certainly a lot of problems.

[00:29:28] So the same problem there is incumbent. The difference is that cryptocurrencies are factories for cryptographic credentials. They give you a place to store public keys. They give you a place to store, a whip of trust and a whole bunch of cryptographic mechanisms that go above and beyond what one would see in a, in a normal website.

[00:29:50] Cryptocurrencies are basically factories for cryptographic credit. Unlike normal websites are unlike the current internet cryptocurrencies, give you the ability to organize, manage store public keys, and develop all kinds of webs of trust as well as even more advanced layer cryptography, which has been invented over the last 20 years.

[00:30:12] So part of the goal of the Cardinal project is to start exploring how we can use these things that we're currently using for storing and saving our. To actually also identify ourselves when and how we want to do. And the hope is that this can then be used when people are required to give attribution to transactions.

[00:30:34] For example, perhaps when they send value to an exchange or back they can do so in a very graceful and easy way. Now the final component is this compliance component and compliance is a construction of things like KYC, which stands for know your customer, things like Hmm. It stands for anti money laundering and things like antiterrorist financing ETF.

[00:30:56] And basically they're all the same notion of there's a transaction that's occurred. What do we know about this transactions? Such that we can say it's a legitimate transmit. This is something that is not really considered in the crypto world, but it's the bread and butter of every single financial institution.

[00:31:14] Whether they're an exchange, they are a bank or anybody who's in a position to be a money service business, where they're handling money on behalf of somebody else. There's very harsh and strict global regulation and standards for how anti money laundering and know your customer and compliance needs to work in general.

[00:31:30] So with respect to this, our hope is that we can find a healthy. Where once we've distributed these cryptographic credentials. And once we have provisions for metadata, that these two factors can be put together in a very creative way, on a case by case basis and a voluntary basis so that when somebody in the crypto world wants to do business in the legacy world, they have an ability to S.

[00:31:55] The transaction from a standard cryptocurrency transaction to one that a bank would actually recognize and feel very comfortable with. For example, the, uh, scenario that we gave in the beginning of this presentation about this ERC 20 token crowdsale one could entirely imagine the idea of saying that the only way, one consent ether to this transaction.

[00:32:17] Would be, if it's stamped with some metadata accessible to the person being sent to, and it has some identity information, that's transitive such that when they cash out and go to the bank, they can disclose that to the bank. But the key here is doing this in a way that protects privacy and doing this in a way that doesn't necessarily make people custodians of the data, as we've seen with the Equifax hack and other such.

[00:32:44] Custodianship of personally identifiable information is quite problematic. So a big goal of the Cardinal project is to explore this side of the space using new cryptography, using, uh, optional metadata, and also using things like trusted hardware, for example, which give us all kinds of capabilities from very secure ways to store credentials, to the ability to provide guarantees that data has been destroyed after a period of time to things like geotagging, for example.

[00:33:11] So this is the interoperability. And if we're successful with this, we can really think of Cardona is that glue that can facilitate the internet of blockchains where Bitcoin can stay. Bitcoin. Ethereum can stay as a theory and ripple can stay as ripple in the banks don't have to change much, but Cordato provides that necessary bridge that isn't centralized and isn't fragile rather.

[00:33:32] It's a large decentralized. And it really ushers in this great new era of interoperability and the last two sections, we talked about scalability and interoperability, respectively, but the third pillar of a third generation blockchain and what Cardona aspires to be. And probably one of the most important of three pillars is this idea of sustainability.

[00:33:53] And you could break sustainability into two components first there, the idea of how do we pay for.

[00:34:09] so cryptocurrencies are not companies, even if one is to say a cryptocurrency or a token as a security, it's still somewhat decentralized. It's still infrastructure. It's much more like roads. It's much more like TCP IP, their protocols. And so when you talk about a protocol, That's open source. The idea is to minimize the operational cost of that protocol.

[00:34:34] So things like putting tolls on the protocol or intellectual property on the protocol, even if it's well-intended, for example, to fund a foundation are likely to be less competitive than completely open, completely free protocols. So as a consequence, Very difficult to figure out exactly how one ought to maintain these systems, pay for these systems in the longterm.

[00:34:56] So certain proposals such as a patronage type of model, where a corporation decides to volunteer it's developers may work in the short term, but the challenge is that those developers end up having a huge amount of influence over the evolution and growth of this. So one can argue that a patronage model will lead to centralization of power into the hands of a few companies that want to modify the protocol of a certain direction.

[00:35:22] For example, right now the W3C is having a large debate about bringing DRM into the. And we've already seen, uh, the eff resigned from the W3C because they feel that larger companies in that effort are influencing this process towards, uh, the benefit of large content distributors, as opposed to a free and open web.

[00:35:47] Patronage may not be the best way I CEO's are also an interesting way. And they're like a quick jolt of energy. They provide a lot of capital and if there's good governance behind that capital and good people behind the capital certainly can result in the creation of a great product, great protocol.

[00:36:03] But the problem is that an ICO is an indefinite event or continuous funding event. Rather it's a large flood of money in the very beginning to do this. But no matter how large that pile of money is it's finite and we'll eventually run out. So the first thing is can we construct a system that has a treasury,

[00:36:26] a treasury is where a blockchain is able to print money and put some of that money into a decentralized bank account.

[00:36:42] and that decentralized bank account is funded through inflation. So the first, the pioneer, this model was dash. If you look at Bitcoin every time a block is produced, it started with 50 coins per every, a block. And then it decreased by factor of two every four years. And now we're down to 1200. Uh, all of that goes to the miner with the dash model, instead of having all of it, go to the minor, some of it actually goes into this decentralized bank account.

[00:37:12] Then there is a democratic method to vote on funding proposals. So what Bob can do is Bob can submit a ballot to the treasury and then the token holders can have.

[00:37:36] and if is a high enough threshold, if there's a high enough amount of. Bob's ballot will be approved and the treasury will open up and pay Boff. So this abstract model is actually incredibly robust because it has a way of being refilled on a continuous basis. It's directly proportional to the overall influence of size of the currency.

[00:37:57] So as the currency grows, uh, it has more and more resources available, which in turn can be spent to grow the currency. So there's a positive feedback. And also it has a democratic process, a democratic participation connected to the system that allows the stakeholders in the system to start having discussions about priorities, namely, what ballots ought to be funded.

[00:38:19] For example, Bob can say, I'm a developer. I want to sustain the system and submit a ballot. And then Alice can say, I'm a marketer. And I want to market the system and create content videos. And now the token holders get to choose. What do they think is a higher priority? Further development or marketing, or perhaps a scientist wants to write a new protocol to improve the existing protocol.

[00:38:43] Maybe it's a new privacy primitive, for example, that, or maybe it's a bit more security with the network stack or a bit more anonymity with the network stack. So instead of going to the national science foundation or the European union and trying to get a traditional research. Scientists of the future may even be able to use the treasury model to propose funding for research, or perhaps you're an application developer, adapt developer.

[00:39:06] Maybe you want to bring state channels to Ethereum. Under the current model, one has to do an ICO or something along those lines issue in an unnecessary token that really doesn't provide any utility above and beyond what ether provides, but do so to raise capital in order to be able to bring this innovation to the.

[00:39:26] Instead of having that segregating value away from the principal token, the token holders now have a mechanism where they actually could provide funding for this DAP. And that's a really exciting proposition. The challenge, however, is that the construction of such a system is a tremendous endeavor and requires quite a bit of deep thought.

[00:39:45] First off, there has to be a proper and fair voting. Second, there has to be incentives to vote incentives, to participate above and beyond some notion that this system is going to, uh, to be a common good. There's a kind of a tragedy of commons notion. There. Third, there has to be an easy way to submit ballots, but do so in a way where ballots actually the reasonable ballots have higher precedents and priorities over absurd.

[00:40:15] And do this all in a way that's completely decentralized and do this all in a way that is somewhat distributed and it doesn't require a centralized. So a treasury is quite hard. Dash had a first example of it, and they've had tremendous success as a project, as a consequence. So , we are quite interested in this model.

[00:40:34] We think this is one of the single most important things about sustainability because it's leaving something behind embedded within the system itself that allows the system to pay for its own bills. It is, as I mentioned, quite a bit of research, so we've already started the process. We first started examining the voting system and we're looking into using a modification of liquid democracy.

[00:41:02] And then combining that with an incentivized treasury model.

[00:41:12] That we have developed, uh, with a joint partnership with researchers at Lancaster university, as well as some of our personnel that come from Ukraine. And our hope is developed a referenced treasury model. That's abstracted from any cryptocurrency. It's just a module that can be plugged into a cryptocurrency such as the theory of classic or Cordato.

[00:41:29] The hope is that the system will have a fairly sophisticated way of balancing the needs and incentives that token holders, as well as the needs of those seeking funding and a reasonable. Now, this is an inexact science. It's one that requires quite a bit of iteration. And this is why we're trying to construct this system in a modular capacity so that the treasury system can be upgraded independent of the protocol itself if necessary.

[00:41:54] So this is something we're very excited about. We should be publishing a paper fairly soon, PR in quarter four of 2017. And our hope is to roll out the first generation of the reference treasury model into the Cardona protocol by about the middle part to the end of 2018. Depending upon how long the research takes, but there's another side to sustainability.

[00:42:14] It's not just about how do we pay for things. It's also about where should we go? And this is an even bigger meta question.

[00:42:34] So. Cryptocurrencies are living creations. They're not static in that. Once you've written the code it's finished, it's done. There's no notion of 2.0, you have to be able to change them. As technology changes, use cases, change or new innovations come out that you can benefit from tremendously. And generally you do this either with soft works or hard forks, but.

[00:43:06] These are forks, nonetheless, meaning that you have to change something. The problem is that in current cryptocurrencies generation one and two, there is no canonical way of deciding which fork is proper. Amongst many that have been proposed. And as a consequence, this results in a situation where eventually irreconcilable differences develop and we see the chain break apart.

[00:43:33] We seen this with Bitcoin and Bitcoin cash. We've seen this with a theory and Ethereum classic, and it will only continue as these systems grow and scale and value. So what we have to do is argue by analogy. Are there any social systems that humanity has constructed, which while they may be controversial, have still maintain a degree of stability and update ability.

[00:43:56] Constitutions are the closest notion that we have. That's the highest law of current. Uh, constitution doesn't change too much, especially constitution like the American constitution. And there are somewhat difficult to change, but when they do change, there's universal consensus post change that they're going to follow this.

[00:44:14] We don't see a fracturing of the country to, to Americas or to UK or something like that. Kind of get consensus around it. Why? Because it's a slow, deliberate process. One that people agreed to follow, at least in principle. So if we were to treat protocols as constitutions, one ought to be able to amend the constitution, one ought to have a process to do so because we're engineers and we like reusability.

[00:44:43] Our hope is to use the very same types of mechanics that are used in the treasury system for approving. To actually being able to consider Cordato improvement proposals.

[00:45:04] so Alice or Bob, the developer can propose a sip and then there's going to be a process which Alison Bob can follow that allows the network to vote on whether this should be ratified or not. This should be a slow systematic, deliberate process that takes time and effort with increasingly higher thresholds prior to eventual adoption.

[00:45:29] Now, the first generation of this technology is more about process and mechanism. It's a Metta consideration that lives outside of the network, but relies on tools within the network. For example, the ability to do voting by stake weight. Later versions, we're going to Explo explore the idea of converting a Cardinal improvement proposal and to something that's machine understandable.

[00:45:59] similar to a formal specification of a protocol. There is this notion that maybe we can actually specify a cryptocurrency in a way that the cryptocurrency actually understands its own. If this is possible, then it may be possible to actually verify if a client is following a specification. In other words, when Alison Bob created their wallets to connect to Cardona, there's this machine understandable canonical notion of how Cardall ought to be configured and their clients will actually be able to self accredit and verify if they're actually following the protocol or not.

[00:46:37] So this is kind of generation two and three. This idea of taking a social process and eventually mechanizing that social process in ways that give us a protocol that lives above the particular software. And we're very hopeful that we can use, uh, emerging techniques from programming language theory and formal verification to pursue these ends.

[00:46:58] So the first micro examples of this are going to start materializing with the formal verification of smart cars. Which is a very important topic for reducing bugs and ensuring that smart contracts are stable and reliable. And this is an area of research that we're pursuing very vigorously at IHK. And we intend on having several publications come out throughout 2018.

[00:47:20] Our hope is that those techniques can then be raised a level and we can begin having protocol level descriptions of how Cardinal ought to work as a full cryptocurrency stack. And then eventually we can pursue a formal verification that clients are pursuing are connected to a specification in the short term.

[00:47:40] The Cardinal improvement proposal process will be completely written up by quarter one of 2018. And I, which K will begin following that process as it upgrades and iterates the Cardinal protocol. And once our treasury voting system is in place, we will make special accommodations so that every Cardinal improvement proposal can eventually go through a process of voting with higher rigor on hard forks and less rigor on salt.

[00:48:06] But nonetheless, there's still some notion of this. We already have an upgrade system built in. If one goes to Cardone docks,

[00:48:16] there's a specification on Cardinal docs.com for how that system works. Uh, and later on that system will be superseded by our new voting system that we intend on rolling out with the treasury. So this is sustainability and that. It is our view on how we should responsibly pay for things and our view of where should we go as protocols start.

[00:48:38] There's usually a lot of founder vision and a lot of initial philosophy, but as more people come into the ecosystem as more hopes and dreams get invested into the ecosystem, eventually these ecosystems grow beyond their founders. And so it's incredibly important to have a process for changing the protocol at a very slow, deliberate, methodical way.

[00:48:57] That's as inclusive as possible. And as resistant as possible to any particular power brokers ability or machinations. So that's Cardinal, Cardinal is a third-generation protocol. It's built with peer review. It's built with high assurance software standards. It's built in Haskell my favorite programming language.

[00:49:16] It's built by a large international team and are very well-funded and I, which case committed to it until 2020. And it's built to be sustainable interoperable and scale. Our view of how do we get cryptocurrencies from the first million to the first billion. Thank you so much for watching. And I hope to hear from you guys soon.

