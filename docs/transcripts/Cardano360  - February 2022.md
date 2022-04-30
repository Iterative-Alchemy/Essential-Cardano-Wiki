# Cardano360 - February 2022

[00:00:00] Welcome to the February edition of Caledonia 360, your monthly catch-up with the people and projects building out this incredible Cardona ecosystem. Now, before we begin, make sure you like subscribe and hit that bell for all the latest Cardona content and the latest news from the team here at IOG. Now later in the show, we'll be checking in with project capitalist.

[00:00:34] We'll be taking a peek into the metaverse and meeting a few more of the projects building on Cardone. We'll meet Eric and Daymond from the Cardona defy Alliance. Plus Coty is joining us for a quick update on jet, but before all that it's time for our regular development day.

[00:00:51] Gentlemen, thank you very much for joining us again this month. Now of course, at the moment, the team is very busy preparing for the next major release. We did a bit of a deep dive on this in the mid month update, but John, perhaps you can give us a reminder of exactly what is going into the next release.

[00:01:05] There's a number of things coming up in the February release, which are, which are quite exciting. Some of them are quite techie. Uh, others are, are more user end users. Uh, when you're, when you're running a computer application, of course, there's lots of data floating around in the computer's memory and how we represent that data or how it's structured inside the computers memory, as it can be done in different ways.

[00:01:22] What we've really tried to do is slim down how we represent data in the running node. And this has the ultimate result that for folks who are running data lists at home or running a node at home, they'll require less Ram to run the node because we've been able to really make more efficient optimizations on the structure of data in Ram.

[00:01:40] So this means that ultimately the node is less resources. And demands less of the end user's computer. So this is a good thing. So now that it can actually craft transactions in the CDL format, the concise data definition, language, this is something that's going to reduce friction for folks. So now that you can actually add quickly from our CLI using our standard, uh, native tools that ship with a node, you can craft transactions and the CDL format rather than relying on third-party tools.

[00:02:05] So a bit of a tricky one, but I think useful, nonetheless, and we've had multisignature is already this idea that you can have a number of entities sign-up transactions rather than one person sign with their private key. You can have many people have to sign with their private key analagist to a joint bank account, but we're rolling out a, a modification here so that we can effectively sign a transaction in incremental stages.

[00:02:27] So for example, you might sign the transaction first and then send it over to me and then I'll be able to sign it rather than having to sign it together. Well, we now have a new tool, so the SBOs can check, uh, the leadership's schedule now that you should schedule it is. Basically a list of who's going to produce blocks next.

[00:02:44] So this enables FPOS to review the next epoch and know ahead of time, who's going to have that leadership spot in like the block. Now I understand some folks might be concerned about security. Well, the way this has been executed and SPO can only check on their own upcoming schedule and not on others.

[00:03:00] So this has no impact in terms of security. We've also added, and this is really a developer level feature. It lets developers inspect the local men pool were transaction sit before they'd be put into a block. It's kind of like a waiting room for a, for a block. This allows developers to kind of look at the mem pool, follow the process of a transaction as it slowly gets towards, uh, being an, a block.

[00:03:19] This is ultimately something that developers have been asking for for a while. So we think it's going to really reduce friction for devs. And I think what's really cool here is that a lot of developers have said, well, when I'm writing smart contracts or writing validation scripts, um, I don't know exactly how much resources I'm using and I've spoken about the resources before I'm blue, this okay.

[00:03:37] Memory limits, CPU limits, they're important. So you have to, when you're crafting your transactions for Plutus, you gotta be aware of these things. And, uh, this CLI command or command line interface tool will allow developers to know exactly how much resources they're script is, is expected to be used. Uh, when it's executing.

[00:03:54] And then finally we're going to be increasing Pluto's resources and the number of transactions per block. So I want to recap what some hard numbers on this. Since the start of this year, we've made blocks 25% bigger. We've allowed through the scripts to use 24% more resources on a pair block level and 40% more resources on a per transaction level.

[00:04:15] So these are real, tangible changes. These are big, chunky changes we've made to layer one since the start of this year, Nigel, we've already talked about how we're grouping the releases this year around three points of the year. Now this is more about predictability than anything else. It is. As we've grown, we've got a lot of, uh, dependent of companies within our network and infrastructure.

[00:04:37] So it's about enabling these different partners to have greater predictability about when we're going to do a major update and a major release. And it helps us to do the coordination about leading up to these different. It's about grouping these different features into one major release. Nevertheless, if something does miss those different segments, it doesn't mean that we have to, we can't release at other dates.

[00:05:03] And so throughout the year, we will be doing incremental updates across our whole technology stack. And I think it's important to note that in some of these features, they don't necessarily need a hard fork. So if we coordinated a major release around the hard port that enables partners and other community members to actually manage their own, uh, development activities, but also we can give incremental updates that aren't a mandatory upgrade path throughout the rest of.

[00:05:32] Now Nigel is John outlined. The focus of the February release is of course around the core platform capability with a number of Plutus enhancements as well. But of course, there's going to be a number of other drops throughout the year. We've, uh, we've talked a lot about the major releases and having those around fixed dates to create greater predictability outside of all of that, there's a huge volume of activity that's going on around delivery areas.

[00:05:55] And within Eastern every area, there are some major deliveries releases and different features that are coming out. So I'll introduce now some of those delivery areas and give you a little bit of a flavor of what's coming up. So within our core technology delivery area, it's our major infrastructure delivery area.

[00:06:11] We've talked a lot about that. There'll be continual performance updates. We'll continue to update our promises to great greater network performance and efficiency. Outside of that, we have a major release coming up within the next few months, which is our UTX own HD pro. Where we are looking to basically change the way that actually we store the whole ledger state.

[00:06:34] So it'd be a mixture between Ram and a hard disk drive for different users. That's a huge advantage because it enables us to cope with a massive increase in network utilization and the growth of our UTX owes in our account structure. In addition, we still have the peer to peer work, which is about introducing a dynamic typology to our network, to enable all our network nodes and peers, to be able to efficiently connect to each other.

[00:07:04] And this is another part of the path towards full decentralization. That's been on the Testnet since December, we're looking to increase the testing on that drought this year and releasing that onto the main net outside of that, there are smaller things that we are doing, but nevertheless, they are equally as.

[00:07:22] We are continuing to look where we can get more bang for our buck within different performance optimizations. And we are working to actually optimize some of the libraries that we have that actually run out in that work. So that, that just gives you a full flavor of the infrastructure delivery area.

[00:07:37] The core technology sitting on top of that, we have an application layer delivery area, which is our smart contracts area, which is where is the key direction where our community's building. So inside of that area, we have a project, uh, about Plutus certification, which is basically our Kadana assurance program for us to be able to do some reading mentoree checks on the different dApps that are hitting our network and get greater assurance to our users.

[00:08:06] Which is, I think something very important for our users going forward and also helps our adapt partners to inside of that. We've set up a whole process around community support. So we are listening to our community and our developers engineering teams, and we're trying to provide tooling and use cases to those guys on a continual basis, we have a team that's working on those things and then delivering those support on top of that, we've supported the setup of different organizations on the network.

[00:08:36] One of which is the Alliance and we've set up a process out. They themselves will actually develop tooling and different, uh, components and features that are really helpful for DAP DAP engineers. And this comes from firsthand experience of building things themselves. What we've just agreed with them is we'll make sure that whenever we deliver anything, it has actually tested with an adapt and then is used in adapt when it hits the network.

[00:09:04] And that. Our quality as we move forwards. I know those guys are coming on later on the show, um, to, to talk at even greater detail. We've also got a lot of work going on in our Basho area, which is all about the, the next generation performance technology. Hydro we've already had an update on that in the mid month.

[00:09:24] It's allowed to technology. We've also got some work with an, a leading edge area with our project called Mithril, which is about sinking to the, the network faster. And in addition to that, we have a large program of work on side chains, and that itself is also going to be a massive network improvement because it enables execution of, uh, contracts and application transactions outside of the main network moving forwards.

[00:09:50] You've already seen this year, lots of updates across our wallets and services area. We are continually trying to improve our existing products, whether it's dead less to introducing more interface changes, as well as improving the sync connection. They're looking to actually build forwards and actually develop a voting sensor and also an at T center.

[00:10:12] In addition to that, we've got the Caetano wallet, which is building on the multisignature technology and features that we're just about to roll out that, which John's just, just talked about outside of that, there's going to be some even more brand new features coming online. We have an exciting DAP store.

