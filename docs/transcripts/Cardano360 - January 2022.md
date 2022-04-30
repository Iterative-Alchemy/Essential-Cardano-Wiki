# Cardano360 - January 2022

[00:00:00] Welcome to your January edition of Cardone 360, your monthly show, where we meet some of the people building out this incredible ecosystem. Now, before we start, remember to click like subscribe and hit the bell to get all the latest videos as they come. Now, later in the show, we'll be catching up with Emergo on the DC spark and with a few of the projects building on Cardone.

[00:00:35] But before we get into that, let's start off with our regular monthly development update. So Nigel, Kevin, John, thanks very much for joining us again on Cardone 360 John, let's start with you a very busy few weeks on the network. And particularly last week with the launch of a major Dex project on Cardona, perhaps you can tell us a little bit about what happened and what.

[00:00:56] Absolutely then. Thanks. So having Sunday launch was really a milestone to see such a large exchange, um, bringing so much liquidity and so much excitement, uh, to the network. Of course, uh, as people will be aware, especially the thousands of people who are excited to use it. Things were very busy, I suppose, no different to the excitement around any other product launch.

[00:01:15] Uh, just like the iPhone. Um, people are standing a little bit in line waiting for it. So I'd like to maybe look at some of the things, some of the factors that played into the overall UX or user experience there. Um, as I mentioned, kind of before, I think when I've been talking to you guys on the program, I think it's really important that folks have a great user experience.

[00:01:34] Um, that's got to come straight after security, stability, robustness straight after that, from my point of view, uh, UX is primary. Um, because people don't have a great time using a product. They're not going to continue to use it. So UX is something that I spend a lot of time focusing on. So it was busy.

[00:01:50] Why was it busy? So let's look at the first pillar, the core network. I've spoken before about the Coronet work and some of its facets. I've spoken as well about the fact that we have this five second propagation window, uh, in which to get blocks across the network. We also have a certain block size, which means that there's pear block, which is every 20 seconds.

[00:02:09] Uh, we have so many transactions that could fit in that. There's a finite number and we have so many scripts that can fit in it. Now scripts are the smart contracts and the Cardinal platform and with a defy marketplace like Sunday's, well, they make heavy use of scripts. So currently a block will hold approximately four scripts at one time.

[00:02:26] And then the rest of the block will be a regular ADA transactions, which are just money that's being moved rather than, than invocation of scripts or execution of scripts. So the reason it was so busy on the launch was we had all of these users all excited to get their swaps out there. And the coordinate work spent its time, uh, processing as many of these scripts as possible.

[00:02:47] Now as script the way. So they swap who have architected their solution as you don't, it's not a single script for a swap. In fact, right now, a single script, a single Cardinal smart contract actually performs a swap on about four transactions. So you can have four users of Sunday swab, uh, satisfied by the execution of a single script, which means when we scale it out in a single block, we were kind of processing about 16 swaps for Sunday as well.

[00:03:18] Now, of course, 16 is a reasonable number, but the excitement was such that there was hundreds and thousands of orders. So therefore a backlog started to grow and we had a little bit of back pressure folks that were waiting to get their, their swaps executed. So I appreciate we can do better than this. So what are we going to do in order to make sure that the layer, one of the.

[00:03:39] Can execute more so than they score scripts. And indeed, uh, forgetting about looking at Sunday, specifically, uh, economically looking at the entire defy suite of products that are out there. We want the throughput to be good for all dApps out there. So in order to do that, we're looking at the following things.

[00:03:55] And I've mentioned some of these before, but just to remind viewers, I think it's worth calling them. Number one is increasing the block size and we're going to be doing that in the very short term. I suspect, uh, in Q1 we'll have another increase to the block size I'll I'll confirm on the program, uh, when I've got more clarity on exactly when that's going to happen, but increasing the block size will directly allow more scripts to be executed in a block and therefore directly increasing throughput on L one, both for regular users of the Cardinal network who are sending ADA and for defy users.

[00:04:23] And additionally for Plutus we're increasing the resource limits that are available to scripts. So that's how much memory a, a script can employ and use when it's executing. And indeed how much computational resource, how much CPU time, how much computer time it can take up and doing. And when these limits grow, we can increase the efficacy of a script.

[00:04:43] So therefore rather than having a script, execute four swaps for a script, we can now have that same single script, actually settle or execute maybe eight to 10 swaps. So as you can see, that throughput really grows as we increase both the block size and the Plutus resources, we have already made changes to the block size and we've made changes to the resources that are available in Plutus not only once, but two days ago, um, on Tuesday, uh, we made an additional increase to the Plutus limits and we, we will be doing so again throughout the year.

[00:05:15] So, as I mentioned in previous videos on the core network, just to close this point off, because this is only one of three things I want to talk about. The core network is going to scale this year. We're focusing on giving ourselves headroom of blood propagation by increasing efficiency. We increase efficiency by rolling out changes like pipelining and input endorsers.

[00:05:34] And those changes that increase efficiency, then allow us to spend that extra time we've gained on increasing block size pushing layer one. So it has maximum possible speed and indeed increasing the resources that are available to the smart contracts in the platform. And when you roll all of this together, what you have is layer one, in-car Dano becoming the most competitive, the best performing network in the D fly space.

[00:05:57] And that's my goal for 2022. So John, the user experience will continue to improve and it's very clear, you know, there were frustrations out there. We need to acknowledge those at this very early stage. Sure. They will continue to improve, but fundamentally we're happy with the network performance in terms of security and resilience.

[00:06:15] I understand. No serious issues there. Absolutely. So I appreciate that. There's things we can do better in terms of overall wait times for users. I'm more focused on that, but in terms of the fundamentals of the security of the network, the stability of the network. Okay. And when I, when I say that, I mean, how secure are your funds?

[00:06:33] Can you be confident when you're using the platform? Is the platform up all the time at 100% utilization running, uh, where every block is full, those characteristics were perfect with that viewpoint of security and stability. We were delighted with how it performed in fact, but we will increase throughput so that the user experience is better.

