# Cybersecurity for Industry 4.0 in the current literature: A reference framework

**Authors:** Marianna Lezzi*, Mariangela Lazoi, Angelo Corallo  
**Affiliation:** Università del Salento, Dipartimento di Ingegneria dell'Innovazione, Campus Ecotekne, Via per Monteroni, s.n. 73100 Lecce Italy

## Article Information

**Article history:**
- Received 2 July 2018
- Received in revised form 7 September 2018
- Accepted 10 September 2018
- Available online 1 October 2018

**Keywords:**
- Cybersecurity
- Industry 4.0
- Industrial Internet of Things
- Review

## Abstract

The cybersecurity issues represent a complex challenge for all companies committing to Industry 4.0 paradigm. On the other hand, the characterization of cybersecurity concept within Industry 4.0 contexts proved to be an emerging and relevant topic in the recent literature.

The paper proposes to analyse, through a systematic literature review approach, the way in which the existing state of art deals with the cybersecurity issues in Industry 4.0 contexts. In particular, the focus will be on the investigation of the main elements associated with cybersecurity theme (i.e. asset involved into cyber-attacks, system vulnerabilities, cyber threats, risks and countermeasures) within those industrial contexts where physical systems (machines, shop floors, plants) are connected each other via the Internet. Four areas of analysis are defined: definitions of cybersecurity and Industry 4.0 concepts, the industrial focus of the analysed studies, the cybersecurity characterization and the management attempts of cybersecurity issues. Through the literature review analysis, a framework of the main features characterizing each area is discussed, providing interesting evidences for future research and applications.

© 2018 Elsevier B.V. All rights reserved.

## 1. Introduction

An ever-increasing number of companies are approaching to Industry 4.0 paradigm (even known as Industrial Internet of Things or Industrial Internet), by connecting the factories and plants to the Internet with the aim to improve their efficiency and effectiveness. In these Internet-connected industrial contexts, the cybersecurity issues represent one of the most relevant challenges to be dealt with.

According to the management-consulting firm, McKinsey & Company, Industry 4.0 transformations are potentially able to create value equivalent to efficiency improvements of 15 to 20 percent [1]. This means a reduction of total machine downtime thanks to predictive maintenance or remote monitoring, as well as an increase of labour productivity due to the automation of manual work. Moreover, a certain number of benefits result from the possibility to analyse the huge amount of data coming from industrial processes (for instance, from sensors and actuators which connect machines and products to computing systems). These benefits include the reduction of inventories and the improvement of service levels (in terms of shorter time-to-market, delivery time and freight costs) and of the product quality (more compliant to the customer expectations).

Within Industry 4.0 contexts, cybersecurity plays a leading role in preventing the loss of companies' competitiveness. In fact, critical industrial equipment is today vulnerable to a number of cyber-attacks, which are able to affect the entire business model. According to Cisco 2018 Annual Cybersecurity Reports [2], 31% of organizations have experienced cyber-attacks on Operational Technology (OT); while, 38% expect attacks to extend form Information Technology to Operational Technology. Although cybersecurity is perceived as a priority by 75% of experts, only 16% say their company is well prepared to face cybersecurity challenges [3]. This is mainly due to the lack of accurate standards to which companies can refer to, as well as the lack of managerial and technical skills necessary to implement them.

European and international organizations are moving in this direction. For instance, in 2017, European Cyber Security Organization (ESCO) collected in a document all existing standards and specifications related to Cybersecurity in reference to the European Digital Single Market [4]. This document helps to understand which schemes (if existing) can be used by companies to address the cybersecurity challenges. In addition, International Electrotechnical Commission (IEC) has published a guide on information security and data privacy [5], which provides guidelines to be covered in IEC publications, and explains how to implement them. IEC Publications are recommendations (accepted by IEC National Committees) for international use.

In the current fast-moving scenario, it is expected that cybersecurity will become an integral part of the strategy, design, and operations of companies that embrace Industry 4.0 paradigm.

Through a systematic literature review approach, the purpose of the paper is to investigate cybersecurity within Industry 4.0 contexts. A reference framework as basis of future research and applications in the field of cybersecurity management in such Internet-connected industrial contexts will be defined.

The next section of the paper describes the research method, and, in particular, the search process (which includes searching criteria definition, papers selection and their assessment). In Sections 3–6, definitions of industry 4.0 and cybersecurity, the target industrial focus, cybersecurity characterization and managing of cybersecurity issues, based on the literature review, are respectively explored. The final sections, concerning findings and conclusions, end the paper.

## 2. Research Method

This study adopts the systematic literature review approach [6] with the aim to characterize the cybersecurity concept within Industry 4.0 contexts. This was achieved by investigating: the target industries to which cybersecurity refers to and the industrial assets damaged; the typology of cyber-threats and the resulting risks for the industrial contexts; the countermeasures to be taken to deal with the cyber-attack events; the guidelines and solutions to manage cybersecurity issues.

