# Cloud Forensic Introduction

## Introduction

* The exponential growth in usage of cloud computing has also led to an increase in cybercrime in the cloud.
* Features of cloud such as privacy, anonymity, multi-tenancy, etc., are attracting users to use cloud technologies. However, the same features are also exploited by criminals

### Cloud Computing
* Cloud computing is the on-demand delivery of compute power, database, storage, applications, and other IT resources through a cloud service platform via the Internet, usually on a pay-as-you-go pricing. 
* Cloud computing provides a simple way to access servers, storage, databases and a broad set of application services over the Internet. 
* In essence, application data are no longer required to be stored on the physical devices, and they are not restricted by physical locations.

### Characteristics of Cloud Computing
* It is an on-demand service where the user can instantly provision computing resources, such as server processing powers and network storage, almost instaneously
* Cloud computing's capabilities are delivered over the network and can be accessed by many user-end platform such as mobile phone, computer and thin client machines.
* The computing resources are pooled together to serve multiple users, and they are dynamically assigned and reassigned according to the user’s demands or requests.
* Capabilities can be elastically provisioned and released, in some cases, automatically, to rapidly scale outward and inward to cope with the demand
* Resource usage can be monitored, controlled, and reported for both the Provider and users.

### Cloud Services Classification
* Cloud Services are classified into 3 broad categories:
  * Software as a Service (SaaS)
  * Platform as a Service (PaaS)
  * Infrastructure as a Service (IaaS)
* In an on-premise scenario, everything from servers, storage, applications are managed within the organisations. 
* The organisation have full control and responsible for all the hardware and software of the systems
* As the oganisation move from IaaS, to PaaS, the organisation are administrating lesser of these resources. 
* Finally when we moved to Software As a Service, the underlying hardware and software resources are transparent to the users.

### Cloud Deployments
* Cloud services can generally deployed in the following ways:
  * Full Cloud Setup: All operations are carried out on cloud service providers or multiple cloud service providers.
  * Hybrid: The most common method. Usually deloyed in scenario where there is existing on-premises infrastructure. An organization's infrastructure then extend it’s deployment and grow into the cloud.
  * On-premises: The deployment of resources are usually housed at the users’ location, using virtualization and resource management tools. Commonly known as private cloud. On-premises deployment doesn’t provide many of the benefits of cloud computing but is sometimes sought for its ability to provide dedicated resources or security.

### Advantages of Cloud Computing
* Services can be delivered globally and swiftly
* Computing powers are no longer restricted by system hardware.
* It reduces the investment in IT infrastructures at the early stage of a product or service.

### Need for Cloud Forensics
* Growing trend towards cloud hosted apps and data
* Digital footprints are increasingly spread out over multiple devices, applications, and services. 
* Fragmentation of data across multiple source
* Cloud computing has become a new battlefield for cyber-crime.
* https://www.magnetforensics.com/blog/all-your-case-data-in-magnet-axiom-pt-1-why-it-matters/

## Cloud Forensic
```Cloud forensics is the application of digital forensics in cloud computing as a subset of network forensics to gather and preserve evidence in a way that is suitable for presentation in a court of law.```

* The processes and fundamentals of digital forensics and incident response have not changed. 
* The scene has change from one that is physical to one that is virtual or remote. 
* Incident response relies on network connections and the applications that we use to access the data remotely.


```Cloud  forensics  is  the  application  of  digital  forensic  science  in  cloud  computing  environments.  Technically,  it  consists of  a  hybrid  forensic  approach  towards the generation of digital evidence. Organizationally it involves interactions among cloud actors for the purpose of facilitating both internal and external investigations. Legally it often implies multijurisdictional and multi-tenant situations” ```

* Cloud forensics is a hybrid forensic approach and involves interactions among the various persons, from the cloud service providers, to the users of the cloud services and incident responders
* https://reader.elsevier.com/reader/sd/pii/S1877050916305506?token=B84B2367AD01FC55D1B3C5E58F01379DFD4E6395C73B3A3CBE07813074CF6E18EA5176F6E71E1E8D020F0DC628078999&originRegion=eu-west-1&originCreation=20220109000257

## Challenges
* This is a paper by NIST where they identify the challenges of Cloud forensic 
  * https://nvlpubs.nist.gov/nistpubs/ir/2020/NIST.IR.8006.pdf

* The objectives of first responders and forensic examiners are the same in the cloud context compared to traditional large -scale network forensics, 
* Distinctive features of cloud computing such as segregation of duties among cloud actors, the multi-tenancy, rapid deployment and virtualisation of these services introduce unique scenario for investigation
* Cloud forensics challenges cannot be solved by technology, law, or organizational principles alone.
* The challenges are classified into the following categories:
  * Architecture challenges
    * include dealing with diversity, complexity of cloud services
    * Data can reside at multiple systems, locations and endpoints.
    * How do we ensure data are properly collected while preserving chain of custody
    * Is the infrastructure able to support seizure of cloud resources without disrupting other USERS
  * Data collection challenges:
    * locating forensic artifacts in large, distributed and dynamic systems
    * locating and collecting volatile data
    * data collection from virtual machines 
    * data integrity in a multi-tenant environment where data is shared among multiple computers in multiple locations and accessible by multiple parties; 
    * inability to image all the forensic artifacts in the cloud
    * accessing the data of one tenant without breaching the confidentiality of other tenants; 
    * recovery of deleted data in a shared and distributed virtual environment
  * Analysis challenges:
    * correlation of forensic artifacts across and within cloud providers;
    * Reconstruction of events from virtual images or storage; integrity of metadata
    * timeline analysis of log data including synchronization of timestamps
    * Reconstruction of events from virtual images or storage; integrity of metadata
  * Anti-forensics 
    * obfuscation, malware, data hiding, or other techniques to compromise the integrity of evidence; 
    * malware may circumvent virtual machine isolation methods
  * Incident first responders challenges:
    * confidence,competence and trustworthiness of the cloud providers to act as first-responders to perform data collection; 
    * difficulty in performing initial triage
    * processing a large volume of forensic artifacts collected
  * Management challenges:
    * identifying the owner of an account
    * decoupling between cloud user credentials and physical users; 
    * ease of anonymity and creating fictitious identities online
    * determining exact ownership of data
    * authentication and access control
  * Legal challenges:
    * identifying and addressing issues of jurisdictions for legal access to data
    * lack of effective channels for international communication and cooperation during an investigation
    * data acquisition relies on the cooperation of cloud providers
    * missing terms in contracts and service level agreements; 
    * issuing subpoenas without knowledge of the physical location of data; seizure and 
    * confiscation of cloud resources may interrupt business continuity of other tenants
  * Standards challenges:
    * lack of even minimum/basic SOPs , practices, and tools
    * lack of interoperability among cloud providers
    * lack of test and validation procedures to ensure the processes are forensically sounded
  * Training challenges:
    * misuse of digital forensic training materials that are not applicable to cloud forensics
    * lack of cloud forensic training and expertise for both investigators and instructors
    * limited knowledge by record-keeping personnel in cloud providers about evidence; etc
    * limited knowledge by record-keeping personnel in cloud providers about evidence; etc

### Summarised
* Identification of cloud service and accounts
* Understanding the technical setup of the cloud service
* Obtaining assistance from cloud provider
* Ability of examiner to gain access to the data
* Ability of examiner to complete a forensically sounded acquisition
* Sheer volume of the data
* Ability to respond in a timely fashion