[00:10:29] That's going to be introducing as a beta release to a smaller community at first, but that's going to be a cornerstone to parts of our application layer and smart contract offering as we move forwards. And then finally, we have a large amount of work within our governance area, which is where we're looking to continually improve decentralization and introduce community committees to make decisions across our whole network.

[00:10:57] Now, in addition to that, within that area as well, What are the core features and as catalyst and catalyst, we'll continue to roll out different funds and support the growth and the investment within our network. So I think, I think team that just gives you a really good flavor of just such a vast amount of work that the whole community and team are working on it Kadana well, thank you Niger.

[00:11:22] Yes, of course. A huge amount to deliver during the rest of this year. And of course, we'll be jumping into some of those areas in future shows, but let's go to June. Now. We obviously are going to cover this in great detail in future months, but one of the areas that is kind of most important and getting the most excitement, John is pipelining.

[00:11:38] Perhaps you can remind us what that is and why that matters. We need to make sure that as we make things bigger, better, we also make things faster. Okay. Making things faster will allow us to make more of these changes as we progress throughout the year. That's where pipelining comes in. Pipelining is making things faster so that we can continue to aggressively scale out the size of blocks and aggressively give more resources to Plutus.

[00:12:03] So what his pipeline touched on it before, uh, technically it's the coalescing of verification of blocks and propagation of blocks, but what does that mean? It simply means that nodes in the network no longer have to do a full verification of a block before they pass it to their neighbor. And instead we have a mechanism where, where the nodes can safely transmit blocks to each hitter before full verification has taken place without jeopardizing the security of network.

[00:12:28] All of this comes together to do one thing, give us more headroom to scale car donno, faster and better. Um, between now and June, we have plenty of headroom to continue to grow the scaling properties of, of. Pipelining is really going to be a major milestone in terms of giving us huge headroom in, in scaling out further.

[00:12:48] John, one of the technical improvements that we have discussed in the past was Plutus script compression, but I understand that's not needed anymore. Eyebrows Twitter. I browse Reddit. I browse YouTube and I've seen folks ask questions about this. And I don't think it's been addressed recently. We were looking at script compression as a technique to squeeze more scripts into blocks, but this was before we had bigger blocks and more memory units available to scripts in general.

[00:13:09] So it's simply not needed anymore. Um, if we did do script compression, it will be an extra step in the process. It will be something that, um, we would have to change the structure of the chain for, because now scripts would, would be in certain areas on compressed and in later areas compressed. So it's just not an optimal solution and we've decided that we're going to move forward without it because things like pipelining and input endorser's basically makes it, make it up.

[00:13:35] Thank you, John. So Kevin alongside pipelining as network level improvement, there's going to be some improvements to Plutus as well, particularly around three CIPS that are particularly important to our developer community. Perhaps you can tell us more about those CIPS and why they matter. Absolutely. So the Plutus team is on fire at the moment.

[00:13:56] They're really. Through the improvements here are great things happening that will really benefit the developer community, reducing the friction for developers, uh, enabling more sophisticated Diaz to be developed, but also as John's hinted at, um, improving the capability to change process these transactions and all of this is happening in conjunction with discussions with, uh, community members via the open CIP process, uh, that allows us to talk to the community, to propose our ideas, to get feedback on those ideas, and then to put together the best possible solution that we can for whatever the technical.

[00:14:36] Happens to be. So you've mentioned three CIPS. The first of these impossible, most significant for many people is that we will be making our Plutus transactions smaller and cheaper, and what we'll be doing to enable that is the ultimate in compression, John. So we're not just reducing your strengths by 10%.

[00:14:58] We're not reducing them by 20%. No, no, no, no, no. We're going to reduce them down to a fixed size. What we're going to do is to stall the scripts on chain so they can be. So a stretch will be a few bites are on chain. You'll be able to refer to it repeatedly. That means you won't have to pass that script in every transaction.

[00:15:19] That means the transaction sizes for Bluetooth straps will go down from the current figure, which is about, um, 16, 14, 16 kilobytes. There'll be dramatically reduced. I don't want to say exactly where we're going to go to, but exact to major change there. And because the cost of a transaction is based on the size because the strip sizes will have reduced.

[00:15:41] That means that, um, the users will be paying much less ADA to run their scripts. That's going to be a win, win, win all around. When there, this is CIP, uh, 36. Uh, then in addition, we're also going to be improving concurrency. This is one of the concerns that people have had when developing D apps of, because of the UTX own model.

[00:16:06] And what we're going to be doing is potentially something called reference inputs, CIP 31. And what a reference input will do is to allow you to refer to a transaction input without spending it. So that allows many different transactions to refer to the same input. So each of them can use the same value each of them can run concurrently, and that will help dramatically with removing one of the major source friction that people have felt.

[00:16:35] So. In addition to that, um, other things that are coming along, uh, will allow scripts to share our Regina so that we able to cooperate better using particular pieces of information. And we will also allow scripts to directly reference data. So at the moment, we're having to hash data values to pass into scripts and that's appropriate in some cases, particularly where the data is large.

[00:17:01] You can just refer to the hash, but if you've got something which has, for example, simple integer, that's perhaps overkill, especially if you don't want to keep it secret. Um, so by providing simple data and values directly with the scripts, sip 32, we will then, uh, cut the cost of accessing those data values and also make it easier for people to see what data is being provided to the scripts.

[00:17:26] So that's, these are great improvements. You mentioned the CIP presence several times, but we're also of course, pulling a lot of content are from a number of people who are actively collaborating with us by get up and your input there. Guys, very, very important helps us to keep rolling out these improvements.

[00:17:46] And the input from community members input from the Cardone defy Alliance is really making polluters much, much better. So lots of things happening to him. Great days ahead for polluters. So gentlemen, thank you very much. Lots of exciting things happening over the next nine to 12 months. And of course, we'll come back to you in future shows and we'll do a deep dive across all those topics.

[00:18:07] And we'll introduce you to a few more of the team behind them. Project catalyst is showing no signs of slowing down with new funds, providing millions of ADA to ever more projects, innovation, sparking ecosystem growth, and the continuing road to decentralized governance Encore, dyno. Eric spoke with project catalyst, Chris Baird to get the latest.

[00:18:32] So today we are joined by Chris Baird, the product manager for the catalyst ecosystem. Welcome to the show, Chris, thanks for much Jerry. Great to be here. So it's been a little while since we talked about project catalyst, uh, what are some of the updates since last we chatted, we've just concluded the voting and announced results of funds seven and what a great turnout we had over a thousand proposals submitted in just fund seven alone.

[00:18:57] And that has produced 269 new projects. Meaning that overnight we've almost doubled in the number of projects that Casper supported since the Dawn of capitalist time. What it means in some other practical terms is we've had a lot more wallets that have registered to vote. So now there's been over 52 and a half thousand while it's the registered to vote in fund seven, which.

[00:19:24] Over a quarter of a million votes, which means that since castless began a little more than a year ago, over 1.1, 5 million votes have been cast, uh, to help decide which projects should be funded by the Cardona treasury, which I think is just mind blowing. When you think about where we've come in a year, that is absolutely incredible.

[00:19:46] So, uh, obviously we have done the voting for fund seven and we're moving on with fund eight. Uh, what are some of the things that are different about fund date? What can we look forward to quite a lot to what we look forward to that's for sure as has been the conventions since, uh, the first amounts of ADA were made available in fund two, we've doubled the fund amounts in size, every single funding round.

[00:20:11] So. Uh, with fund seven, we had $8 million worth of ADA available in fund eight there's, $16 million worth of Baylor up for grabs. Now this is going to be distributed into a 22 challenges and all of these challenges have been set by the community so far. And, um, you know, if we double click and drill down a bit further, $2.2 million worth of ADA is going to be spent on two challenges to grow our developer ecosystem.

[00:20:43] Uh, there's two challenges that are focused on self sovereign identity and accelerating decentralized identity. So that's, uh, a great way. And I think for the Tyler prison team, and we've already seen a lot of great outputs from, um, their challenges, uh, in previous rounds and there's, um, both a million, four Caetano scaling solutions.

[00:21:05] Another challenge around the great migration, uh, from a theory from so supporting projects and dApps and whatnot that want to move over from Ethereum into the Caetano ecosystem. And then I'm really, really pleased to see that there's, um, there's two new grow card Arno challenges. So you might remember we've had grow card Arno grow Africa.