According to the systematic approach, the literature review process was based on keywords and search terms with a replicable and defined search strategy. Although the literature review cannot be considered exhaustive, this provides a significant overview of the current role played by cybersecurity within Industries 4.0, revealing as an emerging research field at international level.

### 2.1. Search Process

The search process consists of three main steps: (i) definition of searching criteria, (ii) papers selection, and (iii) papers assessment. The papers search was carried out through three important indexed electronic scientific databases: Scopus (www.scopus.com), Web of Science (www.webofknowledge.com) and Scholar (scholar.google.it). The research took place until March 2018. Chapters of books, as well as the non-scientific material coming from Google Scholar were not considered.

#### 2.1.1. Searching Criteria Definition

The criteria for searching are based on the terms "cybersecurity" and "Industry 4.0". In order to strengthen the research, some of the most significant related words to the cybersecurity concept, as well as the most accredited variants of Industry 4.0 are taken into consideration.

In particular, concerning cybersecurity, the following definitions were considered to create a properly taxonomy:

- "The ability to protect or defend the use of cyberspace from cyber attacks" [7];
- "Preservation of confidentiality, integrity and availability of information in the cyberspace" [8];
- "All activities necessary to protect cyberspace, its users and impacted persons from cyber threats" [9];
- "The protection of information assets by addressing threats to information processed, stored, and transported by internetworked information systems" [10];
- "Prevention of damage to, protection of, and restoration of computers electronic communications systems, electronic communication services, wire communication, and electronic communication, including information contained therein, to ensure its availability, integrity, authentication, confidentiality, and nonrepudiation" [11].

![Cyber Security Definition](cybersecurity-definition.png)

In Fig. 1, a schematic view of the cybersecurity concept merges information from the just mentioned definitions. It can be stated that cybersecurity aims at protecting the cyberspace (which includes both information and infrastructures) from any cyber threat or cyber-attack. Therefore, the words "cyberspace", "cyber threats" and "cyber-attacks" take part of the searching criteria for papers selection.

Due to this preliminary analysis, the first group of papers was determined through the following searching queries:

- ("Cybersecurity" OR "cyber security") AND ("Industry 4.0");
- ("Cyber attack*" OR "cyber threat*" OR "cyberspace") AND ("security") AND "Industry 4.0").

On the other hand, concerning the term Industry 4.0, the Unite States variants "Industrial Internet of Things" (even referred to with "IIoT" or "Industrial IoT") and "Industrial Internet" (coined by General Electric) were considered [12]. For this reason, the second group of papers is characterized by the following searching queries:

- ("Cybersecurity" OR "cyber security") AND ("Industrial Internet of Things" OR "IIoT" OR "Industrial IoT" OR "Industrial Internet");
- ("Cyber attack*" OR "cyber threat*" OR "cyberspace") AND ("security") AND ("Industrial Internet of Things" OR "IIoT" OR "Industrial IoT" OR "Industrial Internet").

#### 2.1.2. Papers Selection

Concerning the first group of papers, the search in Scopus, conducted into "Title", "Keywords" and "Abstract", returned 31 articles, three of which are written in German language. On the other hand, the search in Web of Science, conduced into "Topic" (involving Title, Abstract, Author Keywords and Keywords Plus), returned 15 articles, 12 of which are the same of Scopus and two are written in German language. Finally, the search in Scholar, conducted into "Advanced Research" on "Article Title" returned three articles, two of which are the same of Scopus. As a result, 30 scientific papers were identified for the first group of papers.

Regarding the second group of papers, instead, the search in Scopus returned 24 articles, four of which have already been considered in the first group of papers. On the other hand, the search in Web of Science returned 13 articles, four of which have already been considered in the first group of papers and five are the same of Scopus. Finally, the search in Scholar, conducted into "Advanced Research" on "Article Title" returned three articles, one of which has already been considered in the first group and another is the same of Scopus. As a result, 25 scientific papers were identified for the second group of papers.

Overall, 55 scientific papers were identified. However, analysing the abstract of each of them, 15 papers (four coming from the first group and eleven from the second one) were rejected since considered off topic with respect to the objectives of this literature review. Therefore, the selection phase conduced to 40 scientific papers to be assessed.

![Paper Selection Summary](paper-selection-summary.png)

#### 2.1.3. Papers Assessment

In order to evaluate the 40 papers selected, it was firstly defined a matrix to record authors notes about each of these papers. This matrix is composed of 17 records, in which the following information was collected: title, authors with affiliations, publication year, source, reference, abstract, keywords, study focus, industry, definition of industry 4.0/Industrial Internet of Things (and variants), definition of cyber security, industrial asset involved into cyber security risks, systems security vulnerabilities, cyber threats, risks related to cyber attacks, and methods to deal with cyber security risks.

