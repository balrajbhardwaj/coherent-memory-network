# Coherent Memory Network

**A framework for giving AI agents governed context in regulated organisations.**

AI does not lack data. It lacks context: where data should come from, whether it is fit for the task, whether the rules are met at the moment of use, and whether the consumer is entitled to it. This repository holds a white paper that sets out the framework, and an interactive demo that runs its rules live.

- **Read the white paper:** https://balrajbhardwaj.github.io/coherent-memory-network/
- **Try the demo:** https://balrajbhardwaj.github.io/coherent-memory-network/demo.html

---

## The problem

Business teams can now build working tools with AI in hours. When a person or an AI agent cannot easily find the approved source for a piece of data, they use the nearest one, and an ungoverned data path is created. Repeat that across many teams and agents and the result is fragmentation at scale.

Most organisations hold the context that would prevent this in documents, spreadsheets and people's heads. AI agents can read none of them. Data quality controls are usually checked in batch, after the data has already been used.

## The framework

The Coherent Memory Network turns that context into something machines can query at the moment they use data. It has five components, each answering one question:

| Component | Question it answers |
|---|---|
| **Authorised Source Registry** | Where should this data come from, and who owns it? |
| **Fitness for Purpose Framework** | Is this source suitable for this specific task? |
| **Runtime Controls** | Does the data meet the rules right now, at the point of use? |
| **Governed Access** | Is this consumer entitled to this data, for this purpose? |
| **Organisational Reality Map** | How does the business actually work, and who acts when something breaks? |

Each component runs as a shared service. An agent does not assemble the checks itself: it declares its identity and purpose, and the network runs every check in order, logs the decision and notifies the data owner when something fails. The white paper also covers the operating model (five roles) and a four stage maturity journey.

## The demo

The demo is a small rules engine that runs in the browser. Nothing is scripted. Every result is worked out from the registry, fitness profiles, controls and entitlements, so when you change them, the answer changes.

**How to use it**

1. **Pick a situation**, such as a stale counterparty feed, a wrong source requested, an unapproved use or a shared service account.
2. **Read the request** as a sentence. Change the agent, or the source it asks for.
3. **See the decision** as a chain of five steps, from Request to Governed access, with the outcome beside it.
4. **Open any step** to see why it passed or failed, and change what drives it:
   - **Registry:** approve or withdraw sources for each purpose, and choose whether a wrong source is rejected and escalated or rerouted.
   - **Fitness:** edit the profile thresholds. The YAML updates as you type.
   - **Runtime controls:** move sliders for data age and completeness, or switch on an outage or broken lineage.
   - **Governed access:** revoke or restore an entitlement.

All systems, agents and data in the demo are fictional.


Then go to http://localhost:8000.

## Original article series

The white paper is edited from a five part series first published on LinkedIn:

1. [Your AI Is Only as Good as Its Memory. Are You Building the Right One?](https://www.linkedin.com/pulse/your-ai-only-good-its-memory-you-building-right-one-balraj-bhardwaj-s0jfe/) (April 2026)
2. [AI Needs Context: Start with a Source Registry](https://www.linkedin.com/pulse/ai-needs-context-start-source-registry-balraj-bhardwaj-opije/) (May 2026)
3. [Why Good Data Isn't Good Enough, and What That Means for AI](https://www.linkedin.com/pulse/why-good-data-isnt-enough-what-means-ai-balraj-bhardwaj-gthae/) (October 2026)
4. [Every Agent is a Control Point](https://www.linkedin.com/pulse/every-agent-control-point-balraj-bhardwaj-plbze/) (October 2026)
5. [Trusted AI: The Coherent Memory Operating Model](https://www.linkedin.com/pulse/trusted-ai-coherent-memory-operating-model-balraj-bhardwaj-fxw8e/) (October 2026)



## Author

**Balraj Bhardwaj**, data architect, data modeller and data governance specialist working in financial services.
[LinkedIn](https://www.linkedin.com/in/bal8/)

## Copyright

© 2026 Balraj Bhardwaj. All rights reserved.

You are welcome to read, link to and discuss this work. Please do not copy or republish the white paper or the demo without permission.

This is personal work. Systems, data and examples are illustrative and do not describe any specific organisation. Views are the author's own.