[00:21:25] That's now been reinstated for funding. It was voted forward funds a fund seven. Um, but we're seeing a new additions with grow Caetano, grow east Asia. And for the first time grow, Catano grow India. So I couldn't be more excited for that. Also open standards and interoperability is becoming a bit of a theme and there's a real new novel challenge, I believe, eh, which is called film and media creatives unites.

[00:21:53] So I think the way that I see is that there's just a lot of growth in all dimensions. And there's hopefully going to be new communities, both internationally and, you know, by sort of industry that are going to be being exposed to Cardone and project costs. Wow, this is incredible. So we've got not only some new challenges that are coming up, but a new challenges that are sort of pushing into new territory at the same time.

[00:22:19] What are some of the new themes in projects that you're seeing coming out? Yes. Well, I think, you know, another thing to point out is that there's a growing interest in this new initiative that we've launched called catalyst natives. And so, so just to touch on that, um, if you haven't come across catalyst natives so far, this is about taking all of this great energy and momentum and community that has been built through project catalyst and allowing other projects outside of our ecosystem, to be able to allocate a treasury and set challenging.

[00:22:52] Um, that, you know, the project costs is community and our broader Cardona community can take a shorter. So, you know, the, the idea is how can we enable more blockchain innovation that uses our, uh, community and leverage his or their expertise. To help solve problems for other sorts of stakeholders. So yeah, we're having these sorts of conversations there, you know, there, there are going to be new Cassis natives coming to the fold very, very soon.

[00:23:19] So that's one certain emerging trend that we're seeing also, you know, the, this, this new found, um, interest in regional support. So doubling down on a particular international territory and funds seven, we've seen a number of Japanese focused projects, supportive, uh, including a really exciting Caetano Tokyo summit projects.

[00:23:40] So, um, we should be growing these local communities even more so, um, we've seen 20 projects funded under the grow. Uh, Cartano grow Latin America, uh, challenge. So, you know, again, there's all of this momentum and community that are building in these local international settings. I also think that this, you know, Uh, some, some new and emerging themes that are beginning to take shape for, you know, spaces, which may be haven't necessarily had a lot of blockchain innovation take place in them.

[00:24:14] So what I'm actually talking about is in fund seven, we've seen three education and EdTech focused projects just in the grow Latin America challenge. So, you know, these are projects that aren't just about. Did you decentralized or digital identities? It's not just about credentialing, but it's creative applications like plater earn and learn models.

[00:24:39] So you can sort of see that there, the blockchain innovation space is now begin to become a bit more pervasive into those more traditionally conservative or reluctant to adopt innovation type spaces. Let's talk a little bit about taking it to the next level with these startups. I know that a lot of the project catalyst participants have been working with business incubators to help develop.

[00:25:03] Uh, can you talk about how that's changed, uh, the outlook of some of these projects? Uh, we can identify that. Internal incubator programs that have been established over the course of the last few months. And now we've fund seven and the catalyst accelerators and mentors challenge for the first time we've got the cut on in treasury that is beginning to fund a whole load of new accelerator and mentor projects.

[00:25:30] We've also been working really closely with the target prison team and the premises pioneers team to provide pathways. Into the pioneers programs. And, you know, particularly for the atalla team, we've seen 22 projects that are funded in decentralized identity challenge in fund seven, many of which, uh, started their lives as participants in the toddler prison pioneers program.

[00:25:54] So we saw this sort of symbiotic relationship between the sort of incubator projects and then those teams that are now being successful in submitting proposals into catalyst. Now, once they're in catalysts and they're being funded by the treasury, well, really that's just the start of their journey.

[00:26:12] We've got the catalyst boost camp, which is all about developing really strong entrepreneurial foundations. So it's helping those participants that are often baby startups. They're at the very start of their venture building journey to understand that the real principal, um, components of what makes for a good business strategy.

[00:26:33] So thinking about. Are the reason their motivations were getting involved in the first place, setting up this business, what the problem is that they're responding to, um, who's their audience trying to find product market fit and then developing, um, key objectives and results as a result of that. So the boost camp is, you know, a starting point, it's like a first platform for some of the startups to be able to go through.

[00:26:58] We've also recently launched the IO incubator, which is for Africa focused projects and that John O'Connor and I have been working on for the last few months, and we've seen nine ventures that are just beginning their, their first, uh, IO incubator program. And then coming back to this idea of, uh, the, the catalyst challenge for fund seven centered around accelerators and mentors, we've got 12 new accelerator and mentor.

[00:27:26] Um, what this has really been set out to achieve is to develop like a co-creation process for these incubators and accelerators and mentors, to projects, to work quite closely with us within the catalyst team, and then start delivering impact and supporting the startups that are coming through. What I think it really boils down to is it helps the startups and the businesses and the project leaders that are involved in all these projects and taking advantage of these opportunities.

[00:27:56] It offers them a better way of understanding what they need to do to become investible and not just investible from a traditional VC sense, but also, you know, in, in the. Um, new sort of crowdfunding sort of dynamic. You've got to be able to commit to communicate your ideas clearly and coherently to win the hearts and minds of the people that are hopefully going to be investing into in the future.

[00:28:22] Whether that, as I said is, um, traditional venture capitalists or investment funds, or, you know, even customers right there, the blockchain landscape is, is quite difficult for people to understand, um, if it's quite new to, to, to, to them. And so, you know, I think these accelerator programs are really there to help refine the ways that these startups communicate their value proposition.

[00:28:46] Chris. Thank you so much for joining us. This is a lot of incredible work that's been going on since last week, talked with project catalyst. Uh, so, uh, how do people get involved? Well, the first thing to do to get involved is, uh, come to a town hall. We, we have town halls every single Wednesday, uh, 6:00 PM UTC.

[00:29:07] You can sign up via a zoom link. So if you go to telegram and you search for project catalyst announcements, you can join the telegram group. So you'll never miss an announcement around project catalyst. We also broadcast live to YouTube on Wednesdays or recommend anybody. That's got an interest or a great idea to come and join town hall and to collaborate and meet with all the other great people that are in the community that are showing up every single week and taking advantage of these opportunities.

[00:29:36] And then, you know, the, the, the other final thing to say is, you've just got to take, take those first steps, get involved. Put in a proposal or, you know, become a community advisor, start reviewing some of the proposals that are being voted for on the ballot, or just take an active interest in those proposals.

[00:29:53] As a voter. There's so many different ways to get involved with catalyst and it's a really, really inviting and welcoming community. So a come join us. And as always, all of those links will be listed in the metadata below Chris. Thanks so much for joining us. We last heard from shaft bar Geffen, Coty CEO of the car summit, where he announced his company's stable coin project for Cardona Jed.

[00:30:20] Eric caught up with should have to get an update.

[00:30:26] At the Guardado summit, Coty announced the creation of the Jed stable coin. And today we are going to talk with Shahaf BARR, Geffin CEO of Coty group, and find out a little bit more about the project. Welcome to the show. Shahaf thank you for having me great to be here again. So shutoff, many of our viewers are familiar with Cotea, but maybe you can give us a quick intro.

[00:30:48] Well, one is Cody. Uh, we've been around since 2017. Cody is a little one for payments, but it's more than just little one. We are fully encompassing financial ecosystem, uh, Christy stud of wallets, payment, gateways, even debit cards and banking. And everything that we do and the rewards, the upside of our ecosystem is funneled to a treasury, uh, where our users can enjoy, uh, great rewards, my, uh, participation.

[00:31:16] Uh, we've been in relationship with Cardinal a few years now. And, uh, I've been the first investment that C funds the Cardinal ecosystem. Uh, so at the Cardozo summit, you announced the creation of the Jed stable coin. Can you tell us a little bit about the stable coin and maybe let us know where the project is right now?

[00:31:35] And the Alaska Dano summit just, uh, actually invited me on stage and we announced together the creation of Jed and Jed is a stable coin that is based on, uh, very advanced algorithmic design. Uh, it uses smart contracts to ensure price the visualization and the coin will hopefully be the biggest one in the Cardinal ecosystem.

[00:31:55] So it will be very useful for decentralized finance, operations and everything else that requires a stable. It's it's, it's more than, than just that down the line. You know, that there is a belief that that fees should be paid with a stable currency, obviously to give, uh, the users, um, a way to predict what they'll pay.