The second phase of the papers' assessment involved the analysis, in a critical way, of the most significant information identified for each paper. The same categories of information was compared among all different papers and the main findings discussed. In particular, the following areas were taken into consideration:

1. Analysis of the concept of Industry 4.0/Industrial Internet of Things (or variants) and that of cybersecurity;
2. Definition of the target industry threatened by cybersecurity risks and the industrial assets involved in the cyber-attack events;
3. Characterization of the cybersecurity concept, in terms of: systems security vulnerabilities, cyber threats, risks due to cyber-attacks and countermeasures to be taken;
4. Overview on guidelines and solutions proposed to manage cybersecurity issues.

The results of this comparative review are reported in the following sections.

## 3. Definitions

After having analysed the first group of papers, the main features of Industry 4.0 emerged from a certain number of definitions; while only a paper defined the cybersecurity concept as "the protection of theft or damage to IT hardware, software and the data stored on the systems" [13].

A comparative analysis across the definitions of Industry 4.0 in reference to cybersecurity, allowed us to notice that some keywords (such as, Internet of Things, Cyber-Physical Systems, manufacturing and data networking) are very common in the selected papers. These words highlight that Industry 4.0 is characterized by two enabling (technological) conditions (i.e. Internet of Things and Cyber-Physical Systems), a target industrial context (i.e. manufacturing), and an enabled condition (i.e. data networking). Consequently, combining all definitions, it can be stated that Industry 4.0 is mainly associated with the concepts of Internet of Things (IoT) and Cyber-Physical Systems (CPS) within manufacturing industrial contexts, entailing the networking of data coming from machines, products, people and, in general, the interconnection of smart devices among different plants and factories.

**Table 1 - Industry 4.0 Key Words**

| Enabling (technological) conditions | Industrial context | Enabled condition |
|---|---|---|
| Industry 4.0 | Internet of Things (IoT) | Cyber-Physical Systems (CPS) | Manufacturing | Data networking |
| Papers reference | [14–17] | [16,18,19] | [14–16] | [14–16], [20,21], [17] |

At the same way, due to the analysis of the second group of papers, it was possible to investigate on the concept of Industrial Internet of Things (IIoT), even referred as Industrial Internet by General Electric in 2014 [22]. To this purpose, a number of definitions were collected. On the other hand, only a paper among those selected described cybersecurity, as that condition where "a system does what it is supposed to do and no more" [23].

As for the first group of papers, also in this case, a comparative analysis across IIoT definitions associated with the cybersecurity issues have revealed some common keywords (such as, sensors, cloud technologies, manufacturing and IoT devices networking), which enable to characterize the IIoT concept. In particular, three main elements emerged:

1. The presence of some enabling technologies (i.e. wireless sensor networks and cloud technologies) that, with the support of advanced industrial analytics and intelligence machine applications, play increasingly more pivotal roles in controlling and monitoring functionalities of facilities;
2. The application of these technologies within manufacturing industrial contexts (with particular reference to Industrial Control Systems);
3. The fact that IoT devices (associated with machines, computers and people) are networked.

Putting together the previous concepts, it can be stated that Industrial Internet of Things is related to the use of wireless sensor networks (to monitor functionalities of facilities) and cloud technologies (to manage data produced by sensors) within manufacturing industrial contexts. In this reference, a set of IoT devices, associated with machines, computers and people, are networked, and communicate and interact with each other.

**Table 2 - IIoT Key Words**

| Enabling (technological) conditions | Industrial context | Enabled condition |
|---|---|---|
| Industrial Internet of Things | Wireless sensor networks | Cloud technologies | Manufacturing | IoT devices networking |
| Papers reference | [24,25,22] | [24,26,27] | [24,28,25] | [29,26,28,27] |

![Comparison between Industry 4.0 and Industrial Internet of Things](comparison-industry40-iiot.png)

## 4. Industrial Focus

This section aims at analysing the types of industry and the related assets threatened by cybersecurity issues within Industry 4.0 and Industrial Internet of Things contexts, focusing on the industrial assets directly involved in the cyber-attack events.

Due to the analysis of the two groups of papers, it can be noticed that the manufacturing industry results the main sector in which the different studies deal with the cybersecurity issues. In fact, referring to the first group of papers, 15 on 26 papers explicitly mention it. Moreover, six papers refers to Critical Infrastructures (CI)¹, without providing more details. However, CI can include a number of sectors (among them the manufacturing one), such as [30]: chemical, commercial facilities, communications, critical manufacturing, dams, defence industrial, emergency services, energy, financial services, food and agriculture, government facilities, healthcare and public health, information technology, nuclear, transportation systems, and waste and wastewater systems. On the other hand, only one paper explicitly refers to healthcare industry, while for three of them the industry is not specified.

