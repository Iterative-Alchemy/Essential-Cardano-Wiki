# Mid Month Technical Development Update - February 2022

[00:00:00] Hello, and welcome to your mid month update, where we do a deeper dive into car Dano development and delivery with no further ado. Let's meet the crew. Now we've got Niger. We've got Kevin and we've got John to tell us a little bit more Nigel. Let's start with you February a busy month as always Tim. I think it's worth just taking a moment before we dive in and just reiterating, explaining again how we've matured as a company to do major releases that.

[00:00:27] So we, we concentrated this year to focus on three major release months so that we've got fixed dates for the end of February, end of June and the end of October. Now this is really important. And I think this is a big step forward for us as a company, because it enables everybody that's involved in our ecosystem, all our downstream applications and products, an indication of when they might have to do an update to that particular pieces of software.

[00:00:54] So it also means that for us internally, um, on our core infrastructure, we've got our engineers that are focusing on these different dates and understand and can actually develop Ida tests and address, uh, the challenges as we go through and build towards these key releases that come through. Okay, great.

[00:01:14] Thanks Nigel. So maybe let's just dive straight in and you can take us through some of the contents of that release. Sure. We're highlighting some of the key features that were included. A lot of it is focused once again on improving our network performance, but we've also building more and more out in terms of our smart contract offering.

[00:01:32] So we're improving our smart contracts, ecosystem, infrastructure, work, that test tooling and all sorts of other bits and pieces that they adapt developers and community will use, um, going forward as they build out all of their exciting new applications. As we step through everything in February, Kevin and John will bring in all the different technical detail.

[00:01:54] And then after that, we'll give you a sneak peek of what we're, uh, what we're planning to do in June. So let's, let's just jump in. Let's have a look at the core platform. We start off with one of the first things that's, that's included into the major release. At the end of February, the node release in 1.3, three did include a lot of this data structure, mapping and redesign.

[00:02:14] Which has improved the sink times for, uh, Daedalus and a number of the other applications that are running on the network, the node release 1.3, four builds and all the good work that we've done with 1.33. Um, but here to tell us a bit more, is Kevin Nigel. So a huge shout out to the noting. They've been doing a tremendous amount of work here to make everyone.

[00:02:35] Uh, lives are better through improving the performance of the node. And we've been seeing a huge strides, uh, forward that, uh, there are some big improvements have been made, uh, in particular to the, uh, memory representation that the node. About 12 all together. We've got a new, more compact data format. Uh, we have smaller transaction inputs and outputs in memory, uh, snapshots, easy, more compact representation and values are being shared during the serialization.

[00:03:06] And all of this means not only less memory usage. Uh, but also very importantly are fast to node and that's what we're all, uh, focusing on, uh, at the moment, improving the overall performance and experience for our user base. There is one wrinkle with this, which is that the first time I. Use the new version of node.

[00:03:27] You may experience a slight longer than usual resynchronization time. That's only a one-off and there's a new version of dateless dateless flight, uh, which aims to make that more obvious to the user. So you to get better information about exactly what is going on under the hood as using new versus dateless.

[00:03:49] Um, but, uh, maybe I should hand over to John. Who's going to ask a bit about our new CDL former. When you have, um, data in a computer's memory, it tends to be instantiated is the word, or when it's created it lives, uh, as an object or a structure. And there are various formats for how, um, data lives in a computer's Ram when it's being used by the program that's created, it turns out though the way computers store data, when they're executing is not necessarily a great way to store.

[00:04:20] Um, when you're trying to move it across the network. So when we want to take some, some data out of the computer's memory and pass it onto our neighbor, as we do, when we're propagating blocks in the blockchain, um, or other messages across the network, it's important that we take the representation out of the computer's memory and, uh, go through a process which is known as serialization in order to take that data object and represent that in a way that is efficient for transport.

[00:04:46] Um, The serialization approach we take is known as CBRE, which stands for a concise binary object representation. And it's loosely based on Jason, which folks might know from web development. Um, this idea that you have text-based key value pairs, but seaboard uses a binary format. So it's represented as pure ones and zeros.