[00:32:18] And we believe that, uh, down the line, all transactions fees should be paid with, uh, with a stable coin and is a very good, uh, use case for that in terms of, of where we at with, uh, with a jet that the design is obviously ready. Uh, it has been, uh, an ongoing project for more than a year now, uh, where we at right now.

[00:32:38] So we are finalizing the complete user experience, the front end, and then the integration to the, to the back end front end is, is almost done, uh, including implementation to NAMI wallet and so on. And we're now starting to integrate to the Jed, uh, contract. The design has already been, been implemented in various networks just to make sure that everything is working properly.

[00:33:04] And what we're focused on right now is actually security. Uh, we're introducing, uh, quite a lot of new security features to ensure that jet is secured for, uh, the ecosystem. And for everybody that is using this, what it means is that we'll be probably going to test it, uh, next month and in March, uh, then do a third party audit and then go back.

[00:33:29] In a matter of, you know, six to eight weeks past this and that, uh, just to make sure that everything is working properly as it should be for what will become one of the biggest stable coins out there. So what specifically brought a security to the focus for you? Uh, for Jed right now? Well, first of all, security has always, always been the top priority.

[00:33:51] Cryptocurrencies as a whole is a confidence based market. Uh, people need to trust what they're using because there's no third party that mitigates it for everybody. Um, as the centralized system work, you need to have trust in the, in the system. So securities by all means stop already. Uh, anyway, and especially when it comes to two things that are financial instruments like stable with that in mind, there's been a few weeks ago, there's been a major hack in.

[00:34:22] Um, a bridge that connects Solano to Ethereum, and that brought up a lot of vulnerabilities, you know, a set of things that we can do to make sure that we are more robust in terms of, um, of design specifically. Uh, the security measures that we, that we've added, um, is the introduction of configuration management contract that will facilitate, uh, the upgrades to the Jedi contract without altering the Jed, uh, meeting policy.

[00:34:50] Uh, this suture is essential to ensure that stable court. And reserve coins, uh, in circulation can still be redeemed after an upgrade. And we are performing an extensive property-based testing to guarantee the preservation of jet stability properties in the absence and the absence of security vulnerabilities.

[00:35:08] I level two audit certification of the on chain code to ensure that the mitigation that is put in place are sufficient to cover all potential security, floods, like double satisfaction problem and, and so on. And lastly, we are restricting the invocation of the pop end points responsible for deploying, uh, upgrading and the termination of Jed instances.

[00:35:29] Only, only to a list of known public key hash. I get that most will not understand, uh, all of it. Uh, but, uh, these are upgrades to the contract and the design and the architecture that just allows us to, you know, sleep better, knowing that we've done everything that. To ensure that Jared is secure, that will not be hacked.

[00:35:53] And once you've finished all of this, and once jet is fully launched a where will you see it being used? Jed we'll hit the ground running. We've been working relentlessly to build a lot of partners. Well Jed, so that once launched and again, marches Testnet and if all goes well through the security audit, then six to eight weeks later, we are out there and there's already, already a very warm acceptance for jet.

[00:36:21] So the list of the non exhaustive list of partnerships around, uh, for a Sunday swap will have Jed in its decks, ADA swap Eric codex, uh, DOE ex mere swap indigo Addax world mobile Erebus hokum. So that's just, uh, maybe a short list, a non-exhaustive list of all the partnerships in line. So when Jedi is out, it's already fully encompassed in the ecosystem.

[00:36:52] And, you know, I believe when I think a lot of people understand. That you know, Jed for Cardinal defy will be what, uh, maybe USB-C is for the theory of, and I was wondering, could you tell me a little bit about Shen what is, what is the, what is Shen first of all, Shen is the reserve coin, uh, that, that bundles with, with Git.

[00:37:16] So that is the stable coin. And shin is the reserve coin that is used for the pegging mechanism, uh, as algorithmic stable coin, uh, does, uh, just in terms of terminology, Jed, and that's the proper way to pronounce the debt comes from, uh, ancient Egyptian, uh, as a sign of stability and Shen, also comes from ancient Egyptian.

[00:37:38] Uh, and it's a sign of, of, uh, of loosely translating, uh, of, of prosperity because that's what reserve points are they fluctuating in value. Uh, and when people add the. To the Jed smart contract, and everybody can add liquidity to meet Jed stable coins. Uh, but you need to be white listed to me to reserve coins.

[00:38:04] Um, uh, this is what you get. And we already in touch with a lot of liquidity providers, indirectly system that will provide liquidity and have Jed and, uh, and shin with. Wow. So lots of things going on from Coty. Uh, any parting thoughts for the community that's watching right now, please continue to, to follow up, uh, what we do, you know, please follow the channels.

[00:38:26] Um, you can obviously follow her if you're watching this, you're already following. Uh, Twitter, telegram, this score, whatever works for you, and we'll keep you informed with everything that we do, and we're all going to make it. And as always, we'll have all of those things linked below. Thank you so much for joining us.

[00:38:49] Looking forward to seeing the full rollout of Jed. Now, if you're enjoying this update on what the catch, all our videos, as soon as we push them live, please make sure you like subscribe and hit that alert bell. Go on. Thank you. The metaverse it's been one of the biggest stories over the past six months and seems to be getting bigger and bigger.

[00:39:14] So what is it and what does it all mean for Cardona?

[00:39:21] So let's talk about the metaverse at the moment. It seems like this is going to be a version of cyberspace where individuals can interact in virtual and augmented reality, basically entering the matrix, but we're not quite there yet. Are we? No, we are at the point where we are building the foundations.

[00:39:38] So the question is why does IOG care? So we care about building cutting edge technology for developing countries, as well as emerging realities. Like the metaverse. So today we are joined by chief technical officer or mom Pellerin. Who's going to talk to us a little bit about how Cardona is going to interact with the metaverse to begin with.

[00:40:00] Ramal welcome to the show and what is the metaphor? The meta is that grew between different, uh, universe. I think that's the best, uh, definition. So for example, melanoma is one universe today, a universe where people are connected in, into a global community and they are working towards a particular objectives.

[00:40:25] And you have different applications between, uh, developed, um, Italia is another, uh, universe. Uh, Facebook is one other universe. Google is another universe. So, uh, the metaverse is the connection of those you universe. And in order to connect universities, you need to actually have, uh, interoperability standards, uh, define.

[00:40:50] So you need, uh, data, and this is what we call the NFCS and FTEs are represented in different, different. On different universe, right? Then you have how you attach an identity to those NFTs because you have a owner, right? And that owner is pattern of one or more community. So you need to be able to have a decentralized identity that Arabs attach a user to NFT and, and, uh, that attachment being seen on different, uh, universities.

[00:41:22] And after you have to, to be able to evolve NFTs in the same way you need to attach, uh, ontologies, you need to, uh, to a particular line of T in order to, to understand in what context was developed at NFTE to attach it to another context and maybe reuse some, some part of the previous context you need to ever whenever.

[00:41:44] Uh, in time also between different version of, uh, applications. So can you tell us a little bit more about the user interface for the metaverse? Uh, what will it look like? What is it going to feel like? I think the visual representation of the metaverse is, um, is an interesting question. We don't, we can't really expect what will be the visualization of the metaverse.

[00:42:07] So people currently are using, um, uh, representation that are, uh, like the real world. Right. So we are talking about, uh, lands and we are talking about, um, you know, looking, looking at NFTs for, for your, your, your, your space, your, your, your house, right? So the virtual reality, the, the headsets where you are immersed in your space are logical first steps, but I don't think it will be the final representation of the, of the

[00:42:40] I think you, you will have something that looks like. Uh, the cosmos, you know, we've got connection with different, uh, universities. So what you're really talking about is interoperability between your normal everyday life and the digital world. It's definitely part of your digital life, your identity, your data, uh, your, your habits, your, your social, uh, circle circles, your, uh, all of these we'll, uh, we'll define what is your.

[00:43:11] Plays in the mid-levels now, obviously there's a lot of talk from centralized organizations and a lot of interest in building the metaverse from companies like Google and Microsoft, as well as of course, well, Metta we're a decentralized technology company. So how do we make sure that the future of the metaverse is decentralized?

[00:43:28] So by definition, if the metaverse is a group between everything and every apps, no corporation, no one corporation can own the metaverse. Right? So meta from Facebook will be a universe by the metadata. Right. But if you represent the metatarsal as a collection of. I can only is one, no one owns a calendar.