At the same way, considering the 14 papers taking part of the second group of papers, six of them explicitly refer to the manufacturing industry; while, the remaining part splits in the following way: one paper focuses on Critical Infrastructures, three refer to energy industry, one to telecommunication, and for three of them the industry is not specified.

Regarding the industrial assets involved into cyber-attack events, all papers of both groups point out Industrial Control Systems (ICS) and Cyber-Physical System (CPS) as the vulnerable systems to be protected.

The Industrial Control System (ICS) is a management and control system, which can ensure that the industrial technical facilities run automatically, while controlling and monitoring the business processes [31]. In particular, ICSs consist of combinations of control components (e.g., electrical, mechanical, hydraulic, pneumatic) that act together to achieve an industrial objective (e.g., manufacturing, transportation of matter or energy) [32]. These systems are commonly used in the critical infrastructures, especially in the electrical, water and wastewater, oil and natural gas, chemical, transportation, pharmaceutical, pulp and paper, food and beverage, and discrete manufacturing (e.g., automotive, aerospace, and durable goods) industries [32].

The term Cyber-Physical System, instead, identifies anything that integrates computation, networking and physical processes. In other words, these systems enable the virtual digital world of computers and software to merge through interaction with the physical analogue world. For instance, a smart manufacturing line can be considered a CPS whether the machines perform many work processes by communicating with the components and/or the products they are in the process of making [12].

**Table 3 - Industry Analysis**

**First group of papers**

| Industry types | Manufacturing | Critical Infrastructure | Healthcare | Not specified |
|---|---|---|---|---|
| Industrial assets involved | ICS | CPS | ICS | CPS | Service Platform | ICS | CPS |
| Papers reference | [37,15,38–40,17,41] | [14,15,42,21,43,13,44,18,45] | [46,47,16,48] | [49,19] | [50] | [20,51] | [52] |

**Second group of papers**

| Industry types | Manufacturing | Critical Infrastructure | Energy | Telecommunication | Not specified |
|---|---|---|---|---|---|
| Industrial asset involved | ICS | CPS | ICS | ICS | Not specified | ICS | CPS |
| Papers reference | [53,22,28,54,24] | [28,24,55] | [56] | [27,26,57] | [58] | [25,23] | [29] |

¹ European Commission defines critical infrastructure as "an asset or system, which is essential for the maintenance of vital societal functions" [61].

## 5. Cybersecurity Characterization

Once having identified the industrial assets mainly involved into cybersecurity issues in Industry 4.0 contexts (in other words, what needs to be protected), this section takes advantages of:

1. The definition of the intrinsic vulnerabilities of the systems that undermine their security;
2. The cyber threats affecting the systems;
3. The risks associated with the cyber-attacks;
4. The countermeasures to deal with cybersecurity issues.

These elements are all associated with the cybersecurity concept. In particular, (1) and (2) answer the question "what is to be protected against?"; (3) highlights the potential risks for the company due to the exploitation of the system vulnerabilities at the hand of cyber-attacks (that is, "what are the impacts?"); finally, (4) answers the question "how should you protect yourself?".

![Cybersecurity Characterization](cybersecurity-characterization.png)

### 5.1. Systems Vulnerability

Vulnerabilities are defined by Jansen and Jeschke [52] as weaknesses in the IT or automation systems that might be exploited by hackers to compromise the cyber-physical system. In a more general perspective, NIST (National Institute of Standards and Technology) glossary of key information security terms [7] refers to vulnerability as weakness in an information system, system security procedures, internal controls, or implementation that could be exploited or triggered by a threat source.

Vulnerabilities can be classified referring to remote access, software and Local Area Network (LAN) [47], and can be associated with both virtual machines belonging to cloud resources and IT systems [21].

Although there are different types of vulnerabilities which affect CPSs or ICSs, very common are those unknown (i.e. zero-day vulnerabilities) [46,21,27,57,55]; these are placed in every interfaces between different components where there is information exchange [14]. In particular, there are a number of vulnerabilities in each component of SCADA systems, in particular concerning: communication infrastructure and network protocols, application server, database server, human machine interfaces, program logic controllers, remote terminal units [40,48].

The evidence shows that IoT devices are attractive targets for botnets because of security is not a priority for many manufacturers. This is confirmed by the use of default passwords and open ports, the lack of built-in mechanisms to receive automatic firmware updates, and the fact that firmware are often forgotten about once installed (owners do not know when their devices are used for malicious purposes or when firmware need to be updated) [17].

Jansen [17] pinpoints the following reasons as cause of most industry devices get hacked:

- Devices in many plants run for weeks or months without any security updates or anti-virus tools;
- Many of the controllers used in ICS networks can be disrupted by malformed network traffic or even by high volumes of correctly-formed traffic since they were designed in an era when cybersecurity was not a concern;
- Many ICS networks have multiple pathways through which cyber-security threats can enter, bypassing existing cybersecurity measures (for instance, laptops which are carried in and out of facilities or USB sticks which are used among multiple computers, without being properly checked for malware);
- Many ICS networks are still implemented as a large, flat network, with no physical or virtual isolation between unrelated networks (allowing the spread of malware even to remote plant sites).

In order to address these problems, companies should undertake a vulnerability assessment process able to identify and assess potential vulnerabilities of systems [54]. In particular, NIST [7] defines the vulnerability assessment as "systematic examination of an information system or product to determine the adequacy of security measures, identify security deficiencies, provide data from which to predict the effectiveness of proposed security measures, and confirm the adequacy of such measures after implementation".

### 5.2. Cyber Threats

The NIST glossary defines threat as "any circumstance or event with the potential to adversely impact organizational operations (including mission, functions, image, or reputation), organizational assets, individuals, other organizations, or the Nation through an information system via unauthorized access, destruction, disclosure, modification of information, and/or denial of service" [7].

Attacks to interconnected physical systems can be characterized by three dimensions [41]:

1. The type of attacker to the system (i.e. insider or outsider);
2. Attacker's aims and objectives (i.e., destruction at a larger scale or on a specific target);
3. The attack mode (i.e., active or passive).

Regarding the attack mode, active attacks aim at making changes to system resources or affecting system operations (some examples are Distributed Denial of Service attacks and Compromised-Key attacks); while, the passive attacks goal is to learn or make use of information from a system rather than making any changes on the system (this category includes eavesdropping and sniffing attacks) [54].

Furthermore, Roy et al. [43] consider three main layers in which cybersecurity threats could act:

1. Aware execution layer (i.e. from sensors and actuators);
2. Data transport layer (i.e. from network architecture);
3. Application control layer (i.e. from user data storage).

In particular, the first layer includes physical attacks, equipment failures, failures of node power lines and electromagnetic interferences. In the second layer, there are denial of service attacks, routing attacks, aggregation node attacks, flood attacks (exhausting the network resources), black hole attacks, direction misleading attacks, Sybil attacks by adding malicious nodes. Finally, the third layer, characterized by unauthorized accesses and taking over control of machines, as well as by dispatching of malicious code, entails the leakage of user privacy and data confidentiality in data mining operations.

The German Federal Office for Information Security (Bundesamt für Sicherheit in der Informationstechnik - BSI) identifies the following main categories of cyber threats referring to Industry 4.0 contexts [21]:

- Direct attacks on external accesses;
- Indirect attacks on the IT systems of the service provider for which the external access has been granted;
- Unknown attack vectors without detection capabilities enabled by unknown vulnerabilities (or zero-day exploits);
- Non-targeted malicious software which infects components and impairs in their functionality;
- Intrusion into neighbouring networks or network segments (for instance, the existing office network).

**Table 4 - Cyber Threats List**

| Cyber threats | Reference |
|---|---|
| Transfer data from and to unauthorized devices | [46,38,51,48] |
| Denial of Service (DoS) attack using massive traffic | [46,47,38,39,40,51,54,55,27,25,42] |
| Escalation of privilege | [47,38,42] |
| Data tampering, spoofing or man-in-the-middle attacks | [38,42] |
| Eavesdropping or data interface | [38,41,24] |
| Repudiation attacks | [38,42] |
| Jamming, Collision, Fake Location Injection, Sybil, Node Replication, Wormhole, Sinkhole, False Routing Information, and Selective Forwarding | [48] |
| Malware, worms and viruses infection (in accidentally or intentionally way) | [17,41,27,25] |
| Abnormal operations induction by using abnormal Distributed Network Protocol (DNP3) function code | [46] |
| Scan DNP3 data points through changing object qualifier | [46] |
| Zero-day attacks | [47,55] |
| Phishing attacks | [54,55,27,25,29] |
| Physical destructions | [41,24] |
| Insider attacks and unwitting behaviours | [41,27] |
| Advanced Persistent Threat (APT) | [55,27,25] |
| Social engineering attacks | [27] |

In the literature, the most mentioned cyber threat is Denial of Service attack. This attack makes the systems not respond to legitimate command from the network [54]. In particular, the attackers flood the controller to force the system and change its behaviour. A common variant of DoS attacks is the Distributed Denial of Service (DDoS) attack where the incoming traffic flooding the victim originates from many different sources (multiple compromised computer systems).

### 5.3. Risks