[00:05:06] So the change that we've made in particular is to see DDL and CDL is concise data definition, language, and re. You can think of it like a schema for C4. So we've tried to tighten up the schema for our underlying serialization representation. And ultimately what all of this means is that when we're sending data across the network, uh, we do so more efficiently and in a more compact way.

[00:05:30] Okay. Thanks, John. Um, next step is to be looking at the further future of our, uh, wallet, infrastructure. Um, and I know we've made a lot of advances and, and, um, improvements in that area. To start off with, to improve the functionality in any of the front end products. We have to look at improving the infrastructure.

[00:05:49] So we're introducing the infrastructure capability for multisignature this time round at the end of. Um, and this will incorporate the ability for parties to be able to, uh, complete transactions with multi signatures, which might be used to validate transactions votes, or many other contracts or other possibilities.

[00:06:10] Kevin, can you help us to understand the other benefits that we can get from this multi-state is a really cool feature. We've we've had it around. Um, since, um, Shelly, as, as a standalone feature, uh, there's new capability, uh, in Plutus of course I basically, what multisig is all about is for two parties to a transaction, to both agree, are that the transaction is.

[00:06:35] So this allows you, uh, to, uh, for example, have two people signing off on payment, uh, transaction or for, uh, two parties to agree, uh, that some contract has been fulfilled. All these kinds of things. Very, very. Uh, feature from the real world perspective. And what have been doing in the node is to improve that capability.

[00:06:59] So there's been work on enhancing the way that the signatures are done are from within the notes. So this makes it easier for people to use the multi-site capability. In addition to, to the improvements, we've got a multisig, we also introduced our reporting a benefit and fees. Um, via the leadership schedule and this enables us to actually get visibility of which SP SBOs are going to be producing the blocks next, um, and helps us to be able to report on it, which is useful if you're a duct developer to see what transactions are getting processed.

[00:07:33] And if there is a possibility that you might need to resubmit a transaction. But it's not just that in terms of the Corp platform development, we've also been lucky to our smart contract capabilities and we've got some cool new features as well, coming out from that area. Yeah. So one of the things to highlight is a local transaction monitoring module missed this, came out of discussions, uh, that happened at the Cardone.

[00:07:57] Uh, last year, uh, so brilliant event, by the way, uh, lots of community engagement, people are getting together are focusing on developing our new ideas. I, our engineers working with the community, um, and, uh, bringing out some really good things of which some people receive prices. So guys participate in this.

[00:08:19] Don't just sit back, join in, do things. There's opportunity. There are opportunities. There are few to make a real difference to the community. So what is local transaction monitoring? Well, this is one of the things that, um, people have really been looking for. It's quite a simple idea, essentially what you need, what you want is some capability to.

[00:08:40] Say how's the node process to transaction without having to wait for this, to pop up in the chain and figuring out has your transaction gone through or not. So the low transaction monitoring that. People study the mentor content lets you see what transactions are being presenced by the node tells you instantly.

[00:09:03] Yes. This has been processed or no, it's not yet in the mem pool. And then you can write applications on top of that, uh, that. Do more sophisticated things. So it's a great capability. It's to be honest, it's not very complex. Uh, it's a relatively small piece of term. So even small things can be really, really useful guys.

[00:09:26] This, this really makes difference. And it's been incorporated now, um, as part of the origami office, our framework. So you can, if using oatmeals are, you can pick up on this capability, you can use it. So. So, of course, in addition, our night, we should also discuss the auto calculations for Bluetooth scripts.

[00:09:50] Would you like to give us an update on that? Sure. Kevin, this is a feature that we had when we first launched a Alonzo and what we've done is we've listened to the community and we've been able to actually improve on it. And that release is going out at the end of February as well. So it's just as a reminder, it's a, and also calculations.

[00:10:08] To be able to understand the transaction size for polices scraps, which is incredibly helpful if you're a developer, because then you can understand how you're going to get things onto the chain and actually how your DAP is going to perform and how many things you can fit into a block. Um, and although all that.

