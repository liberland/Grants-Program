# Liberland Blockchain - the Judiciary

- **Team Name:** Liberland Blockchain Team
- **Payment Address:** fiat or, possibly, BTC
- **[Level](https://github.com/w3f/Grants-Program/tree/master#level_slider-levels):** 3

## Project Overview :page_facing_up:

Follow-up on Liberland Grant Application [pull requesT: Create liberland #831; a623bb28f2c9ce9609bf46e0e5801cda6e55aa47] 

### Liberland Blockchain

Our mission is to conceive a blockchain-compatible solution that translates traditional dispute resolution and judiciary functionalities into the digital realm. Our vision includes a system that synergizes the virtues of centralized and decentralized models.

Liberland Blockchain is a layer 1 public blockchain owned by coin and token holders. The blockchain is funded and supported by Liberland, providing the first set of use cases. The codebase is a fork of Substrate/Polkadot, and the license is MIT, the same as Bitcoin. Liberland does not claim ownership of the blockchain or related materials.

The blockchain allows permissionless usage of tokens and coins as a store of value or medium of exchange. Advanced functionalities critical to the project's future are permissioned. DeFi projects on the Liberland chain are not permissioned unless designed by third-party developers on a per-project basis.

This milestone now sets the stage for implementing the quintessential element of all governance systems - the judiciary. We seek to enable dispute resolution and advisory opinions, traditionally offline activities, to take place within this blockchain ecosystem.

### Overview

The Liberland Judiciary is designed to develop an on-chain system capable of acting on behalf of a party without their explicit permission in pre-approved ways with mutual consent given in advance.

- Facilitate the integration of a 'court as a smart contract oracle', thereby enabling the execution of traditional, verbose contracts on-chain. This system allows for the imposition of sanctions as dictated by the applicable law and the contract itself in the event of a dispute.
- Implement a body of norms or laws to regulate the system's operations, thereby eliminating arbitrary decisions and enhancing trust.
- Guarantee decentralization and security while ensuring that the system is operated by professionals who uphold the quality of decisions.
- Retain recognizability by resembling a traditional courtroom rather than a streamlined IT service app.

The solution we propose introduces a hybrid entity, central yet decentralized, capable of interpreting intent behind actions within the blockchain. Empowered to regulate transactions by reversing or counteracting them, this entity exercises authority particularly in situations where malicious or bad faith intentions are identified. By introducing a virtual judiciary, any questionable actions can be evaluated and, if necessary, nullified.

This architecture enhances the breadth of on-chain business activity, facilitating enforcement of traditional contract agreements and enabling partial algorithmic execution. In effect, this approach instills confidence that transactions, whether off-chain or on-chain, offline or online, will be enforced. Additionally, it offers an authoritative entity to resolve any disputes arising from the obligations agreed upon by the parties involved.

The Liberland Blockchain solution will be a significant addition to the Polkadot ecosystem. By translating traditional dispute resolution and judiciary functionalities into the digital realm, it will introduce a new layer of trust and security to blockchain transactions. The integration of a 'court as a smart contract oracle' will enable the execution of traditional contracts on-chain, thereby expanding the scope of on-chain business activity. 

Furthermore, the solution will provide a hybrid entity that is both central and decentralized, capable of interpreting intent behind actions within the blockchain. This will enhance the Polkadot ecosystem's ability to regulate transactions, especially in situations where malicious or bad faith intentions are identified. 

The Liberland Blockchain, a layer 1 public blockchain, is a fork of Substrate/Polkadot, further strengthening the ties between the two ecosystems. By offering a virtual judiciary, the solution will instill confidence in transactions and provide an authoritative entity to resolve any arising disputes. This will significantly contribute to the robustness and reliability of the Polkadot ecosystem.

### Project Details

#### Simple Process
##### Outline
The Simple process is employed when all parties involved reach a consensus on the selection of a judge or panel of judges to preside over their case. The selection can be explicit (naming a specific judge) or implicit ("we agree to let the system decide"). The system provides parameters (such as cost, experience level, etc.) for judge selection, with the stipulation that parties are bound by their agreement to accept the system's random selection within the agreed upon parameters.

The Simple process is designed to be:
- Quick, and
- More economical than the contested process.
- The intent is to ensure expedient and cost-effective resolution, contrasting with contemporary systems where years can elapse before disputes are resolved. In Liberland, minor disputes could potentially be adjudicated within a day or a few days through the Simple process, and at a significantly reduced cost.

##### Mediation
The appointed judge endeavors to segment the case into manageable portions, drafting a mediation solution for each. This proposed solution is then presented to the involved parties. If an agreement is reached, the process concludes without litigation, and the judge is remunerated a flat fee, which is lower than the litigation tariff.

##### Litigation
In instances where a mutual agreement is not achieved, the judge drafts a mediation solution and presents it to the involved parties. If an agreement is reached, -> the litigation process is averted, -> with the judge remunerated a flat fee that is lower than the tariff payable when Complex Process is used.

#### Complex Process
##### Outline
The Complex Process acts as a fallback mechanism when the parties cannot concur on the choice of a judge or other terms. A mutual agreement on jurisdiction must be established for any process to occur, but there may exist a level of distrust that prevents a jointly accepted judge. In such circumstances, the system adapts to assign three judges:
- The attorney representing the applicant,
- The attorney representing the respondent, and
- An arbitrator, jointly selected by the two attorneys.

This system, although more involved, remains streamlined for efficiency and cost-effectiveness, maintaining the balance between swiftness and the demands of judicature. The Complex Process is designed to handle intricate issues requiring detailed attention and processual protections for the parties involved. Ultimately, the criminal process of Liberland will adopt the framework of the Complex Process.

##### Mediation
1. A user (Party A) alleges that another user (Party B) has violated the standing body of rules (Liberland Law). In case of smart contract, this is done by triggering a function on the contract itself, which enters into 'litigation mode' until the process is resolved
2. Party A selects a judge (Attorney A) from the available roster, agrees to their terms, and pays collateral plus a transaction fee.
3. Party B is notified and selects a judge (Attorney B).
4. Party A and Attorney A compile and submit a Case.
5. Party B and Attorney B compile and submit a Response.
6. The Attorneys meet to create a Compromise, dividing the Case into parts and seeking resolution without litigation where possible.
7. Resolved parts of the Case are executed.
8. The unresolved parts proceed to Litigation.

##### Litigation
1. Attorneys mutually select a third Judge (the Arbitrator).
2. The Arbitrator delivers a Judgement, analyzing the Application and Response according to Liberland law and relevant contract, resulting in statements of "Party X pays to Party Y," backed by a rationale.
3. If the Parties accept, the judgment is executed. If a Party rejects, the Party pays the appeals fee, and an appeal process commences.

#### Appeal
##### Outline
An appeal can ensue after either the Simple Process or the Complex Process. It is initiated upon the request of a party, presenting costs to the petitioner and imposing time constraints, namely the period until adjudication, upon the other party. Additionally, the assurance of the first instance's final verdict is jeopardized. Parties may agree in advance to forgo the appeal process, rendering the first instance judgment as the final verdict, anticipated to be prevalent primarily with the Simple Process.

##### Steps of an Appeal
1. An Appeal Judge is appointed by the algorithm.
2. The Appeal Judge examines the appeal points and formulates an Appeal Verdict.
3. The final Verdict is executed on the Collateral and the Pooled LLM.

#### Functionality: Advisory Opinion
If a party wishes to obtain the Court's opinion on a particular legal, technical or factual matter, even in the absence of a dispute, the system will offer two types of Advisory Opinions:

**Simple Advisory Opinion:** This is a yes/no binary question. The party formulates the question, provides reasoning, pays a fee, and presents the question to the Judge. They then wait for the Judge's decision and can either accept or reject it. If they reject it, they can pay an additional fee to re-run the game up to three times to view the opinions of three different Juries.
**Complex Advisory Opinion:** The party pays a higher fee, formulates a complex question, and chooses a Judge. The Judge then formulates the Opinion on the points of the question. The party waits for the Judge's decision and, similar to a Simple Advisory Opinion, they can accept or reject it, paying an additional fee to re-run the game up to three times if they choose to reject it.

#### Enactment of Awards
##### The Optimal Circumstance
A contract or a case is collateralized such that the collateral is sufficient to cover any additional payments prescribed in the final verdict, beyond the awarded sum and the Court Costs. In this scenario, the collateral serves as a mechanism for execution of the judgement. Collateral may be handled by a third party, such as an insurance company.

##### Case with Insufficient Collateral
###### Seizing LLM
The judge is imbued with the authority to designate an individual's LLM as collateral. Upon such a declaration, an involuntary unpooling of the owing party's LLM stash will ensue, carrying typical ramifications like the forfeit of voting rights associated with that stash. If the full amount is subsequently paid, this directive is withdrawn. However, under circumstances where

there is a violation of the Non Aggression Principle, implicating aggressive conduct against another individual's person or property, or

the damage incurred exceeds one's LLM stash,

the offender's LLM balance could turn negative, resulting in their listing on Liberland's 'wanted' roster, rendering them a 'persona non grata'. Consequently, they lose their voting rights until the owed amount is fully settled.

###### Enforcement Beyond the Chain
In instances where the judgement cannot be enforced by either of the aforementioned methods, the awarded sum will be incorporated into a conventional contract, or appended as a supplement if the dispute is contract-related. This contract, endorsed by both parties, holds legitimacy outside of Liberland, akin to any other contract. It can be presented to an enforcement agency for execution, even against the unwilling party's resistance. Note that this is just an explanation of the process, and doesn't represent a deliverable for the grant.

#### Functionality: Traditional Contracts
##### Overview
Most contractual relationships in the world aren't currently simple and predictable enough to be run on smart contracts. This is likely to remain so even in the age of AI, at least for a decade or so. In the meantime, dumb contracts, that is, traditional contracts, are what runs the world of business and your everyday life. What is a dumb contract? It is an agreement you make with another human being. It is also a smart contract, in a way, but it runs on the hardware and the OS of your brain.

How will it work? Alice and Bob enter into a traditional contract for the sale of goods. They agree to use the Liberland Blockchain Judiciary system for any potential disputes. They choose a judge from the roster and agree on the collateral and fees. The contract is then recorded on the blockchain. Why should someone want to do this?

##### Benefits:
- **Efficiency and Speed:** The Liberland Blockchain Judiciary system offers a Simple Process for dispute resolution. If a dispute arises, Alice or Bob can trigger the judge to give a binding opinion. This process is designed to be quick and more economical than traditional legal systems, potentially resolving disputes within a few days.
- **Cost-Effectiveness:** The system is designed to be more economical than traditional legal systems. The costs are defined upfront and include the judge's fees and any potential award to the victorious party. This transparency and predictability of costs can make the system more attractive to parties entering into a contract.
- **Security and Trust:** The system is built on the blockchain, providing a secure and immutable record of the contract and any subsequent dispute resolution proceedings. This can increase trust between the parties and reduce the risk of fraudulent claims.
- **Payment Processing:** The blockchain can also be used to process payments related to the contract. This can be particularly useful in cases where the contract involves regular payments or where the amount of payment is dependent on certain conditions being met. The blockchain can automatically process these payments when the conditions are met, reducing the need for manual intervention and the risk of non-payment.
- **Smartification of Traditional Contracts:** While the contract itself may be a traditional contract, the use of the blockchain allows for certain aspects of the contract to be automated. For example, payments can be automatically triggered when certain conditions are met. This can make the contract more efficient and reduce the potential for disputes.
- **Functionality:** Advisory Option in State Administration
Beyond dispute resolution and advisory opinions, we plan to extend the use of this system to other areas, such as Administrative Decisions on-chain.

For example, the process of granting or denying citizenship could be complemented with our decentralized system. The Ministry of Internal Affairs, Citizenship Agency would work with the Citizen applicant through steps such as proof of commitment (locked stake), KYC, and Citizenship Interview.

Afterward, they would create a brief report on the results and a more detailed report on the applicant's background. The Judge would then Confirm or Reject the applicant. A Confirmed applicant becomes a Citizen, while a Rejected one must wait one year before re-applying.

This is not an exhaustive list of potential applications for our system. We encourage other builders to explore further expansions.

#### Functionality: Decentralized Registers
Along with the previous system, we can also decentralize our property register operations. The relevant Ministry would create an entry and add background information, which is generally straightforward or automated.

The Judge then makes a final Confirmation or Rejection. These decisions will mostly be affirmations. Hence they are considered low-stakes/low gains games.

To make these games more engaging, we could utilize the Complex Advisory Opinion and establish a group of on-chain Registrars who operate the Registry instead of the Ministry. These Registrars could even propose different opinions on what to inscribe, making the games about these matters more interesting.
### Ecosystem Fit

Help us locate your project in the Polkadot/Substrate/Kusama landscape and what problems it tries to solve by answering each of these questions:

- Where and how does your project fit into the ecosystem?
- Who is your target audience (parachain/dapp/wallet/UI developers, designers, your own user base, some dapp's userbase, yourself)?
- What need(s) does your project meet?
- Are there any other projects similar to yours in the Substrate / Polkadot / Kusama ecosystem?
  - If so, how is your project different?
  - If not, are there similar projects in related ecosystems?

## Team :busts_in_silhouette:

### Team members

- Name of team leader
- Names of team members

### Contact

- **Contact Name:** Full name of the contact person in your team
- **Contact Email:** Contact email (e.g. john@duo.com)
- **Website:** Your website

### Legal Structure

- **Registered Address:** Address of your registered legal entity, if available. Please keep it in a single line. (e.g. High Street 1, London LK1 234, UK)
- **Registered Legal Entity:** Name of your registered legal entity, if available. (e.g. Duo Ltd.)

### Team's experience

Please describe the team's relevant experience. If your project involves development work, we would appreciate it if you singled out a few interesting projects or contributions made by team members in the past. 

If anyone on your team has applied for a grant at the Web3 Foundation previously, please list the name of the project and legal entity here.

### Team Code Repos

- https://github.com/<your_organisation>/<project_1>
- https://github.com/<your_organisation>/<project_2>

Please also provide the GitHub accounts of all team members. If they contain no activity, references to projects hosted elsewhere or live are also fine.

- https://github.com/<team_member_1>
- https://github.com/<team_member_2>

### Team LinkedIn Profiles (if available)

- https://www.linkedin.com/<person_1>
- https://www.linkedin.com/<person_2>


## Development Status :open_book:

If you've already started implementing your project or it is part of a larger repository, please provide a link and a description of the code here. In any case, please provide some documentation on the research and other work you have conducted before applying. This could be:

- links to improvement proposals or [RFPs](https://github.com/w3f/Grants-Program/tree/master/docs/RFPs) (requests for proposal),
- academic publications relevant to the problem,
- links to your research diary, blog posts, articles, forum discussions or open GitHub issues,
- references to conversations you might have had related to this project with anyone from the Web3 Foundation,
- previous interface iterations, such as mock-ups and wireframes.

## Development Roadmap :nut_and_bolt:

This section should break the development roadmap down into milestones and deliverables. To assist you in defining it, we have created a document with examples for some grant categories [here](../docs/Support%20Docs/grant_guidelines_per_category.md). Since these will be part of the agreement, it helps to describe _the functionality we should expect in as much detail as possible_, plus how we can verify and test that functionality. Whenever milestones are delivered, we refer to this document to ensure that everything has been delivered as expected.

Below we provide an **example roadmap**. In the descriptions, it should be clear how your project is related to Substrate, Kusama or Polkadot. We _recommend_ that teams structure their roadmap as 1 milestone ≈ 1 month.

> :exclamation: If any of your deliverables is based on somebody else's work, make sure you work and publish _under the terms of the license_ of the respective project and that you **highlight this fact in your milestone documentation** and in the source code if applicable! **Teams that submit others' work without attributing it will be immediately terminated.**

### Overview

- **Total Estimated Duration:** Duration of the whole project (e.g. 2 months)
- **Full-Time Equivalent (FTE):**  Average number of full-time employees working on the project throughout its duration (see [Wikipedia](https://en.wikipedia.org/wiki/Full-time_equivalent), e.g. 2 FTE)
- **Total Costs:** Requested amount in USD for the whole project (e.g. 12,000 USD). Note that the acceptance criteria and additional benefits vary depending on the [level](../README.md#level_slider-levels) of funding requested. This and the costs for each milestone need to be provided in USD; if the grant is paid out in Bitcoin, the amount will be calculated according to the exchange rate at the time of payment.

### Milestone 1 Example — Basic functionality

- **Estimated duration:** 1 month
- **FTE:**  1,5
- **Costs:** 8,000 USD

> :exclamation: **The default deliverables 0a-0d below are mandatory for all milestones**, and deliverable 0e at least for the last one. 

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **0a.** | License | Apache 2.0 / GPLv3 / MIT / Unlicense |
| **0b.** | Documentation | We will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can (for example) spin up one of our Substrate nodes and send test transactions, which will show how the new functionality works. |
| **0c.** | Testing and Testing Guide | Core functions will be fully covered by comprehensive unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| **0d.** | Docker | We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone. |
| 0e. | Article | We will publish an **article**/workshop that explains [...] (what was done/achieved as part of the grant). (Content, language and medium should reflect your target audience described above.) |
| 1. | Substrate module: X | We will create a Substrate module that will... (Please list the functionality that will be implemented for the first milestone. You can refer to details provided in previous sections.) |
| 2. | Substrate module: Y | The Y Substrate module will... |
| 3. | Substrate module: Z | The Z Substrate module will... |
| 4. | Substrate chain | Modules X, Y & Z of our custom chain will interact in such a way... (Please describe the deliverable here as detailed as possible) |
| 5. | Library: ABC | We will deliver a JS library that will implement the functionality described under "ABC Library" |
| 6. | Smart contracts: ... | We will deliver a set of ink! smart contracts that will...


### Milestone 2 Example — Additional features

- **Estimated Duration:** 1 month
- **FTE:**  1,5
- **Costs:** 8,000 USD

...


## Future Plans

Please include here

- how you intend to use, enhance, promote and support your project in the short term, and
- the team's long-term plans and intentions in relation to it.

## Referral Program (optional) :moneybag: 

You can find more information about the program [here](../README.md#moneybag-referral-program).
- **Referrer:** Name of the Polkadot Ambassador or GitHub account of the Web3 Foundation grantee
- **Payment Address:** BTC, Ethereum (USDC/DAI) or Polkadot/Kusama (USDT) payment address. Please also specify the currency. (e.g. 0x8920... (DAI))

## Additional Information :heavy_plus_sign:

**How did you hear about the Grants Program?** Web3 Foundation Website / Medium / Twitter / Element / Announcement by another team / personal recommendation / etc.

Here you can also add any additional information that you think is relevant to this application but isn't part of it already, such as:

- Work you have already done.
- If there are any other teams who have already contributed (financially) to the project.
- Previous grants you may have applied for.