According to NIST [7], risk is "the level of impact on organizational operations (including mission, functions, image, or reputation), organizational assets, or individuals resulting from the operation of an information system given the potential impact of a threat and the likelihood of that threat occurring".

Security risks related to information systems depend on the loss of confidentiality, integrity, or availability (known as "CIA triad") of information or information systems [49]. In particular, confidentiality refers to the ability to keep information secret from unauthorized users; in this way, the lack of confidentiality may result in data disclosure. Integrity, which means to protect the trustworthiness of data or resources, might entail deception attacks if it is not preserved. In this case, the risk concerns the corruption or modification of records and data and data loss. At the end, availability represents the ability of a system to be accessible and usable on demand; for this reason, when system availability is not guaranteed, denial of service may occur (this causes a lack of productivity at the physical system).

At the business level, cyber threats may have a certain number of negative impacts.

**Table 5 - Business Impacts**

| Business impacts | Reference |
|---|---|
| Sabotage to the entire critical infrastructure or target machines and components (e.g., loss of observability, controllability or eventually the loss of power in the physical system) | [47,42,38,40,41,52,45,29,55,27,23,59] |
| Denial of service of networks and computers | [28,16,27] |
| Theft of industrial trade secrets and intellectual property | [8,16,55,27] |
| Compliance violation in the fields of safety and pollution | [41,52,23] |
| Life-threatening situations for the workers | [59,52] |

The sabotage to the entire critical infrastructure or specific machines and components is the most cited business impact among the analysed papers. This impact is strictly correlated to DoS attacks, which in turn are the most mentioned in the literature.

In general, any of the impacts identified translate into a drop in the company productivity and competitiveness (in terms of degradation of the product quality, reduction of production rate, increasing of maintenance efforts, and delays to fulfil demand) [45,27,54,23]. In other words, the company incurs in higher costs and loss of profitability.

### 5.4. Countermeasures

Countermeasures stands for a set of actions, devices, procedures, or techniques that meet or oppose a threat, a vulnerability, or an attack by eliminating or preventing it, by minimizing the harm it can cause, or by discovering and reporting it so that corrective action can be taken [7].

Jansen [17] refers to the following three high level approaches to guarantee security of Industrial Control Systems:

1. Harden the perimeter, which means to isolate the plant network from the office network with the use of firewalls and demilitarized zone (DMZ) if necessary;
2. Defence in depth, by applying several layers of defence throughout the network, in order to stop and contain those malware breaching the perimeter.
3. Remote access, which is one of the most common ways to penetrate the perimeter firewall. In such case, the use of Virtual Private Network is recommended to isolate remote users in a separate demilitarized zone.

Moreover, with the aim to keep the protection up-to-date, it is necessary to continuously update the implemented security controls on device level (installing new security patches), network level (updating firewall signatures of new threat) and plant/ factory level (monitoring and analysing the actual log sources) [52].

**Table 6 - Countermeasures List**

| Countermeasures | Reference |
|---|---|
| Encryption | [47,42,38,51,24,26,54,27,53,23] |
| Fuzzing to detect software safety errors | [47,53] |
| Obfuscation to obscure the intended meaning of communication by making the message difficult to understand | [47] |
| Patching to solve security vulnerabilities or bugs in the systems | [47] |
| Vulnerability scan | [47] |
| Firewall/zoning, gateway and proxy | [47,40,25,23] |
| Access control (i.e. user authentication, multiple-terminal authorization) | [47,54,27,25,53] |
| Quarantine to isolate infected files on a computer's hard disk | [47] |
| Isolation of data, language, sandbox, Virtual Machine (VM) and Operating System (OS) | [54] |
| Physical resource-based isolation, also known as air gap | [54] |
| Software updates | [20,53] |
| Machine Learning (ML) method on physical data, covering k-Nearest Neighbours (kNN) algorithm, random forest algorithm and anomaly detection algorithm to real-time detect the malicious attacks | [44] |
| Physical protection through shielded wires for physical links and utilizing separated racks or spaces | [54] |
| Tamper proof hardware to prevent attackers from altering system operations and conducting falsification of data | [54,27] |
| Keep data distributed instead of centralising them into one, more vulnerable central storage point | [27] |
| Local storage and analytics so that the raw data do not leave the hardware, and any analytics can be run locally | [27] |
| Intrusion Detection System (IDS) and Intrusion Prevention System | [25] |
| Secure Communication (Virtual Private Network, Secure Sockets Layer, IP Security) | [25,53,22] |
| Antivirus and antimalware | [25,53] |
| Vulnerability assessment (process of defining, identifying, classifying and prioritizing vulnerabilities in computer systems, applications and network infrastructures) | [25] |
| Known vulnerability testing | [53] |
| Static source code analysis to look for software weaknesses | [53] |
| Penetration testing to evaluate and exploit vulnerabilities | [53] |