[00:10:24] Things that you need to do as a developer. So last but not least parameter updates. Now, John, you've been managing this program and these improvements to the network steady and sure. But perhaps you can give us an update on what's happening next. Absolutely. So, uh, 2022, uh, is all about scaling out layer one on Cardona.

[00:10:41] And I've mentioned that before, so let me just remind viewers what we've done. We started off at 64 kilobyte blocks. We moved to 72 and then more recently to 80 kilobytes. So we've already made substantial size improvements to the block size. Um, and then in terms of Plutus Plutus requires resources, um, both computational or CPU units and memory, uh, units in order to do useful things would apply to school.

[00:11:06] We started off with 10 million units on Plutus. We moved to 11.2, 5 million, 12.5 million and more recently to 14 million. So we've literally had a 40% increase in terms of the resources, memory, resources, I should say, available to Pluto scripts. So lots of quite serious improvements there to. We're going today to post another change to the, to the network parameters of main net.

[00:11:29] We're now going to focus on block level limits. So when I looked before I spoke about a block size, I spoke about memory limits. Those memory limits were per transaction. And of course we also have. Pear block limits in both our CPU units and in memory units. So we're going to raise the per block level limits so that folks can not only write scripts that do more, but can put more of those scripts into our now bigger blocks, looking at parameters, John, another area of fairly intense discussion amongst the SPO community has been around the decentralization parameters.

[00:12:03] And I understand that's something we're also looking at very, very closely now. Absolutely. Tim, we had a call recently with over 250. And it was really a learning experience for me. It was the first time that I had FaceTime with so many of them. Um, We're listening at IO. We understand that we, that we have concerns in the community about certain decentralization parameters and in the coming weeks, um, we're going to provide further feedback and clarity on what we do next with these parameters.

[00:12:28] So Nigel, rather than going too deep into what's coming in June, perhaps we can just do a bit of a thousand, a thousand meter view for now or a thousand yard, depending on where you're watching this from, just to give people a little bit of a taste about what we'll be going into in more detail in future.

[00:12:41] Sure. Thanks, Tim. I'll just bring up what we're looking out for. The gene hard fork. We've named it a vassal. This is our major release for the end of June. There's lots of good stuff to look forward to in the June major. We've got a lot more work that's going on for the Plutus optimization work, which is going to really help the duct development community.

[00:13:01] And also we've got some really exciting things around the network efficiency and they're much awaited a pipelining feature. So why is it? Didn't do a deep dive into it right now. We'll be saving that up for the end of the month, 360. Okay, thank you very much, Nigel. And as Nigel says, we'll have lots more information about what's happening in between now and June.

[00:13:20] And of course in the June hard fork and future additions to the show. We also had a chance this month to meet with the hydro team. I everybody I'm Sebastian, a developer and technical manager on hydro here at IOG and happy to be here that old guy's name is Martinez. I'm also working on the hydro projects, doing the breech between the research and engineering to Sebastian.

[00:13:43] So you've recently published a blog post to give an update on the progress of hydro and also. Bust a few myths and misconceptions. Perhaps you can tell us a bit more about that. Yes, indeed. So we wanted to write this book force for quite a long time, to give some status updates on, you know, what we're doing, where we're at, where we're aiming at with this project, but also to address a few, a few concerns we had from observing people, talking in a community and social media and seeing things.

[00:14:13] So I want to do things right. We've seen a lot of this 1 million TPS being called out all over the place. And we've been talking about TPS several times already saying that it's not really a good measure to comparing blockchain, right. Because the. All of them have very different way of defining a transaction.

[00:14:29] So it sounds actually on Colorado is not the same as it comes action on another platform. And even construction within Cal Danno are already very, very different, right? Smart contract transaction versus a just, you know, pure payments transaction is it's quite different. So it's not really good for looking at things plus, um, in the case of Hydra, right.