[00:06:52] Overall. Maybe I could also then move away from the core network for a second. Talk about two other areas where I think docs in general, I will get a better UX, uh, for end users. So the first is with the DOP itself, whether it's the sundae swap platform or otherwise, of course, Sunday, themselves will acknowledge that this rollout was a better release.

[00:07:12] Okay. Relatively mature, but it was still nonetheless. So they're going to be making changes to how their platform processes, transactions selects the transactions from various pools in order to settle them. At the moment, they have a sophisticated scheduling mechanism that chooses which swaps to settle on a fair basis.

[00:07:30] But of course they can tweak that. I think an area where they might want to look at is, you know, um, prioritizing constellations because I think some users were waiting for constellations to go through and stuff like that. But these guys are smart. They're aware of this stuff and they'll make it better as time goes on.

[00:07:45] Um, the final thing I'd like to address is maybe the wallet experience because the core network can be great and the DOP can be great. The third pillar is the wallets, and I have to say those guys did a great job. Um, there are lots of players out there, but maybe I can quickly name a NAMI CC block frost.

[00:08:01] Uh, these folks are working tirelessly to give a good user experience to their end users. And I've no doubt it was stressful times over at HQ for those guys too. Um, I think we can probably work together over time to increase the efficiency of these wallets. These guys are experiencing growth, just like we are and their back ends are architected to be as efficient, as performant as possible.

[00:08:23] But of course, just like with the core network, they need time to grow their backend to grow. They're stuck. And I'm sure that's something that they're going to be looking at too, as they adjust to this new, uh, there's new demand. Thank you, John. So Kevin, uh, we talked to recently about the release of the 1.33 node, which was sort of a prerequisite for any increased activity on defy.

[00:08:45] How is that looking so far? How has, uh, how has that gone? We're very pleased with what we've seen. 10, so a 1 33 a was the prerequisite for rolling out increases in the premise changes that John's been mentioning. Uh, we've been able to, uh, roll out our one or two changes ahead of the Sunday swap launch.

[00:09:07] Uh, but, uh, the information we're getting back from the monitoring, the node on main that looking at the, uh, what's happening with the a hundred percent utilization, uh, situation that we're in, uh, shows that we have, uh, more headroom there going forward. Pumping the parameters, uh, further, this is not the end of the journey.

[00:09:28] Uh, we do have additional capacity there. A hundred percent utilization is the new normal. What we'll be doing is to increase the parameters, taking advantage of the headroom that we've now built in, in 1 33 to enable a greater capacity on, on the. So what one side, three dots for the benefit of those haven't been following along, is it smooths out to some of the, uh, performance bumps, uh, in the system I will be working on this in the background, the new team, the legend team working hard on this.

[00:10:01] We've had two or three takes knotted over the last nine months or so it's been quite a time coming. Uh, what it does is to, uh, reduce the load at certain points in the cycle, say particularly at the 48 hour mark, uh, also, um, at the epoch boundary, there are a few more things we need to do going forward. So that will, again, that is get even more performance out of the node system.

[00:10:28] And I'd like to call out to be networking and benchmarking team without them. We wouldn't have the information that we've had, uh, that would let give us the confidence, uh, to roll out these performance improvements. So. Where we are now we can roll out a further increases in the, some of the flutist parameters, which will let, uh, define, uh, like Sunday process, more throughput per transaction.

[00:10:58] Uh, but also what we're looking to do is to increase the block size, uh, and that will last process, more transactions in a, in a given amount of time and all this will dramatically improve the user experience in the coming months and over, uh, the next. So Kevin just touching also on node 1.33. Um, I understand we've released a Daedalus flight version recently on that.

[00:11:20] What are people seeing there the day of his flight versioning? It includes a node fashion month 33, um, but also, uh, very important includes some tweaks to various, uh, memory settings and parameters that we've been, uh, benchmarking recently. So what this means to normal users, um, is that we will put a lid on the turtle, a memory that is used by, uh, the tablets wallet, the parameter settings, these suggest, uh, the start of a series of improvements that we're looking at.

[00:11:52] We'll tell you more about those going forward into 2022. Uh, but we've got some serious changes in the works that will make a big difference to the token memory utilization for dateless users. Thank you Kevin. So Nigel on the mid-month update, we outlined the 11 ways that we're going to be scaling our dyno in 2022.

[00:12:12] You obviously head of delivery. Your job is to deliver this and to sort of put some flesh on the bones of the plan. Tell us a little bit more about what's going to be happening during the course of this year. I understand three significant updates during the course of this year. How are things looking?

[00:12:24] It's going well, Tim, I think. It's worthwhile points. Now that it's, uh, it's the whole teams come together on this. This is a big effort. We've got a large amount of deliveries that are going to happen. 28 projects at the last count, multiple different deliveries going into production over the course of 2022.

[00:12:42] There's a large number of teams that have come together to organize the scope. But at the same time, these guys are delivering on a daily basis, which, uh, as we've just heard from John and Kevin, we've already knocked out a number of different updates to the, to the network and also support for the different types out is the community right now.

[00:13:00] So how do we go about doing it? Well, it's a large program of work. We have to organize it in different layers. So we have a layer in terms of the fundamental cortex. Um, which is all about networking efficiency and performance this year, looking to provide more optimizations, we then layer on it. Our plaintiff's work, uh, script optimizations, building out more tool sets and the rest of it.

[00:13:26] And we've got multiple products as well, while it's in services. . Uh, the kind of tools that developers use to be able to build that adapts. And then on top of that, even more new products come in coming into the space over the course of this year, whether that's the light wallet or the DAP store. So there's lots of things going on now we've put together a whole map and a plan for this year across all the teams.

[00:13:51] And I think as we, as we go into the coming weeks and we go through one more iteration, um, I think it'd be a great idea if we actually published that, uh, to the marketplace and community. So everyone's got a good view and a vision of where we're taking Kitano they share behind all that. I think it's worthwhile just talking about some of our major upgrades this year.

[00:14:13] We changed it this year and we changed it on purpose. So before we rolled out a major upgrades and release as hard forks and things like this, when as soon as they were. This time, we've decided to do it at certain fixed dates. So why have we done that? Well, the reason why we're doing that is because we now recognize we're in a much bigger community with a lot more people connected to us, but I need some time and some, the ability to understand when different things are happening.