In the literature, encryption seems to be the most adopted countermeasures. This technique converts plain-text data into cipher-text, which can be decoded only by authorized parties who have a key. There are different levels of encryption [42,38]: encryption of the communication between entities in a networked production to mitigate tampering, information disclosure, and denial of service threats; encryption of stored data and use of digital signatures to mitigate repudiation attack; encryption of the data streams to deal with tampering with data, repudiation, information disclosure and denial of service.

## 6. Managing of Cybersecurity Issues

In this section, an overview of the guidelines and solutions proposed by the selected papers to manage cybersecurity issues within Industry 4.0 contexts is provided.

These guidelines and solutions reflect the existence of a certain number of security standards and guidance documents, which create a common understanding of industry specific security controls and methods for assessing the effectiveness of such controls [53]. In particular, the analysed papers mainly refer to:

- NIST 800-53, which provides a set of security control categories and families (i.e. access control, awareness and training, audit and accountability, security assessment and authorization, configuration management, contingency planning, identification and authentication, incident response, maintenance, media protection, physical and environmental protection, planning, personnel security, risk assessment, system and services acquisition, system and communications protection, system and information integrity, program management);
- IEC 62443 series of standards, which evaluates the potential weak points in the overall organization, component and system development process for Industrial Control Systems, with the aim to identify threats and manage cyber risks;
- UL 2900 series of standards, which contains foundational security requirements and testing criteria for software and devices within products.

### 6.1. Guidelines

**Table 7 - Cybersecurity Guidelines**

| Guideline | Reference |
|---|---|
| Providing support to connected products in the field of: cybersecurity consulting, risk management, threat monitoring, cyber incident response, training, cybersecurity packages. | [13] |
| Defining a security approach focusing on network level, transport level, and application level. | [16] |
| Appling a set of actions (focused on information to be protected, the type of threats and the influence necessary to prevent or correct unauthorized accesses) in order to guarantee information security. | [58] |
| Respecting four main steps (design the service, definition of operations, implementation of DevOps, and introduction of control loops) with the aim to implement industrial security services. | [49] |

Focusing on the manufacturing industry, Huxtablea and Schaefera [13] suggest that a firm should offer support to its connected products, in particular in the fields of:

- Cybersecurity consulting to give advice and guidance with regard to cybersecurity strategy at a top level;
- Risk management to prevent cyber-attacks;
- Threat monitoring and detection to provide software and hardware that allow cyber threats to be monitored and detected;
- Cyber incident response to limit damage and prevent further cyber-attack;
- Training to limit the likelihood of attacks taking place;
- Cybersecurity packages in relation to the products being sold (basic subscriptions might include anti-malware software as a service, by offering for instance monitoring, detection and training).

### 6.2. Solutions

**Table 8 - Cybersecurity Solutions**

| Solution | Reference |
|---|---|
| **Framework** | |
| Framework based on the areas of system identification, resilience objective setting, vulnerability analysis, and stakeholder engagement. | [37] |
| NIST framework comprises of five core functions: identification, protection, detection, response, and recovery. | [25] |
| **Approach** | |
| DevOps approach identifies the log sources for security monitoring of comparable asset classes. | [52] |
| Attack tree approach, where the problem is shown as root and its sources as leaves. | [47] |
| **Method** | |
| Collection of a set of risks evaluation methods and quantitative and qualitative methods to calculate the likelihood of attacks on certain components of the systems if other parts are attacked. | [54] |
| STRIDE security analysis of Microsoft as a threat modelling method. | [42,38] |
| **Model** | |
| Process model of VDI/VDE guideline 2182 that considers IT security along the whole life cycle of industrial system. | [21] |
| **Methodology** | |
| Methodology for assessing vulnerabilities in Industrial Control Systems, which entails actions at the level of component, subsystem and operation. | [48] |
| CYBEX methodology is based on five-level block model of data exchange (Information Description, Information Discovery, Information Query, Information Assurance, and Information Transport) to protect data exchange between customers. | [58] |
| **Architecture** | |
| Functional architecture (including a predictive model, an analysis module, a template repository, a distance function, a decision-making module) to support a protection system for Industry 4.0 applications. | [18] |

## 7. A Framework for Cybersecurity in I-4.0

In the literature, the cybersecurity and Industry 4.0 terms started to be strongly correlated since 2015. This was revealed by the electronic scientific databases adopted in this study, which gave back papers where both terms could appear in the title, within the abstract, or as key words.

In fact, although the Industry 4.0 paradigm was used for the first time in Germany in 2011 during the Hannover Fair [60], the awareness of the relevance of cybersecurity issues for the industrial physical systems connected into the network (and for the industrial information correlated to them) has spread only some years later. Still today, this topic needs to be better investigated, in order to provide a more systematic view of its main elements, and support the industrial management environment to face the cybersecurity challenges.