[00:43:54] Uh, so I think he has, it has two great properties to be larger than them. Then one universe owned by one corporation. Why? Because it's owned by the community and many different apps or can be. Engineer the all developed and share the on, on the blockchain. Uh, no one has the control of what will be actually, uh, developed, uh, on, on calendar.

[00:44:21] So it's way more burn. No one takes the decision, right? While I think the corporation will orient what will be honored, deployed on, on their metaverse and how it would work. But I don't see that as a competition, it needs to be a collaboration with, uh, corporations, because if you want to, to enforce the interim via interoperability between universities, you have to work with, uh, other, uh, ecosystems to define what, what is this interoperability protocol around the NFTs?

[00:44:52] So the data, uh, the ontologies. What's the place of the data in the context, right? In a, in a particular application, how you can, I could actually access, uh, metadata of a, of a NFT, et cetera, et cetera. So Cartano obviously wants to be a leader in creating this interoperable metaverse environment, but what does the Cardona blockchain actually offer to somebody who wants to build in the metaverse?

[00:45:17] So Carolina offers a free three main components. So the NFTs through the natives, uh, asset, uh, standard. So anyone today can, can actually create an it on calendar. Uh, the second aspect is smart contracts because you, you, you need to be able to evolve an NFT. From your version, one of NFTE two, the version two of your NFT, and you need to attach digital identities to the NFT.

[00:45:51] So we have at our prism, which is a decentralized identity solution that is required to attach, uh, a user of, to his NFTs and that to translate in different, uh, in other ecosystems or other universe, are you personally excited to see the metaverse come online? I know it's a, it's a digital transformation of, of our world.

[00:46:15] Like it's not, it's beyond blockchain. Blockchain is a, is a, is a tool where the NFTs and the communities are. Th the metaverse is a, is a digital transformation where no co no corporation owns a silo, uh, and, uh, applications are owned by there. And by the users, you know, you, when you, you are a gamer, you contribute to the quality of the game.

[00:46:41] Uh, for example, in multiplayer games, right? If you are, if you have good players, you have a good game, right? So they should, uh, have the reward of their, um, participation in the game, giving back to the users, uh, more that that's what the metaverse is, uh, Isabella and removing frontiers. And connecting silos.

[00:47:05] Thanks so much for joining us Roma. So in the metaverse, it is predicted that everybody will be able to do more or less the things that they do in their normal, everyday base reality life. They can own digital artwork or even land. They can customize a digital avatar. And of course, all of this comes down to one thing and that is NFTs.

[00:47:25] So today we are joined by Josh Miller, our commercial NFT business lead to find out a little bit more how NFTs Dano meet with the metaverse Josh, what do NFTs have to do with the metamours? The metaverse can be incorporated with many components of NFT. Uh, you know, obviously you've seen out there with virtual real estate, so, and Ft can be the certificate of ownership.

[00:47:46] Uh, we've seen it with products like you've seen with, uh, in the fashion industry where you can have a layout, uh, try on different clothes. There's even ones that are coming out that are attached to physical clothes. So think of the metaverse as your new e-commerce plan. Uh, where the entities are either the, uh, ownership or it's the product to be owned, or it's the event that's going on a special access and privilege within, uh, a metaverse I'd say, um, you know, I'd say that the Metta versus the hamburger and the, uh, NFTs are the catch-up, uh, so specifically they bring things together and make them better.

[00:48:21] Yeah, exactly. All right. Okay, great. So for all the ketchup, uh, lovers out there, I suppose, uh, that's NFTs and the metaverse. Uh, but speaking about car Dano, uh, what does car specifically offer to somebody who wants to build NFTs for the map? You know, as far as, uh, what Chardonnay offers is, is along the same lines as every other blockchain, but it's a choice.

[00:48:43] Uh, we talked about Cardona being eco-friendly. We talked about being carbon neutral. Uh, and we talk about the community that drives Cardona is one of the closest and largest that you've seen. I've seen at the end of the day, you have to target your audience and they go with what they know and the best way to get some of that market cap to get some of that pie is to go where the business.

[00:49:04] Um, so was Cardinal being a great part of that. Having its own features, having its own access, having its own flavor, uh, is what draws attention in health to be part of the conversation overall and really brings Cardona into the metaverse, uh, along with building the metaverse up and what it's capable of.

[00:49:21] So obviously you're privy to a lot of the projects that are building on car Dano. Uh, what have you seen out there so far? The big metaverse ones to keep an eye out on are the ones that are actually being backed by big names, uh, that are coming on to Cardinal and not just to be a Cardinal exclusive, but like I mentioned earlier to be part of the conversation and to be that multi chain, uh, to be that multicomponent, but you're going to see some really interesting stuff coming up here in the next few weeks.

[00:49:46] So we were just having a conversation with Roma about how the Metta versus a sort of glue that allows you to bring value from your digital life back to your base reality life. Uh, what are your thoughts? Yeah, he's absolutely right. And we're going to see that more and more as it things evolve because there's no reason why you couldn't take even the house you live in apartment or anything like that.

[00:50:08] And the things within your house. If you buy a couch, if you have a certain TV, even children's toys and why you couldn't have a digital representation of this in the metaverse, uh, and that can also lead to I marketing campaigns or, uh, you know, uh, uh, product targeting from these brands, uh, that are out there.

[00:50:26] That's going to enhance the experience all around. So what you see in the metaverse they'll get ideas to bring in a physical one, or you'll be able to interact with brands more, uh, interact with people more and really, uh, bridge the gap, uh, between digital and physical. So we're beginning to see this picture emerge of the metaverse as a sort of interoperable layer between the real world and the digital world.

[00:50:48] Very cool. Who is actually building the foundations of the metaverse. Well, we tracked down a couple of the projects that are working on car Dano for the metaverse. And today we are joined by Linda Antos of clay nation. Welcome to the show Alaina. So what is claiming. So we start out as a series of 10,000 algorithmically assembled NFTE characters.

[00:51:10] Um, and we made them entirely from clay. Um, we're one of the first, I think, handmade generative series on . And, um, like we really wanted our characters to have a little personality and imperfections, which kind of end up making them quite lovable. I think if you really have a look, you can kind of see fingerprints, you can see dust and fluff, um, like from our animators hands really pressed into the clay.

[00:51:32] Um, and we think that makes them pretty special and lovable. We released declination series back in September. Um, we always had it in mind that we wanted to bring these characters to life. We didn't just want them to be still, especially as we were at a stop motion animation group beforehand. And so like the first step that we're taking in terms of metaverse interaction is we're providing everyone that holds one of these, a AR and VR compatible.

[00:51:54] And they're going to be ready to explore virtual worlds. Um, so everything that we're doing at the moment, we're always building with interoperability considered like at each stage. And, um, we hope that this will enable us to integrate with other projects voting on Caetano as well as hopefully projects on other blockchains.

[00:52:11] So clay nation is a collection of characters that exist in the digital world that you can take into the real world. So basically a metaverse, but why build it on Carlisle? Voting clinician, uncle Don. It was a really obvious choice for us. Um, firstly, and possibly most importantly, our K community is on chronic.

[00:52:29] And that support is one of the key reasons that we're at this stage now, you know, we started off quite small, humble animation group and like we've ended up growing because of that community support. And that is say like grassroots and we filled out on Caetano. Um, prior to, prior to launching the project, I was running a state pool and chronic anyway, and was involved in economic community.

[00:52:49] And, um, the re the real reason I got. So I was drawn in initially because of the sustainability benefits. No proof of stake, both financially, like with the low fees, it makes it possible for us to do a lot more. And I'm environmentally with the low energy intensity of good on it. Another thing that's really exciting is that we feel NFTA metaverse products on Kadana kind of just at the infancy.

[00:53:11] And, um, we've been at the forefront of the NMTC sort of since, since that started really taking off one Catano and, um, building as we go along kind of on the ride with it and, um, the rapid growth of it. Just means that there's a, there's a huge scope for creativity and innovation, and we want to be a part of that.

[00:53:28] So you mentioned we're kind of at our infancy right now of projects that are building in the metaverse and projects that are building or in car Dano. Uh, where do you see us going in the future? It's a huge question. Um, so I think in the same, like in the same way that you can't step in the same river twice, um, I see the metabolic experience as something that is constantly evolving and every single experience in the math class will be unique.