[00:14:42] So they get the chance to prepare and make sure that they're integrating their right times and ready for launch as you well know, we've got over a hundred exchanges that have to follow our upgrade cycle, as well as hundreds and hundreds of SBOs. So we changed it this year and we said, okay, well, what if we get fixed release date?

[00:15:02] What would this look like? And we decided to pick on February, June, and October, and those dates are fixed so that each of our major partners that supports the network knows when actually they're going to have to do a major update. They can configure their technology and configure their resources to be able to support it.

[00:15:21] It's much easier to go to manage. In order to do this, it means then that we have a flight slot pattern across our different deliveries, where we've got three different runway slots, but people have to be able to get that code ready to be submitted into those slots and be ready with pets. As I've talked about February, June, and October in February, it won't be a hard fork, but it will be a major release it's about more work and towards our efficiency, performance and optimization.

[00:15:51] And it's also given us the underlining elements that police, that we need to be able to provide the sips for scripts optimization. Um, and this is what's going to, we're going to get there within February. And then we hit June. We have a significant increase when it comes to both the pipelining work and also the pollutive script optimization work inside that June hard for cause also going to be in our initial release of hydro, where there's going to be a lot more releases down down the line.

[00:16:19] As we actually prepare that piece of technology, the initial release of Hydra is going to enable us to actually understand the efficiencies that we get and the different transaction types that we get around Hydra. And to be testing it out on our main net, as we hit. But likewise, as we then develop the technology, we'll be looking for subsequent releases and follow releases as the year goes on October less well-defined as yet.

[00:16:44] And we will definitely be preparing and publishing more materials as we get through. But hopefully that gives you a good flavor of what's going to be happening this year. Thank you Nigel. For that. John let's finish off with you. We've got more dApps coming down the pipeline, a hundred percent being the new normal.

[00:16:58] What does it mean for the launch of those applications? It's a great question. Let me put it this way. I want to see the network at a hundred percent utilization at the entire time. That means we're getting the maximum bang for the book out of the implementation that we currently have running in may in there.

[00:17:13] So any blocks that are have space in them, that's not being used. That's not good. We want to see users use Cardona. We want to see Cardona being used to its maximum potential. Okay. That's my kind of starting point, but I will say we're seeing growth in the Cardona ecosystem and on the applications that are running on the, on the network.

[00:17:32] Hard to keep up with in terms of performance increases, but we're doing it. Um, we've already had three bumps to the layer one and throughput, the most recent of which, uh, being on Tuesday this week, but we're not stopping there. And in fact, given the release of 1.33, just to echo the comments that Kevin made, uh, on this, on this program and on previous discussions, we now have the headroom to start making more regular cadence in terms of our parameter bumps.

[00:17:59] And we're going to be increasing layer one, not only in block size, not only in clueless resource limits, but also in the efficiency of the node. And also in, in rolling out things like input endorser's layoffs, which is our next generation consensus mechanism, um, which is an iteration of aura Boris and indeed pipelining.

[00:18:18] So we have a plan that we're going to be enacting this year and we feel not only will. Will it allow Cardinal they're wanting to grow as the excitement and adoption grows, but also we're confident that we'll be able to outpace the growth of demand with growth of our performance. Gentlemen, thank you very much.

[00:18:39] Imma go. Uh, one of Cardona's three founding entities, educators, creators of your Roy wallet and now venture investors in Africa. Eric caught up with Kesha today. I'm joined by Kesha Dwyer, the marketing manager for Emergo. And she's going to give us an update on some of their recent progress and goals to the.

[00:19:00] Welcome to the show. Kesha, thank you. Nice to talk. Let's begin at the beginning. Uh, Emergo was there at the very outset and the inception of the car, Dano blockchain, and everybody knows it from the Yervoy wallet, uh, with that being said, what's going on with your eye right now. So really talk about your toy.

[00:19:19] Let's just talk about what's happening on Cardinal. So Cardinal has seen remarkable growth in recent months and with the high increase in transaction volume, coupled with what we expect, um, in terms of like future growth, we are focused on continuously improving and stabilizing your wave wallet as we grow with Cardinal.

[00:19:40] So you're away. It releases frequent back end improvements that aim to address the synchronization issues our users are facing. Sometimes resolving these network congestion issues takes us a little bit longer than we would like, but we want our community to know that your toy developers are continuously working to securely optimize your toy while its infrastructure and expand our server capacity.

[00:20:04] So we think the community for their incredible feedback and patience as we carefully manage that high peak load during these exciting times. So obviously we're dealing with a lot of growth in the Cardona ecosystem right now, more growth means more wallets. So how does your Roy keep leading the way as a founding entity it's inherent in our role to lead and support the ecosystem?

[00:20:27] So we always put the community first. We are listening to their feedback. We continue to iterate your toy based on the community's interests. Um, we also voluntarily provide resources. To support open source projects, which would benefit the community. Um, our Cardinal sterilization library is a good example of any Emergo led open source project and the library.

[00:20:50] There plays a big role for other wallets and depth to build on Cardinal plus that you Margo is always seeking new ways to lead the ecosystem. Um, the Cardinal improvement proposals represent an area where we believe we can bring our expertise to help shape the Cardinal standards for other projects building on card.

[00:21:09] So in Cardinal, obviously there's a huge focus on the community and we've recently heard that there's going to be a collaboration between Emergo and the developer community. So maybe you can tell us a little bit more about that. Sure. It's actually something we're really excited about. Um, Emergo in partnership with the Cardinal foundation has launched a new project to develop a community driven DAP tool sack for credit.

[00:21:34] And our goal there is to enable developers to easily deploy smart contracts on Cardinal. What devs can expect, um, is a modular tool stack with clear documentation and programming guidelines. And with that DAP tool stack, the folks building on Cardona will be able to connect without a full node, enabling faster and more flexible integration to support depths and wallets.

[00:21:59] Um, but I do want to talk about having the adapt tool that you like open source allows for a variety of applications to be built by third parties and increases the diversity of options available for developers to build solutions. So we believe that this will lead to an increase in the overall speed to market and adoption of.

