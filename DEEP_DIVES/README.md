# 🐋 Deep Dives

## Description

The Deep Dives format is designed to give all participants a taste of what it feels like to work on the big and meaty Open Problems by contributing directly to them in an intense design session - evaluating all the possible solutions, their advantages and shortcomings, and documenting the results.

This type of discussion is core to the genesis of IPFS. We’ve done multiple over the years which have yielded many valuable results such as IPLD, PubSub, GraphSync and other advancements to the original IPFS protocol.

These design sessions are not about explaining how things work, they were focused on finding the solution with the knowledge and resources we had available.

## Instructions

### Overview

- **Objective**: Deep knowledge transfer that only happens in synchronous interactions.
- **Activity**: In a group of max 4 people, dive deep on a complex technical design topic.
- **Outcome**: The output of each of these sessions would be a RFC like document (can be very raw) that describes the proposed solution (even if with known shortcomings), or it could be a map of all the important concepts, obstacles, and related topics you covered in the session.

### How

- **Duration**: 1:45h

On the day, this is how y'all will Deep Dive 🐋:

1. Large cards with [Deep Dive topics](#topics) will be displayed
1. You **choose a deep dive** to participate in and **take a slip** from the card
1. Groups assemble and the **topic owner explains the problem**
    1. Existing solutions should be briefly enumerated!
1. Groups discuss their topic
    1. New ideas are suggested 💭
    1. Groups **aim to come up one good solution**
        1. It can be a completely new solution or a change/fix to an existing one
1. After 1 hour, groups take a **10 minute break** (phew) ☕️
1. Groups reconvene and **send a PR to [ipfs/camp](https://github.com/ipfs/camp/tree/master/DEEP_DIVES) with their proposal**
    1. Didn't come up with any solutions?
        1. List your ideas, and why they weren't suitable so we can bootstrap future discussions
1. Groups **customise their slide for presenting their solution** at the graduation ceremony
1. Groups are free to iterate on their PR or their slide overnight

The next day (graduation day), this is what happens:

1. Each group gets **2 minutes to present a summary of your solution**
1. You get **one slide** in the shared slide deck
1. The best solution(s) win an award 🏆

### Topics

| # | Topic | Owner | Description |
| :---: | :--- | :---: | :--- |
| 1 | [Private DHT](./01-private-dht.md) | **[@kishansagathiya](https://github.com/kishansagathiya)** | Improve privacy of the DHT Protocol |
| 2 | [Scaling up the DHT 📦](./02-scaling-up-the-dht.md) | **[@Kubuxu](https://github.com/Kubuxu)** | What can we do to optimise the performance of our DHT? Are there alternatives? |
| 3 | [Reducing the information leakage on a libp2p dial](./03-reducing-the-information-leakage-on-a-libp2p-dial.md) |  |  |
| 4 | [Locking the IPFS repo for concurrent access](./04-locking-the-ipfs-repo-for-concurrent-access.md) |  | How do we manage concurrent access to an IPFS repo when we have multiple tabs on the same domain or web workers or service workers? How do we avoid being too restrictive (i.e. locking everything) whilst guarding against race conditions and concurrency problems? |
| 5 | [Identity for DApps 📦](./05-identity-for-dapps.md) | **[@satazor](https://github.com/satazor)** | What are the next challenges post IDM? |
| 6 | [Live Streaming Capabilities through IPFS to X thousand](./06-live-streaming-capabilities-through-ipfs-to-x-thousand.md) |  |  |
| 7 | [Upgrading the HTTP-API to a RPC API](./07-upgrading-the-http-api-to-a-rpc-api.md) |  | We desperately need a new remote API https://github.com/ipfs/http-api-spec/issues/116 |
| 8 | [Offline First](./08-offline-first.md) |  | How can IPFS currently be used to support communities with little to no network bandwidth? What improvements to the protocol would make IPFS offer better solutions to these challenges? |
| 9 | [Package Managers: What Now, What Next? 📦](./09-package-managers-what-now-what-next.md) | **[@jessicaschilling](https://github.com/jessicaschilling)** | Community evaluation and ideation session to recap the current (as of late June) state of the IPFS-enabled package manager landscape, discuss happiness and pain points, and do some ideation/co-creation  around the direction of our next rounds of package manager efforts. |
| 10 | [IPFS on Mobile](./10-ipfs-on-mobile.md) | **[@carsonfarmer](https://github.com/carsonfarmer)** |  |
| 11 | [Private content on IPFS 📦](./11-private-content-on-ipfs.md) | **[@ianopolous](https://github.com/ianopolous)** |  |
| 12 | [Building the IPFS Community](./12-building-the-ipfs-community.md) | **[@stefanhans](https://github.com/stefanhans)** | Community, evangelism, engagement, on ramp. |
| 13 | [IPFS for websites (static, dynamic, search, etc)](./13-ipfs-for-websites-static-dynamic-search-etc.md) | **[@dietrich](https://github.com/dietrich)** | What are the best practices and open questions for using IPFS for static / dynamic websites? What about indexing and searching? |
| 14 | [IPFS in blockchain](./14-ipfs-in-blockchain.md) |  |  |
| 15 | [Open research problems in IPFS](./15-open-research-problems-in-ipfs.md) |  | Content routing |
| 16 | [Revocation/Rotating of IPNS Keys](./16-revocation-rotating-of-ipns-keys.md) | **[@aschmahmann](https://github.com/aschmahmann)** | The idea of using a public key to identify mutable data is cool, but what happens when that key becomes compromised? |
| 17 | [Building Reusable Data Structures](./17-building-reusable-data-structures.md) |  | IPLD and IPFS allow data to be portable and reused between applications. What are some good behaviors or work flows to promote data reuse instead of re-creation. |
| 18 | [Service and Content Discovery under Partition 📦](./18-service-and-content-discovery-under-partition.md) |  | We tend to think of our systems as operating in either the “global internet” or a “local network”, but the reality can be more complicated than that. Do our systems meet that challenge and if not what would we like them to do? |
| 19 | [Referencing HTTP/centralized web content from IPFS 📦](./19-referencing-http-centralized-web-content-from-ipfs.md) |  | Currently data is available to the IPFS network when a node advertises that they have data and provides it upon request. Would it be useful if we could advertise data provided by HTTP? What are the tradeoffs and mitigations we would need? |
| 20 | [How can IPFS support sharding 📦](./20-how-can-ipfs-support-sharding.md) |  | How to best pin an arbitrary part of a DAG https://github.com/ipfs/go-ipfs/pull/5142 |
| 21 | [A better HTTP API](./21-a-better-http-api.md) |  | Upgrading the IPFS HTTP API to be more RESTful and easier to use |
| 22 | [Garbage Collection how to make more efficient large block stores 📦](./22-garbage-collection-how-to-make-more-efficient-large-block-stores.md) |  | We currently stop-the-world and collect, what's involved with incremental, generational. Could we use a separate datastore, something else? |
| 23 | [Connection management](./23-connection-management.md) | **[@jacobheun](https://github.com/jacobheun)** | How can we better manage connections in libp2p to create stable overlays and reduce the impact on connection resource consumption? |
| 24 | [Replication protocol 📦](./24-replication-protocol.md) | **[@hannahhoward](https://github.com/hannahhoward)** | How can we more quickly sync a DAG or part of a DAG between two nodes? A compliment to bitswap, affectionately overloaded as GraphSync |
| 25 | [Do not replicate lists - DNR](./25-do-not-replicate-lists-dnr.md) | **[@olizilla](https://github.com/olizilla)** | How to stop your node from replicating content due to take down notices or other reasons |
| 26 | [Fast IPNS 📦](./26-fast-ipns.md) | **[@hugomrdias](https://github.com/hugomrdias)** | How to increase the IPNS resolution speed |
| 27 | [MultiWriter IPNS 📦](./27-multiwriter-ipns.md) |  | Allowing multiple peers to update an IPNS record |
| 28 | [WASM in JS IPFS](./28-wasm-in-js-ipfs.md) |  | Should more WASM be used in JS IPFS, what for and where? |
| 29 | [Resource utilization](./29-resource-utilization.md) |  | What are the different places an IPFS node will operate and what are the appropriate resource utilization profiles for them? |
| 30 | [IPFS Education and Documentation](./30-ipfs-education-and-documentation.md) | **[@meiqimichelle](https://github.com/meiqimichelle)** | What are the biggest improvements we can make to documentation for IPFS? |
| 31 | [Mounting an IPFS filesystem 📦](./31-mounting-an-ipfs-filesystem.md) | **[@djdv](https://github.com/djdv)** | Is there a way to efficiently mount IPFS as a filesystem? FUSE support is [here](https://github.com/ipfs/go-ipfs/blob/v0.4.21-rc3/docs/fuse.md). What are current limitations, challenges? What needs to happen to enable mounting of MFS? WebDAV is often used in network storage drives, and mainstream operating systems come with native support for mounting WebDAV as drives. It could supersede Writable Gateway and create a surface for interop with apps that provide built-in client-side support for WebDAV. https://github.com/ipfs/in-web-browsers/issues/146 |
| 32 | [Faster content discovery](./32-faster-content-discovery.md) |  | How can we make content discovery faster using ideas like peer hints or web seeds https://github.com/ipld/ipld/issues/57 |
| 33 | [Re-configuring IPFS on the fly](./33-re-configuring-ipfs-on-the-fly.md) |  | What would need to happen for an IPFS node to be able to be re-configured without a restart? |
| 34 | [IPNS link rot](./34-ipns-link-rot.md) | **[@alanshaw](https://github.com/alanshaw)** | Right now, IPNS needs to be refreshed by original publisher every day, otherwise it stops working. There should be a way to pin IPNS address so that other peers keep refreshing the last valid entry when original node goes offline, keeping the last version alive even if the original publisher disappears forever. |
| 35 | [Deterministic CIDs! Reproducible File Imports! Verifable HTTP Gateways!](./35-deterministic-cids-reproducible-file-imports-verifable-http-gateways.md) | **[@lidel](https://github.com/lidel)** | How to deterministically get the same CID for the same data, even if ipfs.add defaults change? How can we validate data read via HTTP Gateway without running full IPFS node? https://github.com/ipfs/roadmap/issues/19#issuecomment-494529255 https://github.com/ipfs/in-web-browsers/issues/128 |
| 36 | [Key Management](./36-key-management.md) |  | How it works today? Where we need to be? Eg: `ipfs key` is missing primitives for signing and verifying things using keys, we dont have interop for key import/export, keys are stored unencrypted on disk etc. I see this as "where we are"+"what devs need" → "where we need to be for 1.0"  type of dive, producing some tangible AIs |
| 37 | [IPFS in Web Workers](./37-ipfs-in-web-workers.md) | **[@gozala](https://github.com/gozala)** | Where we are, limitations, known problems. https://github.com/ipfs/in-web-browsers/issues/55 |
| 38 | [UnixFS v2 📦](./38-unixfs-v2.md) | **[@mikeal](https://github.com/mikeal)** | https://github.com/ipfs/unixfs-v2/blob/master/SPEC.md, https://github.com/ipfs/roadmap/issues/19 |
| 39 | [Using CRDTs to build real-time collaborative DApps](./39-using-crdts-to-build-real-time-collaborative-dapps.md) | **[@jimpick](https://github.com/jimpick)** | What are the hurdles to using CRDTs in dapps with IPFS? How can we make peer-base easier to understand and use? |
| 40 | [Better NAT traversal so that Relay servers are a last (not first) resort](./40-better-nat-traversal-so-that-relay-servers-are-a-last-not-first-resort.md) | **[@raulk](https://github.com/raulk)** | The current cost of running relay servers for IPFS is unsustainable.  We need to implement better NAT hole punching mechanisms in libp2p to reduce the usage of relay servers by NAT’d hosts.  TCP hole punching has a success rate of ~60%, so we should be preferentially hole punching.  TCP simultaneous open is one example.  STUN servers are another example; yet another is making every non-NATed host in a libp2p network a relay node. |
| 41 | [libp2p connection bootstrapping and protocol negotiation 2.0](./41-libp2p-connection-bootstrapping-and-protocol-negotiation-2.0.md) |  | Our connection bootstrapping process is chatty and inefficient. We incur in several round trips upfront just to negotiate the basics (encryption, muxing). Stream-level protocol negotiation is also inefficient. We are working on Multiselect 2.0 and a revamped connection bootstrapping process. This is the very heart of libp2p. Help us get this right. |
| 42 | [libp2p message orientation](./42-libp2p-message-orientation.md) | **[@bigs](https://github.com/bigs)** | libp2p is currently stream-oriented. We want to enable message-oriented communication (e.g. UDP). Help us envision what the APIs would look like, and how an application could simultaneously hold stream-based and message-based conversations with peers in the world via libp2p. |
| 43 | [IPFS metrics and usage statistics 📦](./43-ipfs-metrics-and-usage-statistics.md) | **[@lanzafame](https://github.com/lanzafame)** | How to collect telemetry like application metrics and usage in a distributed world |
| 44 | [Decentralized Data Processing](./44-decentralized-data-processing.md) |  | |
| 45 | [Building Dynamic P2P Applications](./45-building-dynamic-p2p-applications.md) | **[@jkarni](https://github.com/jkarni)** | |
| 46 | [Better file chunking](./46-better-file-chunking.md) | **[@mib-kd743naq](https://github.com/mib-kd743naq)** | |

**Note**: topics relevant to package managers have a 📦 suffix.

### Topic description template

Use this template to create your one-pager description about your topic. Send a PR to https://github.com/ipfs/camp/tree/master/DEEP_DIVES with your topic description page e.g. `FAST_IPNS.md`

```markdown
# <Deep Dive Topic NAME>

<Short summary of topic including Open Problem(s) to solve>

## Goal

<Define what we would get if the Open Problem(s) are solved for this Deep Dive>

## Requirements to consider

<Do we have requirements (i.e. work with 1MM nodes)?>

## Where to learn about it

<List of talks, links to github issues, code, notes and so on>
```
