# Liberland Blockchain - the Judiciary

- **Team Name:** Liberland Blockchain Team
- **Payment Address:** fiat or, possibly, BTC
- **[Level](https://github.com/w3f/Grants-Program/tree/master#level_slider-levels):** 2

## Project Overview :page_facing_up:

Follow-up on Liberland Grant Application [pull request: Create liberland #831; a623bb28f2c9ce9609bf46e0e5801cda6e55aa47] 

### Liberland Blockchain

We are Liberland, the world's freest country. Currently, we are settling the physical land and developing our blockchain. 

Liberland Blockchain is a sovereign blockchain owned by token holders, founded and supported by Liberland which provides the first set of use cases. The codebase is a fork of Substrate/Polkadot, with MIT license. Liberland does not claim ownership of the blockchain or related materials.

Functionalities such as trading and DeFi projects are permissionless by default while some critical functionalities such as country politics are permissioned and require KYC.

The next blockchain milestone is translating traditional contract, dispute resolution and judiciary functionalities into the Web3 realm, synergizing the virtues of centralized and decentralized models.

This milestone implements the quintessential element of all governance systems - the judiciary. We seek to enable dispute resolution and advisory opinions to take place within this blockchain ecosystem.

### Overview

#### Project Overview

The Liberland Judiciary is designed to develop an on-chain system capable of acting on behalf of a party without their explicit permission in pre-approved ways with mutual consent given in advance.

- Facilitate the integration of a 'court as a smart contract oracle', thereby enabling the execution of traditional, verbose contracts on-chain. This system allows for the imposition of sanctions as dictated by the applicable law and the contract itself in the event of a dispute.
<RETHINK>
- Implement norms or laws to regulate the system's operations, thereby eliminating arbitrary decisions and enhancing trust.
- Guarantee decentralization and security while ensuring that the system is operated by professionals who uphold the quality of decisions.
- Retain recognizability by resembling a traditional courtroom rather than a streamlined IT service app.

The solution we propose introduces a hybrid entity, central yet decentralized, capable of interpreting intent behind actions within the blockchain. Empowered to regulate transactions by reversing or counteracting them, this entity exercises authority particularly in situations where malicious or bad faith intentions are identified. By introducing a virtual judiciary, any questionable actions can be evaluated and, if necessary, nullified.

This architecture enhances the breadth of on-chain business activity, facilitating enforcement of traditional contract agreements and enabling partial algorithmic execution. In effect, this approach instills confidence that transactions, whether off-chain or on-chain, offline or online, will be enforced. Additionally, it offers an authoritative entity to resolve any disputes arising from the obligations agreed upon by the parties involved.
</RETHINK>
#### Project Ecosystem Fit
The integration of a 'court as a smart contract oracle' will enable the execution of traditional, worded contracts on-chain, thereby expanding the scope of on-chain business activity.
By translating traditional dispute resolution and judiciary functionalities into Web3, it will introduce a new layer of trust and security to blockchain transactions.
The Liberland Blockchain will be a significant addition to the Polkadot ecosystem as our pallets and practices can be used directly or in other parachains.

### Project Details

#### Simple Process
##### Outline
The Simple process is employed when all involved parties reach a consensus on selecting judges to preside over their case. The selection can be explicit (naming a specific judge) or implicit ("letting the system decide"). within given parameters (such as cost, experience level, etc.) for judge selection.

The Simple process is designed to be quick and cost-effective.

##### Mediation
The appointed judge segments the case into portions, drafting a mediation solution for each. This proposed solution is presented to the involved parties.
If an agreement is reached, the process concludes without litigation, and the judge is paid.

##### Litigation
<UNCLEAR same as mediation ?>
When mutual agreement is not achieved, the judge drafts a mediation solution and presents it to the involved parties.
If an agreement is reached, -> the litigation process is averted, -> with the judge remunerated a flat fee that is lower than the tariff payable when Complex Process is used.
</UNCLEAR>
#### Complex Process
##### Outline
The Complex Process is used when the parties cannot agree on the choice of a judge or other terms. An agreement on jurisdiction must be pre-established for any process to occur. In such circumstances, the system adapts to assign three judges:
- The attorney representing the applicant,
- The attorney representing the respondent, and
- An arbitrator jointly selected by the two attorneys.

The Complex Process is designed to handle intricate issues requiring detailed attention and processual protections for the parties involved while maintaining balance between swiftness and the demands of judicature. 
Ultimately, the criminal process of Liberland will adopt the framework of the Complex Process.

##### Mediation
1. Party A alleges that Party B has violated the rules (Contract or law). In a smart contract, this is done by triggering a function on the contract which activates 'litigation mode' until the process is resolved
2. Party A selects Attorney A from the available roster, agrees to their terms, and pays collateral plus a transaction fee.
3. Party B is notified and selects Attorney B.
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
An appeal can ensue after the litigation process, unless the parties agreed in advance to forego the possibility of appeal, which is anticipated to be common in the Simple process. 
Appeal is initiated on request, which questions the litigation verdict.
Appeal must be paid for by the party initiating it.

##### Steps of an Appeal
1. An Appeal Judge is appointed by the algorithm.
2. The Appeal Judge examines the appeal points and formulates an Appeal Verdict.
3. The final Verdict is executed on the Collateral.

#### Functionality: Advisory Opinion
If a party wishes to obtain the Court's opinion on a particular matter in the absence of a dispute, the system offers two types of Advisory Opinions:

**Simple Advisory Opinion:** A yes/no binary question. The party formulates the question, provides reasoning, pays a fee, and presents the question to the Judge. They then wait for the Judge's decision and can either accept or reject it. If they reject it, they can pay an additional fee to re-run the game up to three times to view the opinions of three different Juries.
**Complex Advisory Opinion:** The party pays a higher fee, formulates a complex question, and chooses a Judge. The Judge then formulates the Opinion on the points of the question. The party waits for the Judge's decision and either accepts or rejects it, paying an additional fee to re-run the game up to three times if they choose to reject it.

#### Enactment of Awards
##### The Optimal Circumstance
A contract or a case has suffiient collateral to cover any additional payments in the final verdict and the court costs. In this scenario, the collateral is used for the execution of the judgement. A third party, like an insurance company may handle collateral.

##### Case with Insufficient Collateral
###### Seizing politipooled LLM
The judge has the authority to designate an individual's politipooled (staked) LLM as collateral, triggering involuntary unpooling of the owing party's pooled LLM.

However, under circumstances where

- there is a violation of the Non-Aggression Principle, implicating aggressive conduct against persons or property, or
- the damage incurred exceeds one's LLM stash,

the offender's LLM balance could turn negative, resulting in their listing on Liberland's 'wanted' roster, rendering them a 'persona non grata'. Consequently, they lose their voting rights and potentially access to other Liberland services until the owed amount is fully settled.

###### Enforcement Beyond the Chain
In instances where aforementioned methods cannot enforce the judgement, the awarded sum will be incorporated into a conventional contract or appended as a supplement if the dispute is contract-related.
This contract, endorsed by both parties, holds legitimacy outside of Liberland, akin to any other contract. It can be presented to an enforcement agency for execution, even against the unwilling party's resistance.
Note that this is just an explanation of the process and doesn't represent a deliverable for the grant.

#### Functionality: Traditional Contracts
##### Overview
Most contractual relationships in the world aren't simple and predictable enough to be run on smart contracts.
Dumb/traditional contracts, are what runs the world of business and everyday life made in an agreement with another humans under juridistictions of nation states. 

We aim to translate these traditional contracts into Web3.

How will it work? Alice and Bob enter into a traditional contract for the sale of goods. They agree to use the Liberland Blockchain Judiciary system for any potential disputes. 
They choose a judge from the roster and agree on the collateral and fees. The contract is recorded on the blockchain.

##### Benefits:
- **Efficiency and Speed:** The Liberland Blockchain Judiciary system offers a Simple Process for dispute resolution. If a dispute arises, Alice or Bob can trigger the judge to give a binding opinion. This process is quicker and cheaper than traditional legal systems, potentially resolving disputes within a few days.
- **Cost-Effectiveness:** The system is designed to be cheaper than traditional legal systems. The costs are defined upfront and include the judge's fees and any potential award to the victorious party, offering transparency and predictability of costs.
- **Security and Trust:** Blockchain provides a secure and immutable record of the contract and dispute resolution proceedings. This increases trust and reduces the risk of fraudulent claims.
- **Payment Processing:** The blockchain can be used to process payments related to the contract. This is useful in cases where the contract involves regular payments or where the amount depends on certain conditions being met. The blockchain can automatically process these payments when the conditions are met, removing manual intervention and the risk of non-payment.
- **Smartification of Traditional Contracts:** While the contract itself may be a traditional contract, the use of the blockchain allows for parts of the contract to be automated. For example, payments can be automatically triggered when certain conditions are met. This makes the contract more efficient and reduces the potential for disputes.
- **Functionality:** Advisory Option in State Administration
Beyond dispute resolution and advisory opinions, we plan to extend the use of this system to other areas, such as Administrative Decisions on-chain.

For example, the process of granting or denying citizenship could be complemented with our decentralized system. The Ministry of Internal Affairs, Citizenship Agency would work with the Citizen applicant through steps such as proof of commitment (locked stake), KYC, and Citizenship Interview.

Afterward, they would create a brief report on the results and a more detailed report on the applicant's background. The Judge would then Confirm or Reject the applicant. A Confirmed applicant becomes a Citizen, while a Rejected one must wait one year before re-applying.

This is not an exhaustive list of potential applications for our system. We encourage other builders to explore further expansions.

#### Functionality: Decentralized Registers
This system enables decentralization of property registers. 

The relevant Ministry would create an entry, whichcan be confirmed or rejected by a judge. These decisions will mostly be affirmations and are considered low-stakes/low gains games.

Alternatively, a group of private on-chain registrars can provide concensus or different opinions on inscriptions of registered entities.

### Ecosystem Fit

- **Where and how does your project fit into the ecosystem?**

The project aims to translate traditional dispute resolution and judiciary functionalities into Web3, introducing a new layer of trust and security to blockchain transactions.
The integration of a 'court as a smart contract oracle' will enable the execution of traditional contracts on-chain, expanding the scope of on-chain business activity.
The Liberland Blockchain project fits into the Polkadot/Substrate/Kusama ecosystem as a layer 1 public blockchain that is a fork of Substrate/Polkadot, that can be used directly or in parachains.

Although we deploy the system on our blockchain, it is fully open source and, available for anyone to use and adapt. 
Or just bridge to us and use it as part of Liberland's system. 
Additionally, the judiciary and registries pallets could be deployed as Liberland recognized, but separate private courts to provide traditional contract execution as a parachain on Polkadot and Kusama.

- **Who is your target audience (parachain/dapp/wallet/UI developers, designers, your own user base, some dapp's userbase, yourself)?**

The target audience for the Liberland Blockchain project includes developers, designers, and users of the Liberland Blockchain, as well as developers and users of other parachains, dapps, wallets, and UIs within the Polkadot/Substrate/Kusama ecosystem. The project also targets individuals and organizations interested in utilizing blockchain technology for dispute resolution, judiciary, traditional contract and company/asset management functionalities.

- **What need(s) does your project meet?**

The Liberland Blockchain project meets the need for a blockchain-compatible solution that translates traditional dispute resolution and judiciary functionalities into Web3. It provides a system that synergizes the virtues of centralized and decentralized models, allowing for the execution of traditional contracts on-chain and facilitating enforcement of traditional contract agreements. It also introduces a entity capable of interpreting intent behind actions within the blockchain and regulating transactions, especially in situations where malicious or bad faith intentions are identified.

In addition, it is the judiciary of the country of Liberland, fulfiling one part of the liberlander ambition to attain statehood, namely, to be able to appoint judges and to resolve cases of those who wish to live under Liberland' jurisdiction.

- **Are there any other projects similar to yours in the Substrate / Polkadot / Kusama ecosystem?**
  - **If so, how is your project different?**
  - **If not, are there similar projects in related ecosystems?**

Upon a comprehensive review of the solutions currently available within the Polkadot Ecosystem, we have found that none of these proposals or existing systems align directly with the unique functionality and objectives of our proposed solution. The two proposals that bear the closest resemblance to our initiative are the SaaS3 Court and the DOT Marketplace. However, upon closer examination, these systems diverge significantly from our approach in several key areas.

 **[SaaS3 Court](https://github.com/SaaS3-Foundation/saas3-dao/tree/main/pallets/court)**: This proposal outlines a jury-based judiciary system specifically designed for the blockchain. However, it lacks the comprehensive legal framework that our solution offers, as it does not aim to establish a full-fledged jurisdiction or nation-state. Its primary focus is to implement a judiciary system on the blockchain, where jurors are compensated in tokens based on the outcomes of certain cases. This system, while innovative, does not encompass the breadth of legal considerations that our solution addresses.

**[DOT Marketplace](https://github.com/WowLabz/dot-marketplace-v2/blob/Phase3_Milestone3/pallets/pallet-tasking/src/lib.rs)**: This proposal presents a general marketplace that could potentially offer judicial and legal services, contingent on market demand. However, its scope is both broader and more specific than our solution. While it is not a specialized judicial solution, it is also too narrowly focused on marketplace and task functions to present a significant competitive threat. Notably, it does not explicitly propose a meta-system to handle disputes arising within the marketplace.

In light of these observations, we believe that our solution does not compete with either the SaaS3 Court or the DOT Marketplace. Instead, we see potential opportunities for collaboration with these initiatives. Our unique approach to providing a comprehensive legal framework on the blockchain sets us apart and positions us to address a distinct set of challenges and needs within the Polkadot Ecosystem.

As of the time of writing, there are no known projects within the Substrate/Polkadot/Kusama ecosystem that offer the same combination of features as the Liberland Blockchain project. We are the first country to run its government (and judiciary) on the blockchain. But besides that, the unique aspect of this project is the integration of a 'court as a smart contract oracle' that enables the execution of traditional contracts on-chain and the introduction of a entity capable of interpreting intent behind actions within the blockchain. The entire world of traditional contracts is currently barred entry into the blockchain world, and we are attempting to forge a key allowing that huge, majority part of the world economy to come into the Polkadot ecosystem.

## Team :busts_in_silhouette:

### Team members

- Dorian Stern-Vukotic, Senior Developer
- Kacper Zuk, Senior Developer

### Contact

- **Contact Name:** Dorian Štern Vukotić
- **Contact Email:** [dorian.sternvukotic@gmail.com ]
- **Website:** [Liberland](www.liberland.org)

### Legal Structure

- **Registered Address:** 3/F, Chinachem Tower, 34-37 Connaught Road Central, Hong Kong
- **Registered Legal Entity:** Liberland Limited

### Team's experience

Our team has extensive experience in developing blockchain solutions. We have been working on the Liberland Blockchain, a layer 1 public blockchain owned by coin and token holders. All team members individually have 7+ years of software engineering experience with 1+ years experience with blockchain technologies, primarily Substrate, Rust and Solidity.

### Team Code Repos

- [Liberland GitHub](https://github.com/liberland/liberland)

### Team LinkedIn Profiles (if available)

- [Dorian Stern-Vukotic](https://www.linkedin.com/in/djstern)
- [Kacper Zuk](https://www.linkedin.com/in/kacperzuk/)

## Development Status :open_book:

If you've already started implementing your project or it is part of a larger repository, please provide a link and a description of the code here. In any case, please provide some documentation on the research and other work you have conducted before applying. This could be:

- **academic publications relevant to the problem:**
1. [**BLOCKCHAIN'able JUDICIARY: BLOCKCHAIN, ARTIFICIAL INTELLIGENCE, INTERNET OF THINGS and JUDICIAL SYSTEM (ONE)**](https://www.amazon.com/BLOCKCHAINable-JUDICIARY-BLOCKCHAIN-ARTIFICIAL-INTELLIGENCE/dp/1703687477) by Ismail Mohammed; This book discusses how modern technology can be used to ease complications of legal process issues and procedures.
2. [**Stanford Journal of Blockchain Law & Policy**](https://stanford-jblp.pubpub.org/): This journal publishes articles and essays related to blockchain law and policy. Some recent articles include:

3. [**On-Chain DAO Governance and Decentralized Regulation**](https://www.ssrn.com/index.cfm/en/maxplancklawrps/max-planck-luxembourg-res/) by Max Planck Institute Luxembourg for Procedural Law.

4. [**Cryptocurrency and the Family Courts - Some International Experiences**](https://financialremediesjournal.com/content/cryptocurrency-and-the-family-courts-some-international-experiences.4fc550f56143411ca515055b2ce2872d.htm) – by Financial Remedies Journal
This article discusses how cryptocurrency is being dealt with in family court cases in England.,
- **links to your research diary, blog posts, articles, forum discussions or open GitHub issues:** [development JIRA](https://liberland.atlassian.net/jira/software/projects/BLOCKCHAIN/boards/2),
- **contact with Web3 Foundation:** conversation with Seraya Takahashi from 26-07-2023

- ### **Links**
[Github](https://github.com/liberland)
[Docs](https://liberland-1.gitbook.io/wiki/v/public-documents/blockchain/)
[Testing guide](https://docs.google.com/document/d/1ntrT6bafTD2LfXUG9QLxOieogXELn9icN1y__EGfZ98/edit#heading=h.yfda4shb4ggs)
[Blockchain website](https://liberland.org/blockchain)
[Project website](https://liberland.org)
[Mainnet explorer](https://polkadot.js.org/apps/?rpc=wss%253A%252F%252Fmainnet.liberland.org#/)
[Mainnet frontend](https://blockchain.liberland.org/signin)
[Testnet explorer](https://polkadot.js.org/apps/?rpc=wss%3A%2F%2Ftestchain.liberland.org%2F#/explorer)
[Testnet frontend](https://testnet.liberland.org)
[Metaverse](https://liberverse.net/)
[Liberland Marketplace](https://market.ll.land/)

## Development Roadmap :nut_and_bolt:

### Overview

- **Total Estimated Duration:** 2 months
- **Full-Time Equivalent (FTE):**  4 FTE
- **Total Costs:** 30 000 USD.

### Milestone 1 Simple Process

- **Estimated duration:** 1 month
- **FTE:**  1,5
- **Costs:** 15,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **0a.** | License | MIT |
| **0b.** | Documentation | We will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can (for example) spin up one of our Substrate nodes and send test transactions, which will show how the new functionality works. |
| **0c.** | Testing and Testing Guide | Core functions will be fully covered by comprehensive unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| **0d.** | Docker | We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone. |
| 0e. | Article | We will publish an **article**/workshop that explains the functioning of the judiciary and its impact on the Polkadot environment |
| 1. | Substrate module: Judiciary | We will create a Substrate module that will facilitate the adjudication of cases under the Simple Process, e.g. when the parties agree on the Judge or the Judge selection method|
| 2. | Substrate module: Escrow/Collateral | We will create an Escrow solution which will also be useable in the judiciary, as explained above |
| 3. | Substrate module: Traditional Contracts | The Traditional Contracts Substrate module will enable users to turn traditional contracts into smart contracts by attaching collateral to them and the algorithmic power of each party to click on "dispute" and activate the Judiciary module |
| 4. | Substrate chain | Module Traditional Contracts will enable parties to agree to be adjudicated using the Judiciary Module, covering the court costs and the contract using the Escrow/Collateral module) |
| 5. | Frontend| We will deliver a basic frontend to operate the new substrate modules |


### Milestone 2 Example — Additional features

- **Estimated Duration:** 1 month
- **FTE:**  1,5
- **Costs:** 15,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **0a.** | License | MIT |
| **0b.** | Documentation | We will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can (for example) spin up one of our Substrate nodes and send test transactions, which will show how the new functionality works. |
| **0c.** | Testing and Testing Guide | Core functions will be fully covered by comprehensive unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| **0d.** | Docker | We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone. |
| 1. | Substrate module: Advanced Judiciary | We will create a Substrate module that will facilitate the adjudication of cases where the parties can't agree on anything more than having their case adjudicated in Liberland|
| 2. | Substrate module: Judiciary Market | We will create a module that gathers on-chain data to facilitate the operation of the marketplace of judges |
| 3. | Substrate module: Insurance | The Insurance Substrate module will enable users registered as insurers to pay collateral for others and to receive compensation based on a smart contract |
| 4. | Substrate chain | Modules X, Y & Z of our custom chain will interact in such a way... (Please describe the deliverable here as detailed as possible) |
| 5. | Frontend| Judiciary Marketplace and Insurance frontend |
| 6. | Smart contracts: ... | We will setup smart contract templates for judiciary and insurance contracts.


## Future Plans

- Liberland is a country that is currently establishing its control over the land.
- This system will become the obligate judiciary for the country's citizens and anyone who want to do business with the country.
- We are also setting up a system of promotion for the Liberland Blockchain
- The judiciary will be a big part of that
- We will also connect to 3rd party services, enabling the operation of the judiciary with their platforms
- After the success of our first Liberland Blockchain/ Polkadot conference, we will keep organizing more.

### Judiciary development future plans
- Easy to use contract builder frondend that deploys a hybrid smart/traditional contract with defined juridistictions
- Upgrade escrow functionality to adapt for use with insurance companies, allowing partial escrow etc
- Integration with the company, land and asset registry pallets to allow full legal support for on chain assets
- Setup default company hybrid contracts to support shareholders in preparation for the Liberland stock market
- Bridge more tokens so that contracts can support BTC, USDT, ETH, DOT etc...
- Instantiate a new chain with these functionalities as a parachain on Polkadot/Kusama

## Additional Information :heavy_plus_sign:

**How did you hear about the Grants Program?** Web3 Foundation Website

- **Work you have already done**: We have set up the Level 1 Liberland Blockchain, and have already received and utilized a grant from Web3 Foundation for it. The blockchain currently handles the political process, stores legislature and handles vetoes, uses assets as political token, has company, land and other asset registries, and is integrated into the Liberland metaverse
- **Other teams**: We are grateful for the help of the [Neti Blockchain Development Company](https://neti-soft.com/) They have contributed greatly to the development and we expect them to remain with us for the development of the judiciary.
- **Previous Grants**: Liberland Blockchain Level 2 Grant: accepted and paid out.