[00:22:18] Now, obviously there's a ton of stuff happening around NFTs right now, but we've heard that Emergo is about to jump in the space as well. Uh, can you give us a sneak peek at what you guys are up to? So we were seeing the incredible amount of interests, um, and we were keen on. Thriving C and F T space as they like to say.

[00:22:39] Um, and we're proud to announce that the launch of our NFT marketplace fever read it'll be happening early 2022. So February will provide a way to connect socially conscious artists with buyers and sellers within the Cardinal ecosystem. It's developed by your Margo at four Cardinal, and we're utilizing ADA for transactions such as minting buying and.

[00:23:01] Um, the pre-launch buzz has already been exciting. Um, we've been named a top five NFT platform to watch for 2022 by grit daily. Um, and we've also received a coverage from prominent media publications, such as crypto sleep. But right now we are calling on Cardinal talent to get in touch with us to be a part of our highly anticipated launch.

[00:23:23] So if you are a Cardinal artist or musician interested in selling your work as an NFT and share our beliefs, that technology should have a positive social impact. Get in contact with us at dot IO. Um, we have a team that will assist the creators with putting together their collection, um, and best practices for promotion to really guide.

[00:23:46] Going through the process for the first time. So this is kind of for my own personal edification, but, but what do you actually mean when you're talking about social impact? Um, is this a pretty broad scope or, uh, you know, what kind of artists are you looking to support here and what we mean by, uh, trying to, uh, connect socially conscious artists, um, is like, I really believe that we are being aligned with Cardinal principles.

[00:24:09] So for example, Cardinal foundation just had a really impactful initiative of planting 1 million trees. Um, and on our side, for instance, we are talking with an artist, um, from Iran, she's a female graffiti artists. And I mean, just in terms of groundbreaking and breaking all the rules, we find that to be like that type of, um, compelling narrative.

[00:24:32] Yeah. So let's talk about Africa, um, at the summit and Margo announced that it would have a a hundred million dollar fund that was focused on Africa. So what's happening with that initiative at the. We've had an incredible amount of interest for our Africa initiative. Um, and we've assessed numerous companies and we have a lot more in the pipeline.

[00:24:50] It's a bit early, but what I can say is that there are two projects that have been carefully vetted and should complete your Merkel's investment process. Um, we'll syndicate a news release about this at the appropriate time. So, you know, we say stay tuned on that front. I'm also in Merkel's education unit Emergo academy has launched a new Cardinal entrepreneurial program for our Emergo Africa partner.

[00:25:14] I think in labs and Damien labs is an African tech incubator for startups building on Cardinal. Um, there are three at Daniel labs portfolio companies taking the program with the goal of incorporating Cardinal blockchain to their application. So everybody stay tuned to Emergo. All of their social channels are listed below and you can see what they are up to next.

[00:25:37] Kesha Dwyer. Thank you so much for joining us. Uh, do you have any parting thoughts for our audience before you go? Thank you for having me. Um, and just, I mean, with these updates developments and our investments, we truly look forward to Cardinal on 2022 and for our contributions to the ecosystem. Thanks for having me with a commitment to interoperability and building bridges, both literal and metaphorical DC spark a fast emerging as one of the more significant contributors to the Cardona week system.

[00:26:08] We caught up with Nicco and Sarah and new CMO, Kara Rossi to hear more about Flint wallet, milk and meat, a side chain animal. DC spark is focused on building critical products and solutions for leading blockchains. And that's why they've decided to work with Plutus and the larger Cardona ecosystem today we're joined by three of their global team.

[00:26:30] And, uh, well, why don't we start by having you guys go around and tell us who you are and what you do with DC spark? Uh, sure. Uh, so my name is and one of the co-founders and also the CEO of. This is spark. Hello. My name is Sebastian often called Sippa and I'm the CTO of DC spark. Hello, my name is and I am the CMO of this is fart.

[00:26:54] So Carol, let's begin with you. Can you give us a high level impression of what the mission of DC spark actually is? So where of course I crypto building company with the Misa we're developing different product for the crypto ecosystem globally. So if you ask me about the mission, I think that the mission until now, so it's focusing, always trying to have curiosity in ways of understanding the best way that we can solve technical projects in a very high level.

[00:27:23] And I think that it's great to have Nico and Sarah here cause they was staying in better, but also with a global mindset and global. I mean we're solving global problems, um, or I would say not problems, love the challenges and to self love and challenge. It is unique today. People from all over the world with different kinds of views, I'm thinking we're looking for diversity in all sense, then we can have new ways of solving something in the fastest and most I think correct way for, and also, um, we are a remote company, so we have people talking today.

[00:27:58] We are actually in three different continent at this precise moment having this talk and we have people working from all over the world. So I dunno, save yeah. Save. I know it's in Tokyo. So, um, um, Nico now is at this precise moment. He's in Europe and in Latin America, but. Moving from one place to another and finding the best ways that we can solve somebody's.

[00:28:20] So speaking of the best way to solve big problems, what led you guys to working with Plutus and the Cardona ecosystem more broadly? So as people will probably know Mia and eco have been involved in the car dynamical system for many years now, we were involved all the way back when you know, Emergo was really kind of getting on the scene and we're leading the team there along with another one of our co-founders AHPRA Koernke, who's not here today.

[00:28:46] And we really felt like we could take, you know, the expertise we have to the next step. And it could be more to the Cardinal and crypto ecosystem by starting our own company, which has become DC spark and. We wants to not just build great products for Cardinal, but build a great products for the crypto ecosystem because we believe, you know, a lot of times people are kind of too focused on their individual projects.

[00:29:13] And we really believe in, in building bridges and, and advancing us an ecosystem. You know, as part of that, we obviously work on Kardon a lot, but in the past, we've, you know, try working with ergo during our time at Emergo and people at the time were kind of skeptical of building bridges. Cause Cardona never really had, you know, that many connections to other.