[00:53:50] Um, regarding K nation, we hope that people would be able to experience that fast, you know, culture, music, arts education, and all of this will be in, will be within this experience. And, um, I think like something that's really exciting is how massive these experiences can be. Um, it will open so many doors to imagination and really real connections.

[00:54:13] So there are loads of hurdles and many unknowns when it comes to metabolic development, but there are also limitless capabilities and I hope. I hope so and good time. Um, this will provide next level opportunities to be cool all around the world. Fantastic. So how do people get involved? Inclination? A great first step is to jump into our discord.

[00:54:33] Um, you'll find the community are super welcoming there and, uh, our team or our team are actually very active as well. So we're always happy to help. Um, we have Twitter spaces every other Monday where we answer questions from the community and we also have a website which is. Entrance point, which has a lot of information on, on why you might want to collect one, um, the different types that we have, the different verities, everything like that can be found there.

[00:54:55] Thanks so much for joining us Lenna. So now we are joined by Josh Jones of cornucopias a new game that is building on Cardona for the metaverse. Josh, welcome to the show. Tell us what is cornucopias cornucopias is a metaverse and NFT based blockchain game that has a variety of themes zones that people can explore that, uh, has different attractions in each zone.

[00:55:20] Uh, we're going to be, uh, using NFTs for the economy throughout, so people will be able to own their own assets. Uh, and then there's also going to be the metaverse elements in there where we bring in all sorts of different value from community and from different entrepreneurs and businesses around the world.

[00:55:38] So in terms of building this as a metaphor game, what makes it different than building a traditional style? Really the best way to answer that would be to say that we have to involve community. Uh, we have to allow it to be a platform and then it has to be interoperable eventually so that we can connect to other Metro versus, or other metaverse based projects, uh, because there needs to be a connection of this open world, right?

[00:56:05] Eventually. So I think it is an evolving vision for the metaverse, but our solution is going to be to bring in community and add value and create incentives for the community to participate community entrepreneurs and businesses, to participate in building this and to really carry out the scope we have to gradually decentralized so that we've got this self evolving and self growing world.

[00:56:30] So we talked with one of our folks that's working on NFTs about how one of the benefits of building on Cardona is that you get the community along with it. What's card auto bringing to cornucopias. So we love Cardona for a variety of reasons. It's really bringing some key elements in its solution that, uh, we need.

[00:56:50] So for example, thinking about scaling in the future, when the tidal wave of people come to the, uh, blockchain and come into crypto, uh, I think a lot of the other chains are going to break because they haven't really been designed with the fundamentals in mind. And so there's, there's been these quick fix type solutions.

[00:57:10] Well, with Hydra and with scaling Cardona was going to be able to handle that volume. And with gaming volume, we have a tremendous need for, you know, there's, there could be millions of games saves per day, billions of games, SES per day, eventually. So, uh, that there's a huge need for scalability there and Kardon, and we'll have that, uh, additionally, the catalyst project, Voltaire, Voltaire, and governance.

[00:57:35] We're going to need that as well. Because as I mentioned before, we need to have this ability for the community. And decentralization to grow the project, uh, for us. So it's gotta be a project that grows on its own and that businesses can be built on top of that and that the community can steer it and help it to evolve.

[00:57:54] Uh, so there's that as well. And lastly, a taller prism, that's an enormous feature that is going to be needed more and more as, as a result of blockchain, achieving mass adoption and government regulations around the world. We're going to have needs for a tele prism, uh, a variety of needs. And so that identity based solution is something we're actually hoping to connect with the atalla, uh, prism team soon.

[00:58:17] So, um, yeah, that's, there's a lot, I mean, there's so many and you know, lastly, I'll sum that up with, we're attracted to the vision and mission of Cardona bringing an economic identity to the billions of people around the world. That lack it. I mean, that's a selfless kind of mission that I, I I'm really attracted to.

[00:58:37] And, and I love the, uh, the Ethan. Th the, the blockchain ethos is kept in mind with Cardona's vision and mission, you know? So, um, there's so many issues with, uh, monetary policy around the world and, and Cardona, I think, has that in mind. So it seems that your focus is on identity, scalability and governance.

[00:58:57] Is that about right? Yeah. Those, those three features of car Dano are tremendously. Th they're going to be invaluable for us. All right. So what does cornucopias look like in three years cornucopia in three years? Well, I'm hoping that we've got a variety of solidified partnerships, uh, that bring in the music and the arts into our platform and bring these creative forces in.

[00:59:23] I'm hoping that we have, uh, a variety of different projects building on top of our, our city, uh, and connecting to these individual bubbles where these custom domes that we're allowing people to build. So a unique use cases, for example, maybe Tesla's building out a. A training center and, uh, and the ability to showcase their vehicles in virtual reality within their own space that they have.

[00:59:51] And then there's a connection within the city that allows them to achieve that and drive traffic to their space. Uh, maybe there's a variety of different, um, communities participating in gaming guilds. And, and, uh, for example, we've got a partnership with Tingo, uh, which you guys are well familiar with Tingo wire, uh, Tingo mobile and they're, they have 10 million subscribers.

[01:00:16] And so what we get to do there is we get to bring our learn to earn features to 10 million subscribers in Nigeria. So we're very connected here at cornucopias with the mission of, of really bringing value in Africa. And what's going on with. Uh, we love that. I'd really like to see a lot of these early partnerships that we're forming that add tons of value, uh, panning out, uh, in a platform kind of way that enables so many others to create.

[01:00:46] On top of our platform. We also have a partnership with European business university where learned to earn aspects of people can get scholarships by playing our game. And so there's a lot of things that we really want to see happening, and it needs to be in three years happening on its own without our control and direction.

[01:01:06] So how do people get involved with cornucopia? Yeah, they can just go to cornucopias.io, our website, or you can follow us on Twitter at cornucopias game or go to our discord. So any of those are going to point you in the right direction. We've got a strong community, a really positive one, and we're creating an awesome, fun, creative, engaging community.

[01:01:26] And, uh, we'd love to have you involved. So clay nation and cornucopias are only two of the projects that are building on Cardona for the metaverse. Now, there are obviously a lot of other projects that we couldn't feed your here, but you should absolutely check them out. And we've listed them in the metadata below the creation of the metaverse will likely mirror the development of the internet.

[01:01:46] And that means that independent creators and entrepreneurs will be responsible for filling the space with new businesses and new experiences. Cardona wants to be the platform that's open to everybody that they can build. As we said, this is just early days for the creation of the metaverse. So to find out more about projects that are building on Cardona for the metaverse make sure to stay tuned to all of our official channels.

[01:02:13] Every month, we introduce you to some of the innovators building on Cardone, so you can check them out. Let's head over to Matt. Now who's been talking to a handful more

[01:02:25] this week. I continued my mission of talking to you projects, building on Cartano so that you, the community can find out what's going on in every corner of the ecosystem. This week we had on project nuMe trading, tent token and CC vault IO. Let's jump in. What is your mission and how is that different from other projects or pre-existing solutions in the market?

[01:02:50] Our goal at is to become the go-to Kadana wallet for newcomers and power users alike. From the beginning. We've asked our user for the suggestions when you features on GitHub and now on discord, and that's how we've been able to implement many of the current features of CC. What I O for instance, detailed CFP support.

[01:03:12] Yeah. Well, Matthew, thank you. First of all, for having us on, uh, it's an honor to come on and talk to the community that we're building an all encompassing ecosystem for musicians to live from conception to essentially retirement, uh, and that makes us extremely different from any other solution, uh, that's being built currently or anything from the traditional system that exists today.

[01:03:33] The name of our project is token T O K H. Dot IO. Um, we are a smart contract driven NFT marketplace. Our mission is to, uh, offer users and intuitive user-friendly platform, um, with features such as comprehensive minting auction systems, bundled sales, policy management, verification services, royalties, secure token wallet, and a premium partner artist program.

[01:04:00] 10th is an automatic native Cordato. As a trading system. It allows to users to connect and trade directly between them. I think the most common case right now, we've seen this obviously NFTs since it's, it allows you to trade easily and fast instead of going through a smart contract marketplace and locking your assets and waiting for someone to buy it.

[01:04:23] What are the advantages of building on Cartano? Why are you and your team in the Cardinal ecosystem, as opposed to any other, we entered the Caetano space in 2018 when there was only a vision of a blockchain like Bitcoin, but with a proof of stake, consensus and Unchained governance built from the ground up to last for decades, our team believes that GoDaddy as a technology of us, the best long-term solutions in the space.