**Table 9 - Framework of References for Cybersecurity Research in I-4.0**

| Area of analysis | Topic | Features |
|---|---|---|
| **Analysis of definitions** | Cybersecurity | Strictly correlated words: cyberspace, cyber threats and cyber-attacks. |
| | Industry 4.0 | Enabling technological conditions: Internet of Things and Cyber-Physical Systems.<br>Target industry: manufacturing.<br>Condition enabled by the technology: data networking. |
| | Industrial Internet of Things (IIoT) | Enabling technological conditions: wireless sensor networks and cloud technologies.<br>Target industry: manufacturing.<br>Condition enabled by the technology: IoT devices networking. |
| **Study of industrial context** | Industry types | Most frequently mentioned industry: manufacturing. |
| | Industrial assets | Main vulnerable systems: Industrial Control Systems (ICS) and Cyber-Physical System (CPS) |
| **Analysis of cybersecurity in Industry 4.0 (or IIoT) contexts** | System security vulnerability | Most common vulnerabilities: zero-day vulnerabilities.<br>Suggestion: undertake a vulnerability assessment process. |
| | Cyber threats | Levels of action: aware execution layer, data transport layer, application control layer.<br>Main points to focus on: type of attacker, attacker's aims and objectives, and attack mode.<br>Most mentioned cyber threat: Denial of Service attack.<br>Main consequences: unauthorized use, disclosure, disruption, modification, or destruction of critical data and/or data interfaces; denial of service of networks and computers.<br>A list of attacks affecting ICS and CPS. |
| | Risks | Cause: loss of confidentiality, integrity and availability of information or information systems.<br>Risk typologies: data disclosure (loss of confidentiality); corruption or modification of records and data loss (loss of integrity); denial of service (loss of availability).<br>Impacts at business level: sabotage to the infrastructure or machines and components; denial of service of networks and computers; theft of industrial trade secrets and intellectual property; compliance violation in the fields of safety and pollution; life-threatening situations for the workers.<br>Most mentioned business impact: sabotage to the infrastructure or machines and components. |
| | Countermeasures | Main categories: isolation of the plant network; application of several layers of defence; isolation of remote users.<br>Main action: update the security controls on device level, network level and plant/ factory level.<br>Most mentioned countermeasure: encryption techniques.<br>A list of countermeasures. |
| **Identification of management attempts** | Cybersecurity guidelines | Security standards and guidance documents: NIST 800-53, IEC 62443 and UL 2900.<br>A set of guidelines to deal with cybersecurity issues. |
| | Cybersecurity solutions | Security standards and guidance documents: NIST 800-53, IEC 62443 and UL 2900.<br>A set of solutions to deal with cybersecurity issues. |

## 8. Conclusions

This study explored the cybersecurity issues within Industry 4.0 contexts, using a structured approach for the literature review through a qualitative analysis of the contents coming from the selected papers. In particular, the papers' assessment focused on four areas of analysis. These areas involve: (1) the analysis of cybersecurity and Industry 4.0/IIoT definitions; (2) the study of industry type and industrial assets mainly affected by cybersecurity issues; (3) definition of systems vulnerabilities, cyber threats, risks and countermeasures to be taken, with regard to Industry 4.0 scenarios; (4) identification of guidelines and more structured solutions to deal with cybersecurity issues.

As a result, a reference framework of the main features for each area was defined. The framework collects the most cited evidences for each area of analysis and summarizes them for providing an immediate prospect of synthesis useful to lead future research but also the managerial actions.

Although a number of different solutions for dealing with cybersecurity issues within Industry 4.0 have been already developed, none of them take into consideration, at the same time, the three exposure layers of Cyber Physical Systems (physical, network and computation) that could be abused by cyber-attacks. For instance, in the research of Flatt et al. [21], the physical aspects are treated but without an integration with networking and computation processes; while, in the studies of Preuveneers and Ilie-Zudor [42] and Preuveneers et al. [38] the aspects of networking is treated without an integration with the others elements of the system.

Moreover, papers analysed do not face cybersecurity theme with a purely management perspective, but they focus on IT side. A management perspective should support companies in the correct implementation of new organizational practices and initiatives of change management.

Future research can use this study as reference framework to address investigation in the industrial field and enlarge the current state of art. From the managerial point of view, instead, the study provides a shortcut to a complete view about cybersecurity in I-4.0 that can be used as basis for supporting the decision making process about cybersecurity issues but also a reference material for training in IT department.

## References

[References 1-61 are listed in the original document but omitted here for brevity]

---

*Corresponding author: marianna.lezzi@unisalento.it*