[00:29:33] Well over time, a lot of people in the current ecosystem grew to learn more about ergo. A lot of people started getting involved in that ecosystem too, and there's been a lot of really positive, um, you know, cross-pollination and we believe that we entity spark and kind of take that the next step. So our products that work on TC sparkle be off seed launch on Carano, um, and we're, you know, dedicated very much to growing the Cardone ecosystem, but also we're trying to connect to other ecosystems and, you know, bring them, uh, you know, into the journey with us to kind of move the crypto ecosystem forward as a full, so DC spark is working with a couple of different ecosystems.

[00:30:07] This includes Selana. It also includes Herbet, uh, Nico, this one's for you. So what led you guys to have this sort of cross chain philosophy of development? So in the crypto world, uh, usually there is this fourth w what you always hear. Uh, people saying, which is straight off. So you cannot beat the best in everything you need to like specialize in beans.

[00:30:29] Really. You have something, for example, as looking to be very, very decentralized and it's doing a great job, but other ecosystem are like putting four different. Uh trade-off and this actually is something that also Charles has said multiple times. And if you guys remember, uh, there is this whiteboard from Charles when she talks about, uh, scalability, interoperability and sustainability.

[00:30:52] So we go in like multi chain ECOS also in Kanban can buy interoperability. And one of the good things for the entire ecosystem of Carolina is that everything that we are doing in other ecosystem is going to be able to connect with Carano. So. This is going to be really good, because if you think of like different ecosystem, like blockchain as countries, you want to via country, that's interconnected with other countries.

[00:31:18] So maybe you can export and import some services. And this is something really interesting that maybe there are like some specific things going on. For example, in Tara, they have a stable coin called a USD. That actually seems like they're exporting it for other blockchains and by other blockchains use in it is making stronger.

[00:31:37] So I think Cardinal has a lot to bring cough, especially with everything related to this scientific approach. So I think you talked about ability place really. Uh, we'd Cardona. And also with our curiosity that we always like to understand different ecosystem and different approaches to do this stuff. So you're trying to get the best from many ecosystems to work together with DC spark products.

[00:31:58] Um, with that being said, uh, what are some of the products that we can expect to see from you in the near future? Yeah, I can talk about that. So the first product we plan to release kind of fully to the public is called Flint and Flint is a wallet for Cardinal. And the reason we're building Flint is, is kind of two reasons.

[00:32:15] One is because as we talked about, we're really interested in interoperability. We really want the bridge to other ecosystems and, you know, technical expertise that they have and bring them to the cards and ecosystem and bring our stack to them. And the easiest way to do that was to have a wallet that you know, will work well with these other, you know, ways of operating blockchains.

[00:32:33] For example, when the other projects we're going to be working on, which we'll talk about later, it's milk. And, you know, he'll explain how all that ties into our interoperability vision. And to really bring that to the masses, you know, Flint will play a key role, but at the same time, as we do this, one of our core core philosophies in DC spark, it's really building, you know, the crypto ecosystem.

[00:32:54] And that means that we contribute a lot of open source code and we plan to continue to contribute a lot of open source code. And so Flint is a wallet for Cardona, but it's not just a wallet. It also encompasses all of the open source work that we're doing, which is also being reused by many other projects, other wallets, exchanges, dApps, and so on.

[00:33:12] For example, you know, DCS. Probably the top contributor to the rust SDK that's being used currently by basically every DAP and Cardinal is being used with basically a brick wall and Cardona, and we're building the open source and we have other projects and libraries that we're currently working on that either are open-source already or are planned to be open source.

[00:33:31] And we also write a lot of Cardona improvement proposals and actually I'm on the committee for Cardon proposals as well. So I help other people get their proposals emerged. And so, uh, Flint Nellie represents, you know, a product that helps us with interoperability vision, but also, you know, it's kind of the encapsulation of all of this huge amount of open source work we're doing to the current ecosystem.

[00:33:52] And it's helping us, you know, have a clear vision on what the Cardone ecosystem needs next and how we can prioritize getting that solved, not just for our product, but also for every other company out there who wants to build on pro Cardinal as well. So you not only building products, but you're also building out the ecosystem for developers.

[00:34:11] Very cool. Um, now, Nico, I heard you mentioned at one time before, but maybe you can give us a little bit of insight about Malka Metta. Uh, something that we have here is that, uh, even from Charles that, uh, Carvana is not just for like one specific like Bristol machine with polluters, but also the is to bring like different, beautiful machines.

[00:34:31] And there is like work with KVM with, uh, Yella an event, uh, this solar project called, uh, moon, which is implementing another programming language. So they do have Cardinals to be able to actually, uh, be open, uh, bring like different profiles of different people to the ecosystem. And this is something that we're trying to achieve with Camila.

[00:34:53] So Camille is going to be bringing EVM capabilities for Cardona, which is like pretty good because a lot of the projects that are already working well in other ecosystem could come to Carolina. So we don't need to reinvent the wheel. And Plutus developers for people that are. Understanding how to do things in the Catan approach.

[00:35:12] They can focus in, bring it new teen of agent. That's like something unique, not only for Carolina, but also for all alert, uh, blockchains. So we hope that, uh, with male Camella, uh, we can bring like a lot of adoption and speed up the, uh, the integration of like different tools, different projects into the current ecosystem and also, uh, support, uh, ADA and this, uh, pretty cool because I like all the projects will milk Camila.

[00:35:43] We are not using a new token. We are using ADA as the base currency. So when you move from Cardinal to Milky Maida using Flint, do you want to be used in corrupt either, uh, to pay for fees, uh, to use different tabs? So that way is trying to be part of the Cardinal ecosystem X. You want to feel like an extension that another different.

[00:36:05] So let's talk a little bit about extending the ecosystem. Um, now I know you guys are working with many different organizations, um, including groups like Herbet, uh, but how does this all connect back to Cardona? Different approaches are already are pretty good for like different purposes and blockchain is not that great, in my opinion, for everything that's related to the centralized identities and the centralized identity is something critical to be able to put for usage in the blockchain.

[00:36:33] So blockchains need decentralized identities, but they are not the best ones to create a centralized entities, or is this project that's a decentralized peer to peer network that actually has all the capabilities and all the. Identity. So the work that we are doing in orbit, uh, is pretty cool because, uh, we are also helping that ecosystem and us previously, uh, I commented take years to start like connecting different ecosystems.