[01:04:50] We also like the fact that for every new challenge that comes up there is always a research paper that addresses the issue and like an implementation of that paper already on the way. So the reason we chose Cartano to build on it, just a couple of reasons. The first biggest one is that if we're going to be interesting, millions of dollars worth of IP rights on a network, we need to go with something that we know is going to be around and have staying power.

[01:05:16] Another big thing is that we need fi predictable. You cannot run a business. If you don't know what your expenses are gonna be. The reason we chose Cardona is Cardona is a bedrock level, one blockchain. Um, it has the advantages of being peer reviewed scientific method, making sure that everything is very stable, solid well-defined it's not going to have problems.

[01:05:43] You're not going to have to turn it off, turn it on again. And so that's what we need to build our music ecosystem. Also, the other projects that are building on Cordato. So we don't plan to build everything ourself. We're going to be, you know, finding partners and others to, to help us with certain aspects of that.

[01:06:01] And so, you know, we'll be looking for service providers that do things like file storage on the blockchain or. Trading a fungible tokens. We'll be building some of those pieces ourselves, but also it's a great ecosystem in general, for collaboration. First, the blockchain is developed based on a scientific approach, a very mutable and very scalable when it comes to native assets.

[01:06:26] The fact that it goes through a proof of stake, uh, that, that involve, uh, low energy and low fees, uh, was also very interesting for us. And we are really interested in the, in the UTX. So model two, which is very unique in the way it's built. And the engagement from the kernel community has been like a huge facilitator to improve our development process.

[01:06:48] The first biggest advantage and be on building on credential is the extended you take. So model, which is literally what allows her project to exist. So this model allows us to trade multiple assets in a single transaction. We've done internal testing and we sent like, it was like 30 50. And if there's in a single transactions, we also love the Cardinal, like the methodology between credential of measure twice.

[01:07:14] Cut once. So. We, we love the philosophy behind credential and that's why we're in the space. We want it to be early and we want to help the ecosystem by building the tools for collectors to trade and to collect as easy as they can leveraging all the benefits of Cardinal. So how's it going? What stage are you guys at now in your development?

[01:07:33] A lot of app is currently packed with features all crammed into one, not so pretty UI. Um, we are currently working on a modular version, two of which will be much more static and allow users to activate the parts of the wallet that they need and the activate, the parts that they don't need. This new system will also enable the integration of third party projects.

[01:07:59] We are also working on staking board, a feature that not only earn users, more ADA on the delegation, but also provide a much needed revenue stream to fund future sees what I owe. Uh, it will also allow us to submit our code for a security audit, which has been requested a lot by our community. Um, and because security audits costs money.

[01:08:26] And our main objective at this point is to secure a revenue stream. Right now, we are in the process of, of fundraising and development. So we've already started development. We are working towards our minimum viable product, which includes, um, fractionalization of IP rights on Cardona. So we take a music and Ft.

[01:08:50] Fractionalize it. And. Fractionalized ownership of that. As far as auditing work and security work, we have advisors on board. They're also in the process of putting together mobile apps. So we, we will have eventually a streaming experience for the MVP. We started with minting service first and we quickly we'll start working on our marketplace, but it was a very basic version early on.

[01:09:14] So we implement a smart contract functionality thanks to Quinn. And it was still a very basic version of the smart contracts. So we're right now working towards upgrade to a smart contract. And we would like to prove that it's really secure and it's safe to use. So we're thinking of two routes at the moment, whether it's to open source it or put it up for auditing.

[01:09:34] I think we're about to close about 5 million. Being so sold on our marketplace, which is huge and nearly 10,000 sales, you know, completed. And that there's a lot of auctions still taking place in our marketplace. And we're proud of that. Um, what we're looking forward to next case as a site to revamp and well integration with the smart contract of the new version of a smart contract, frankly, we're already on main net.

[01:09:59] We are an open beta right now. Like anyone can access that anyone can create a tent. Anyone can trade a tent. We are still in beta because it's just like the first version. And we still have a lot of plans for the future. And we are looking maybe into the future as the project rolls more to get audited and to allow.

[01:10:20] Like other people to look into the inner workings, but for the moment we just need our internal testing and we try to be super clear and super transparent. And the way the wallets work, they show all the transaction outputs just before you're going to sign it. We're also like working right now with other projects in the space to help us grow and to help them grow.

[01:10:41] So, for example, we're working right now with integrating ourselves with a lot of descript servers. The most popular bots likes you. And if the bot and when book are working with us to allow every server, they are in to just open a 10 by doing a district command successful launch and staying power are two different things.

[01:11:00] Post-launch what are some of the crucial milestones on the path to becoming an established part of this. Once we've secured the funding. That's the next major milestone. We will be able to grow the team significantly, um, that will allow us to not only refine the user experience, but also venture into new areas and partnerships with other Kadana projects.

[01:11:23] Interesting for PR projects like ours would be the integration of Atala prison, service providers, Texas, and marketplaces. And we will also explore hydro notes for low cost, internet transactions. One thing that we really have to keep in mind when you talk like about launch and stay in power, is that as has been mentioned before, we really focusing very much on our community and that it has been shown with the airdrop that we did to our community members that were loyal, uh, from the beginning.

[01:11:57] So I can tell you in reference to milestones for what new is going to be looking like as. Go into the future. I want to put a caveat and I want to say that our governing ethos is we under promise and over deliver everyone on our team is in the same mindset. So with that being said, like Andrew mentioned for our minimum viable product, having that fractionalizing of IP rights, that's the first step.

[01:12:25] And the reason we chose to do this and to go go, this approach is because if musicians are our focus, then that is something that can immediately generate income for a musician. So that's the reason we went with that for a second, uh, the marketplace to actually trade the IP rights. Right? So that's the next step.

[01:12:45] After we have that in place, then we're going to be ready to start collecting royalties and the distribution of the payouts of Royal. Right. And so with that, then we have the streaming platforms that's going to go live with also the option to do ticket sales for the artists through the app. And then finally, we're going to get to the point to where we can fully decentralize the protocol and have the Dow creation to where we can hand off the keys to the community and let them steer the ship on where they want the future of this music.

[01:13:17] Eco ecosystem to go. Token has a roadmap planned for 2022. Uh, Q1. We have planned a complete site revamp, um, Q2 we're focusing on our token implementation to the site, along with the rewards mechanism. Uh, Q3, we're gearing up to approach the commercial sector for implementation of NS NFT, such as retail ticketing and luxury goods.

[01:13:44] And we're going to close out Q4 with a cross chain integration planning, working on the ability to buy and sell NFTs from one blockchain to another. For the moment, one of the crucial things we want to do is still do much more like marketing wise to help her shuttle grow and be like more known between the projects.

[01:14:03] And the other thing we're working on is with integrations for us, integrations is a key part of the ecosystem and allowing ourselves to work with other projects. We know we like stand alone. We have a great product product, but as we get ourselves integrated, Other project, for example, we have a partner program.

[01:14:23] So every project can have their custom link where like, just about to launch that. But that partner program is super important for us because it allows projects could give their community another benefit. And this integration with discord bots is another way for us to launch. And obviously there's like extra functionality we want to add to the product, like, uh, the ability to chat while you're trading, um, the ability to have an easier communication with the people.

[01:14:51] How do you see your project's niche developing on Cardona over the next few years and into the longer term and what industry problems do you feel that your project is uniquely able to address? Well, as more and more projects are launched on Caetano that appeal not only to tech savvy people, but also to the masses.

[01:15:11] It is important that the average user can interact with blockchain services in a natural way. Think about online banking systems, they all have their pitfalls, but people have learned to use them in future versions of . We want to make it easy to get started and also easy to use our wallet on a daily basis.

[01:15:34] So with the current music system in place, you're going to find that it's much like the banking industry, where there are tons of middlemen and they're gatekeepers. And so basically to keep things very simple, Um, what we're essentially doing is we are going to be replacing the middleman with a protocol.

[01:15:50] That's not incentivized to make a profit. It's just incentivized to have just enough income to where it can function and pay for its infrastructure and run. And so when you do that, you all of a sudden, essentially create more revenue for the artists and the creatives. And so it doesn't have to get sucked up by maybe a pro in the middle that takes half the profits, or it doesn't have to go to a label who owns all of their IP rights.