[00:14:50] Very similar to having ledgers that are quite isolated from one another. Right? So looking at all those ledgers and summing up all the possible TPS of oldest independent nature together, and you, you can read. Any numbers, you won't write 1 million, 1 billion, you know, whatever you call it. So we don't really like looking at that.

[00:15:10] And we think it's much better to look at things like the system and time of the transaction, for instance, or the actual amount of data that is being transferred over a period of time. And this sort of benchmarks are much more useful tourists and meaningful as well seconds. Right. We also wanted to address the fact that it's hydrolyzed not only about FPOS and actually that SPLs are probably the less likely candidates to be running hydro head in the first place.

[00:15:40] Right. Uh, hydro head is, is, is something. That anyone can rerun. It might need to be someone with his Dallas wallets or a lightweight provider, or even Saudi's provider. Like, you know, you name it. So where do you hold it to to make that clear that this is not just an SPU thing. This is a Potter construct, a, a tool.

[00:16:02] And we want to encourage people to build this infrastructure off the Yatra solution on top of using. So Sebastian you've also recently published the hydro roadmap. Perhaps you want to dig deep into that and tell us a little bit about the, uh, the progress there. Of course then, and terms of the roadmap we want to be transparent as well.

[00:16:21] So this is why we opened up what we internally planned out to be essential steps on a high level, uh, across, uh, maturing. What we have right now from a developer preview, as it was in September over, uh, first prototypes, really making it matured. Um, make it capable to run on the F on the dyno test nets and eventually reached may net maturity.

[00:16:44] The public roadmap is available on GitHub, and you can see on this dimension, for example, how multiple features actually comprise new releases. Uh, we have even made a recent release 1 0 3, and, uh, you might want to check out all the descriptions on what we do, what we edit, what we choose. And there'll be many more releases along as we, as we matured, uh, the Hydra had, or the hydro note capable of hydro had protocol further along until eventually 1.0.

[00:17:12] Of course, this is something we want to do because really to be transparent, what we're building, what we're working on and even discussed with the community and how PR how important some features are for, for one or the other use case in the beginning. It's of course, most of the things are essential, right.

[00:17:28] But as we further progress, Um, many of the extensions of the advanced protocols, which are based on, on Hydra head are up for discussion. And we gladly do that on open platforms like GitHub and also other channels. And of course the community contribution to the project is going to be key going forward as well.

[00:17:46] Perhaps you want to tell us a little bit more about that? Yeah. As can be demonstrated here. Right? If, if GitHub, um, roadmaps, right. We also have like get up discussions. Um, we have a discord channel, uh, which is on our IOT technicals. Um, you can ask hydro channel's name. You can ask anything. If you want to be informed on a high level, we can point it to a resources to our documentation maybe, or, uh, people also educate themselves.

[00:18:10] Uh, there, uh, of course there's also a stock change. You can ask them very concrete, uh, questions you have while even trying out. And very much encouraged, right? So it's really, we want to take you on this journey and all to get it built, uh, as scalability solution for Cunanan. So we'll have a lot more from Mathias and Sebastian and over the months ahead to keep you fully up to date with what's happening with hydro.

[00:18:34] If you want to read that blog post and make sure you check out the link in the show notes before we'll also have a demo for you. So keep an eye on our social channels and we'll share that as soon as it's available. So gentlemen, thank you very much for joining any final thoughts before we leave. Maybe we want to just remind people that what you are currently building and aiming that's releasing.

[00:18:52] Is it really your first step in the hydrate journey? Right. Hydra head is one of the first protocol of the high coal Hydra family. We want also to get his rights right. And to make these as useful as possible for the community. So please engage with us. These curled guitar or any media that's that is most convenient to you because the feedback is crucial to be able to write thing.

[00:19:14] Great. Thank you, Mathias. And all the links will be in the show notes below. Thank you very much, gentlemen, and we'll see you again very soon. So that's it for another month of the mid-month update, please make sure you put in your diary the last Thursday of this month for the car 360 full show. Thanks very much for joining us.