[00:37:01] So Catalano can benefit from some of the cool innovations from Oregon and elsewhere. We can, uh, benefit from some of the key innovative. Carolina. So this is a little bit, but we're trying to do understand different ecosystem and be able to connect. So what specific products are really good too, they can support other projects and it could be like sort of language change, and we can have more of like a frail approach between different cool technologies.

[00:37:26] So obviously you have a lot going on right now. Uh, but maybe you can give us an idea of what to expect from you guys in the next five years or so. What we are trying to achieve in the next five years is that Neil Camira is going to evolve to be like a protocol that can extend blockchain capabilities.

[00:37:42] Not only EPM can be added, but older like futuristic or other technologies that are going to be created in the future. So we are going to be able to extend the capabilities of the different blockchains, the same way that the internet can be built with different programming languages. We want to be able to stick all these different programming, languages and capabilities for different.

[00:38:01] And at the same time through Flint, we want to be like the interface to connect in normal people that don't have done much like taking the kind of knowledge to be able to use all these, uh, different projects, different things without having to complicate it. Because when we are talking about Seiko layer solutions with the assets here and there, it's difficult is a complicated.

[00:38:24] And if we want to actually be there for like the normal person that maybe they're going to start using crypto for some staff that previously they use fear, or they use like the app store in iOS or Google play, we actually need to have a way better UI UX and ideas that Flint is going to be this top layer.

[00:38:43] Do I, that's going to make it extremely simple crystal clear for any person to be able to use crypto without even sometimes realizing that they are using crypto. So they wouldn't need to know any like technical concept. We've recognized ourselves a script took a system builders and ecosystem does not happen without our community.

[00:39:03] So one of the step-by-step process that we're doing is really understanding our community in this case, like our dental community for us is fundamental and of high value because the founders are very related of course, to the Cardinal community. But also that community have give us insight and information that help us generate the product better.

[00:39:22] So how did we do it? I think even though it's a challenge, part of building a strong ecosystem can by generating alliances and network and listening to whoever is actually using our product. So I think it comes a lot with listening conversation, building a strong net. And also becoming this connector, which is valuable for them and also for us.

[00:39:46] So with that being said, how do people get involved with DC spark? Or how do they connect with you guys? TC spark has a lot of reach in many places who were involved with improvement proposals on Cartano were involved open source work. We have participation in a lot of Twitter spaces, telegram all those groups, but we also have our own communities.

[00:40:07] So you can follow us on the TC spark Twitter. You can join the DC spark discord and we try and be kind of omnipresent. And so you can easily find us, you know, wherever fits you best with be you a developer or just somebody who wants to be involved in the ecosystem. Okay. Okay. So for all of our viewers, the channels will be tagged below.

[00:40:25] So make sure to go and check out the show notes, DC spark. Thank you so much for joining us. And we're looking forward to hearing more about what you're up to in the near future. So max has been out on his regular mission meeting, just some of the projects building on Cardall. Now let's head over now and handle.

[00:40:44] So I've been continuing my journey this month, talking to some of the many projects building on Cordato so that you, the community can also find out more recently. I spoke with Carter shift and power muesli swap chip drops and NFT maker. So let's jump right in. Kind of shift is a community run launchpad that raises funds bills and accelerate startups that are solving social as well as environmental issues.

[00:41:12] And to put it in very understandable terms, think of it as Kickstarter plus Y Combinator put together, uh, so matters is the first company. It's a product and startups studio that's basically helps new businesses to succeed in scale. So they've supported more than 150 a company startups over the last 14 years.

[00:41:33] We also have steam, which is a spinoff from a very known renowned engineering school in France. And, uh, and yeah, the third company is smart chain, which is a blockchain engineering company. Um, the, we we've been working on the proof of stake blockchain for the past two or three years trip drops mission.

[00:41:52] Is, we are a car Dano token dispensing service. Uh, we offer an intuitive platform for token issuers to, uh, distribute their, their token. Um, so whether it be a meme token, a utility token, whatever, we allow the user to come to the platform and withdraw the tokens of their choice and cover the a UT XO, along with the processing.

[00:42:21] The mission of empire is to provide a solution to the housing challenge in Africa, through the provision of decentralized finance, the challenge for us is to find new ways and mechanisms and new technologies to address this seemingly insurmountable. And that's our mission is to overcome that we are a decentralized exchange on the Caetano network.

[00:42:42] So Missy swap is a place where people can meet to trade tokens, but it's different from other decentralized exchanges to see on the Caetano blockchain is that we are based on the other book model. That means that people are able to place limit orders. They can follow the audits and the other book and get the better or deeper view of the current market than what the, whether the price is going to increase or decrease.

[00:43:03] And if you make it in a nutshell, it's a mentoring tool built on Kadana. And, um, we have a pro solution. So artists and non and people can come to our platform and upload their assets to an F T maker. And we meant on demand and FTS so that people can, uh, take our API implemented in the website and start setting through our payment.

[00:43:26] What advantages does spilling on Cardona offer your project? Uh, why in particular, is it on Cardona? Well, there's three reasons. One is that, uh, we see a huge of value alignment in terms of what we're trying to build as well as what Cardona vision is. So I think a lot of it is driven towards creating impact, but also enabling more people access to these technologies and are loving them to participate in creating impact.

[00:43:54] That's one, two is there is also an alignment in terms of the kind of projects. So if you look at Cardone or Africa, I mean, it's a huge market for us because it's also, there is the French speaking part of Africa and, you know, being a company that's based in France, we have a lot of access to do, uh, projects with them.

[00:44:14] So there is a huge, a French community here that wants to be part of . And we really see ourselves at that bridge trying to enable that to happen. And I three, I think we're building on, I like it's the future for impact. And we strongly believe in the vision that Cardinal has for the future. Right? So those are the three main reasons on why we're developing on CarNow and what we see happening with this relationship going forward, the advantages of building on Cardona for us, or.