[01:16:16] Typically if you're a very small artist. So how can you do that? You can choose to sell part of your IP rights to the community. This is great because now you have not just consumers of your music, but you have people who are invested in you and your success. This creates a positive feedback loop. So this is going to build upon.

[01:16:34] Um, I can tell you right now what we are going to do for car donno. I think we are uniquely positioned to help with actual mass adoption as an ecosystem that is not focused on crypto, but focused on mainstream and people who aren't in crypto, uh, for us to bring those people into this ecosystem, really, without them knowing.

[01:16:55] If we've done our job, right. They won't know that they're really working with the blockchain or it shouldn't feel techie. It should feel organic. So when we imagine, and bill tuck and the metadata has structure, and even the name talkin, you know, vision and FTE, we're not just GP art on the blockchain.

[01:17:11] What we've been forcing is a much wider use cases for NFTE NFTs in the future. So we are positioning ourselves to evolve within the space, uh, needs in the future. Yeah. You know, like why do you use cases like being able to, uh, buy a ticket or buy a car and actually sell the ownership of a car as an NFT is one thing.

[01:17:30] And now we could work with commercial partners. Like, let's say Gucci wants to build a handbag and with it NFT inside, it that's a proof of purchase and saying that this is authentic. There are so many white use cases that people are yet to dream of digital art and NFT. Collectibles is just one thing, you know, w we're going to show the world that there's more.

[01:17:49] Directly, I would think is the peer to peer trading. Right. Um, as I talked about a little bit earlier, like for the most part, the most rated asserts are obviously NFTs. Um, I think that niche, like the NFD ecosystem is just going to grow over time. Like it's still super early in Cardinal, but we can see. And I mean, no one can ignore the relevance that the NFTs are gaining.

[01:18:16] So as the ecosystem grows, there will always be the need for personal direct transactions. Like not every transaction requires a smart contract marketplace where the asset is locked, where you cannot like guarantee that the seller you want will take it. Like there's always going to be the need for human interactions.

[01:18:34] And that's what we want to enable and empower this direct between users transactions, the space grows. We will always be focused on peer to peer. That's like our nation, how we see it. I want to thank all the projects that came on the show today for sharing their ideas, their vision, and their mission with the wider ecosystem until next time.

[01:18:55] Now, remember none of these interviews constitute financial advice nor should be seen as a direct endorsement from IOG. Always do your own research. So as defy grows on car domino developers are coming together to continue to evolve and build out the developer ecosystem from tools and API APIs to core polluters improvements and enhancements.

[01:19:15] The Cardona defy Alliance is a new consortium looking to help standardize Plutus and Cardona development best practice within the defined community. I sat down with Eric and Damon from the project to hear more about the mission and to hear how the Plutus developer community is rallying behind that shared purpose.

[01:19:34] So Eric Damon, regular viewers might recognize you from your work with Charlie three and with the indigo protocol. But today you're here to talk about the car Dano defy Alliance. Eric, perhaps you can tell me a little bit about the history of that and how it all came about. Really the CDA came about from individual work that a lot of the defy protocols were encountering, uh, as we were building on Caetano emotion to create an Alliance to achieve more, uh, greater in numbers, right?

[01:20:00] So started to ideate the concept of putting bright minds. Brilliant engineers together in the same room and, um, overcoming development, hurdles and tasks, uh, with, with more people, uh, achieving that same mission rather than just individual teams. So you're slowly and steadily building out your membership, the brightest minds in the room, as you say, but Damon, how is this going to filter through, into real ecosystem value?

[01:20:24] Yeah, absolutely. I think that's a great question. And part of our core ethos, I mean, why get everyone together to, to create when, if there's no real reason for it? Right. So it's, it's an intensely innovative area, you know, car Dano in general. So. Getting the ecosystem up running faster will benefit everybody.

[01:20:44] That's trying to build for Cardinal and benefit the community as well. So getting all of these projects together to work in tandem, to make that ecosystem boost faster, benefits everybody, but more specifically, we want to benefit the growth on a development side as well. You know, Plutus scripts and libraries to help other projects deal with their journeys along the way for having proper documentation, I think is huge.

[01:21:08] And that's a real big goal of ours. And then also education everywhere from the general consumer, all the way up to the high core developers and even into marketing business development areas. Like how can you build your project faster and get to the level where we are without having to go through the same hurdles.

[01:21:26] So it's kind of. Making a, a success book to a point and making sure that everybody understands what they're investing in, how to manage that and just navigate the ecosystem a little bit better. Now, Eric, you're working quite closely with a number of the team here at IOG. Tell us a bit about how that's going.

[01:21:42] Yeah, it's been great so far. Um, I think to get closer with the inner workings of IOG, just for myself, has been good to understand kind of how things go, the nature of conducting business from a collaborative approach perspective. So yeah, I think it's been really positive. Um, and, and just really to, to Damon's point, the ethos of the CDA is to empower and enhance the education of Plutus.

[01:22:06] Uh, so being more involved with the IOG representatives has been really helpful in that, so that we can, uh, achieve that mission. And Eric, of course, this is a growing membership organization. How are you looking to expand upon your member base? So, yes, the CDAs and open enrollment Alliance, we have, uh, our application process through the website.

[01:22:23] So it's easily accessible to anybody who is interested in the CDA. Perhaps you can provide the. Yeah. So it's just easy application process. And our member relations team will align an interview with each applicant post, uh, receiving that application. Uh, and then the application is then reviewed internally and all the notes from the meeting that the member relations team convey to the group and we'll have an internal vote.

[01:22:46] So as to approve the, uh, new member applicants enrollment in the CDA, so a very easy process, uh, we do need to make sure that the criteria is met for each individual applicant, that they are in line with where we want to see a new member being with regards to their development process. Um, and obviously being aligned with being a defy protocol as well.

[01:23:05] Damon you're leading on the marketing efforts for the CDA. Tell us how can the community get. I think just making sure you guys keep up to date with our regular developments. Uh, we work together to manage our, our meetings and what's coming up next or new member positions like right now, there's only a few, um, Eric and Ben from M labs and myself and Cody, uh, have legitimate positions that we are specified with.

[01:23:30] But I think it brings a lot of trust to the community to see that we have specified roles and that we're working on things. So just keep up to date to see our new membership and other things in our blog posts. And obviously through the website, which Eric just said. Be in the description below. So gentlemen, thanks very much for joining before you go.

[01:23:49] Maybe I'll give you a quick opportunity to update us on your projects. Damon, how's it going with Charlie three? Yeah, Charlie theory going really good. We just had a catalyst fund, seven wins. So thank you to the community there. Uh, and that's to provide. Free price feeds for startups in the ecosystem. So you don't have to worry about the price of Oracle feeds.

[01:24:09] So that's really nice and past that we've got a working aggregation model for our Oracles, uh, so we can be ready to provide the data that we need to, to projects that need it, uh, pretty, pretty soon. And working on scalability options from our side, expanding the team as much as possible and looking at new investment ventures to keep us running through to the future.

[01:24:30] So, uh, really excited about our progress so far, the engineers are doing a fantastic job and just looking forward to, uh, the birth of a few new projects on main Matt and Eric. What's the latest on. Full steam ahead, Tim. Uh, we have recently added on three new core team members in our product research and product innovation teams.

[01:24:49] Um, so that's very exciting for us growth. We've also as well recently gotten approved for our fund seven catalyst proposal. Thank you to the community. Um, not only for approving Charlie's because we'll also be using the Oracle platform, uh, but as well for ours. So we're, we're building out a multi-decade SDK and collaborating with mint swap on that as well.

[01:25:06] So very exciting. Thank you to the community again for approval. Um, and really a vote of confidence with indigo. Our contracts, smart contracts have been passed. Security audit will probably go in for a secondary audit as we get closer to main net. But, um, yeah, like I said, full steam ahead and a lot of productivity, Eric Daymond for the Cardona D fire lights.

[01:25:24] Thanks very much. So that's a wrap for February. If you haven't already make sure you hit that, like subscribe and bell and be sure to check out the links below. Also, you can head over to the IAG blog for the very latest on the car dyno stack exchange, a new resource for the Cardona developer community.

[01:25:42] The latest on the hydro family of protocols, plus pipelining and more. Be sure to join us for the March mid month development update and set a reminder for our full March show happening on the 31st, where we bring you the latest development news, plus all your ecosystem updates. Thanks for joining. And we'll see you in March.