[00:44:47] Um, it's pretty distinct how we work in enabling offsetting the costs for projects. What that translates to users is users are able to pull numerous assets for a very, very low relative and cost is that would cost them on other chains, you know, the technology and the core principles of science and how.

[00:45:09] The ecosystem plans to scale all the components are there for us that make it a sound system. We want to build a legitimate business in Cardona is the appropriate foundation upon which to do that. I don't think we could really emphasize enough how important the extended UTX. So model is to, to what we're doing, you know, for, for ages in the space in general TPS transactions per second has always been a source of contention and everybody's got to have the best TPS.

[00:45:34] And this really does prove that TPS is not the end all be all. It's really kind of a blind metric. How many transactions per second is irrelevant when you consider we have all these inputs and we're sending out all these outputs and we're handling three customers at one time. So it just, the sheer volume of what we can actually transmit on the chain is pretty phenomenal.

[00:45:52] Impact chose the Kadana blockchain for number of reasons, the, this first rare. The environmental aspect, that if we're going to build 50 million homes, which is our end goal, we have to make sure that we support the environmental aspect of that. So we have to practice what we preach. We were also attracted to the academic rigor because ours is a financial system.

[00:46:14] So we have to be strict in the management of that. And the third element for us was the really exciting community that came with it. The huge bonus was the African focus for the community. One of the big advantages of the Takano network is that it's based on the, you takes a model and it has very, um, rigid research in how to, how to use that.

[00:46:41] And we figured that with this very elegant approach to translate. We can develop this decentralized exchange on the audiobook model in a very typical fashion. There's also a great community, which we were astonished by how awesome, like the feedback from community members was. Yeah. That's that drew us to it.

[00:47:04] Tonnato like we, we want to enrich this, this ecosystem. I think, uh, building on Kadana is it's very different from building on any other blockchain. And there are many differences in the way that the protocol is structured on a very fundamental level. And I think that it's, uh, in some parts it's a lot more difficult, but a whole, um, decision to go with this, you know, Bulletproof system of peer reviewing, every single thing that Kadana was doing makes it very easy for us to build solutions, which are actually.

[00:47:34] Um, secure and build smart contracts, which are actually secure. So how's it going? And what stage are you guys at now? So basically a roadmap started six months ago in this, in September of 2021. We went through a period of a private sale for which we managed to raise 1.5 million and post that kind of momentum.

[00:47:56] We'd only focused on building a community. So we've managed to do that on discord, where we have grown into us six times, uh, in a period of three weeks, followed by a six K following on Twitter. What we expect to do in the Q1 of 2022 is actually our. Release a launchpad beater version for crypto enthusiasts, with the option of being able to stake for the projects that they support, as well as they'd be allowed to score these projects.

[00:48:26] Um, the reason that we're having this launchpad come out, um, is because we've seen a lot of interest from impact projects and change makers to want to be part of Carter shift. And, um, I know that I'm not allowed to publicly say the names of these projects, but they will be announced soon. So keep updated on our socials for that.

[00:48:48] So it's going pretty well. Uh, we launched roughly 14 days ago and already we've seen 60,000 withdrawals and, you know, It's amazing. People are coming to cut down on every poll, just to see that, oh, there's another type of reward that they can withdraw. And we had a very unusual effect on the Cardinal ecosystem.

[00:49:07] The way people are actually taking their funds out of the exchanges and then putting it into staking. And we know this because there's been a lot of support requests saying, Hey, why, why can't I get any rewards? I don't see anything. And we have to explain to them and educate them. Did you just start staking?

[00:49:23] Cause I can see that. That's probably why you're not getting any rewards, which is fun to see that we're actually having a direct impact on the users. So for us, because it's a real fight. We had two real challenges as one we had to prove to the crypto community that we could deliver on the ground. And we also had to demonstrate to the developers and to the people on the ground, to the traditional players, that the crypto community is not just a bunch of, you know, Monday laundries and drug dealers.

[00:49:52] And actually that there's a very real use case for this kind of technology. And it presents a very real opportunity. So in order to do that, we actually applied for, to catalyst for, for funding to, to demonstrate that, um, which we successfully did and we've delivered four houses in undefined. Through project catalyst, utilizing the new tech, et cetera.

[00:50:13] So we're really excited around that and you demonstrate kind of how quickly, how much quicker we can move and how much more effective things can be. So right now we're still in, we're in the fundraising stage so that we can start the platform development. We know it's a long road to go, and we're just taking those first, first baby steps to get the process going and to, and to get the next stage of the project underway.

[00:50:36] Swap launched back in November, 2021. And since then we managed to gather a big community around our product. We have more than 15,000 unique traders already on our platform. And based on the tremendous feedback we get got and feature requests, um, the, the managed to build that. Original house smart contracts, Missy swab, V2.

[00:50:55] And we are very proud that we partnered with M labs where the audit is currently ongoing, ongoing, and hope that we can launch it in end of January, 2021. And one of the true benefits of Missy swap is that we are truly decentralized exchange. So the artists can be matched by any matchmaker, which is different to other approaches.

[00:51:14] So, and if tea maker was successful, yes, last year, but, um, in January now it's exploding. So we have more signups than ever more people than ever are using our pro tool. And we are really diving into the next state of NFTs. Um, we are convinced that we will, yes, we will have those 10 K randomize drops, but we think a bit, a lot of those artists and people who signed up now we're bring additional value to cut out, especially the financial.

[00:51:46] Massive success. And we can't wait to get started. So to launch and to find staying power are two different things. So post-launch, what are some crucial milestones on the path to becoming an established part of the ecosystem to become an established on the ecosystem? We have mainly two side of our world map to first is our product roadmap.

[00:52:06] So basically the launch of a launch pad, which will be in Q1 2022 was the first projects on it. Courtesy is, uh, was, uh, was berm with DDT coalition of three companies, which have complimentary skills. So how we can, we create the good ecosystem around us with DeCarlo community, with the people on the ground, because we already working in Western Africa and south America, and we are not on the ground yet because of the three cock book companies are mainly in France, but our partners are there and we need to find the right partners to be able to.

[00:52:39] Scored a project basically identified the right projects and the right entrepreneurs scored a project, assess every, everything, and be able to support the projects also locally. And we've been already having a lot of talks, uh, in several countries, uh, to us, to how we can provide our technology and our infrastructure.

[00:52:59] It's mainly the biggest part of it because, uh, uh, as we are accelerating the process as the project, we need to be able to, to, to accelerate more than two or three projects every quarter, uh, which will be the case. At first, our first milestone we were going to spending most of our time is establishing a legal operational framework that will enable drip drops to compete on a global.

[00:53:23] And so that's number one and we're moving very fast. Uh, projects are going to have to enable incentives for their users in some way, shape or form. You're going to want to issue your users, some sort of reward or achievement. You're going to want to know what their progress is. We're going to enable you an API where you can do that.

[00:53:39] So then you don't have to worry about token distribution. You just focus on your project and, um, drip drops will enable the tools for you to incentivize your users, to make your products more compelling. We didn't want to be the gatekeepers of which project gets onboarded and which gets pulled it off.

[00:53:56] So we wanted to create a token that is, um, very well distributed to the community, and it could be used to actually govern the platform. And what people don't realize is that we might be the only if not the first to actually create a token that is 100% distributed to the committee. And it wasn't designed that way so that we will have no saying the platform, hopefully walking towards their doubt route and with working with some of the smartest minds in the industry, trying to figure out what is the right way to do coming from the housing space and real-world development.

[00:54:31] We know it's a long-term process. Um, so absolutely we used to it. So, so for us, that that's really part of that, that process to ensure that we are able to deliver an on the ground. So in, in, um, Q1, uh, obviously the first, first one is the, is the token sale. So in terms of the fundraise, um, and then also the NFTs.

[00:54:52] So it's to then expand the number of houses that we can deliver. So to demonstrate that, and then by Q3, the objective is to have the MVP, which is then the financial flow. So that's to have the value flow, um, as well as, so we will then have the necessary tokens and infrastructure in place to do the MVP by Q3.

[00:55:12] So that's a key milestone for us. So not a lounge. We are astonished that we have a really fast increasing, uh, user base and we assume landed being on the top position of, of the most used smart contract on the, on the whole blockchain. Our philosophy for this is to, to stick to what we did, which is deliver.

[00:55:36] We are running out the version two off a smart contract, which will improve the liquidity and, uh, which will adjust or improve the experience of using our other book decks. Yeah. We are going to increase the community engagement and the decentralization of our project with a launchpad and staking and government governments features.

[00:55:59] So what we're trying to do is really to professionalize and grow the system and create a team to build something of a larger scale, and really go from a solo, deaf project to a real company, which then can deliver on really large projects. And, you know, around that, um, there are so many things to do. You have to grow in a community, you have to, um, basically educate people about your system and your tools and what you're actually contributing to Caetano.

[00:56:28] So I think these are really the milestones that we're tackling right now. How do you see your products needs? Developing on car Dano over the next few years and into the longer term. And what problems do you feel uniquely able to address? We would like to set a standard for how tokens get distributed, or we want to make handling your tokens as easy as possible.

[00:56:50] Just let us know who they need to go to and w or where they need to go. And we can do that with accuracy and precision, really cool new features that are coming. So right now you can stake your ADA to a pool and get rewarded at NEDA where we're going in the future is maybe you have an NFT project that has an NFT.

[00:57:11] You can stake it to a pool that's associated with that NFT project and then receive some of their fungible token and response for that, that staking. So we're kind of expanding the whole concept of staking on current. Yeah, I think we're, we're uniquely positioned to facilitate a huge reduction in friction for projects that are coming from other chains, or we can greatly reduce, you know, that stress and friction for those projects.

[00:57:38] So they can focus on the things that they're trying to build. And, you know, drip drops can handle that distribution aspect of the, of the. That project for them. So the niche that we're addressing is very specific actually, because, you know, there are a lot of players. There are a lot of generic kind of platforms, and we are specifically focused on the longer term aspect of, of defy and enabling the liquidity within that longer term view, if you like, because housing is different to other kinds of, of financing.

[00:58:09] So we that's very much our niche focus. So another niche is to really have the relationships on the ground to know and understand that so that we can start just like a Donna is developed, where it started off with, you know, managing and controlling the process. And then gradually decentralizing, we have the same objectives.

[00:58:27] And so really for us, it's around building that out in terms of relationships with not just other crypto players, but also. Finances, uh, traditional funders, DFI is who've played in the space. This is Rob is in the, in the core business of being a decentralized exchange. And I think the need to, for people to meet and to swap things has been there for centuries, and it will also continue in the future.

[00:58:51] And that's why I think that the defy space or the space for Dexus in general on the Kadana blockchain is only going to grow. And we hope that muesli swap can be an integral part of this. So just being the place for people to come and to swap these tokens, I think the niche of NFT maca is, um, will be NFTs and, uh, closing this gap between, um, people outside of the community and the technology.

[00:59:16] So I think this will be our niche and this will be our main goal. So what we try at NFT maker, what we try to do is we try to close this gap by educating people and by explaining to them. Kind of blockchain Kadana is green blockchain. And in addition to that, how NFTs could work in the future. So imagine yourself in like ticketing or something like, um, bringing fine art to the blockchain.

[00:59:42] Those are the things that are already happening. Not only building, you know, a minting tool, but we're also building a whole ecosystem around the minting and around the NFTs. And we have plans to basically expand this ecosystem, all building upon our foundation of NFTE makeup pro. And it's really important for us to, um, make, you know, the whole user experience as easy as possible.

[01:00:02] I want to thank all the projects for their time today and for coming on the show to share their vision and mission with the community. It was great to speak with you all. So that's about it now for January. Remember, you'll find links to many of the people and the projects we've covered today, down in the show notes below.

[01:00:19] Also make sure you check out the blog where you can read more about Cardona's plan for scaling in 2022, how we're improving the developer experience. And if you're new to defy, there's a piece there which should help demystify things a little. And remember, you can always find the latest on development in our weekly development updates from decentralization, peer to peer to networking and addressed.

[01:00:38] You follow us on Twitter, and those will land every Friday. That's it for this month, we'll see you at the February. Mid-month update.

