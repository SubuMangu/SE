# Ch 1: Introduction
## What is Software Engineering?
- **Definition:** Software engineering discusses systematic and cost-effective techniques for software
development.  These  techniques  help  develop  software  using  an  engineering
approach.

### Is Software Engineering Science or Art?
- Software engineering is not as rigid as science, but also not as flexiblea art.
- In science everything is structured,but unlike SE for a problem there exists a single solution which is theoretically proven.
- In art opinions are subjective(depend on people) , but unlike SE there is no way to evaluate opinion and it is unstructured.
- Hence, software engineering, like other engineering disciplines, there exists multiple solutions,but the best solution is chosen, which gives the best tradeoff among all the factors like cost, maintainability, usability.

## Evolution of Art to Engineering
<p align="center"><img src="Images/Screenshot 2025-05-09 190108.png" width="" height=""></p>

- Initially, an idea is developed as an esoteric **art**, where less people are involved.
- Esoteric means small group discussion,
- As more people find the idea interesting, they involve and at this point, the idea is converted from art to **craft**.
- Even though many people involved at this point, but it is implemented in an unorganised manner.
- So later on, the idea is implemented in organised manner to large scale production and it is finally transformed from craft to **engineering**. 

- **Example(Evolution of Iron Making technology):**  Consider the evolution of the iron making technology. In ancient times, only a few people knew how to make iron. Those who knew iron making, kept it a closely-guarded secret.This esoteric knowledge got transferred from generation to generation as a family secret. Slowly, over time technology graduated from an art to a craft form where tradesmen shared their knowledge with their apprentices and the knowledge  pool  continued  to  grow.  Much  later,  through  a  systematic organisation and documentation of knowledge, and incorporation of scientific basis, modern steel making technology emerged.
- Software engineering also evolved in the same manner:
    1. In  the  early  days  of  programming,  there  were  good programmers and bad programmers. The good programmers knew  certain principles  (or  tricks)  that  helped  them  write  good  programs,  which  they seldom shared with the bad programmers.
    2. Then people involved in dicussing about these tricks and it transformed to craft
    3. Over the next several years, all good principles (or tricks) that were organised into a body of knowledge that forms the discipline of software engineering. 

## Software Crisis and it's solution
- Software crisis refers to increase in software price compared to the hardware price.
- Sometimes the software prices crosses the price of the hardware on which the software is runed

**Reason:** rapidly increasing problem size, lack of adequate training in software engineering techniques, increasing skill shortage,  and  low  productivity  improvements.

**Solution**
- Following the principles of software engineering

## Program vs Product
- There is a difference betweena toy software or program written by a student in his first programming assignment and a professional software which is implemented on a large scale as product.

|Slno.|Program(Toy Program)|Product(Professional Application)|
|-|-|-|
|1. Size|Small in size|Large and complex to be developed by a group of developers working in a team.|
|2. Functionality|Support limited functionalities and lacks good interface.|Have good software interfaces and more functionalities|
|3. Team Size|Written by a individual programmer|It  is  usually developed by a group of developers working in a team.|
|4. Documentation|Lacks proper documentation|It cointains all the documents like requirements specification document, design document, test document, users’ manuals, etc.|
|5. No of user|Single or less user|Scalable enough to generate revenue|
|6. Structuredness|Program donot follow structured paths like DFD,UML|Follows DFD,UMLs|

## Types of Software Development Projects
- There are 2 types of Software Development Projects: Software Products and Software Services

### Software Products
- These are the software available off-the-shelf(pre-made) and used by diverse range of customers. Hence they are known as **Generic Software products**.
- Since these kind of companies need to target a lot of users,It cannot be possible at once.Hence, each software product is targeted to some market segment(set of users).
- One way to this is to develop product lines that target slightly different market segments based on variations of essentially the same software.For  example,  Microsoft  targets  desktops  and  laptops  through  its Windows 8 operating system, while it targets high-end mobile handsets through  its Windows  mobile  operating  system,  and  targets  servers through its Windows server operating system.

### Software Services
- A software service usually involves either  development  of  a **customised software**  or  development  of  some  specific  part  of  a software  in  an outsourced mode known as **outsourced software**.

**Customised Software**
- A *customised software* is developed according to the
specification drawn up by one or at most a few customers.
- These need to be developed in a short time frame (typically a couple of months), and at the same time the development cost must be low.
- A customised software is developed by tailoring some of its existing software.

**Outsourced Software**
- Outsourced software means that a company gives part of its software development work to another company (usually a smaller or specialized one) to do the job.
- It is preferred in the following conditions:
    1. **Lack of expertise -** The main company might not be good at doing a certain part (like UI design or security), so they let a specialist company handle it.
    2. **Cost savings –** Another company might do the same work at a lower cost.
    3. **Speed –** If the main company is busy or wants the project done faster, they let someone else do part of the work.

## Exploratory Style Software Development
<p align="center"><img src="Images/Screenshot 2025-05-10 115301.png" width="" height=""></p>

- Here development starts  after  an  initial  briefing  from  the customer. Based on this briefing, the developers start coding to develop a working program. The  software  is  tested  and  the  bugs  found  are fixed. This cycle of testing and  bug fixing continues till the software works satisfactorily for the customer.
-  An  exploratory  development  style  can  be  successful  when  used  for developing very small programs, and not for professional software.
- The graph given below shows the increase in development time.With increase in programme size,for different software development procedure.

<p align="center"><img src="Images/Screenshot 2025-05-10 120104.png" width="" height=""></p>

- The main reason behind unsuitability of exploratory style software development is the exponential increase in development time with respect to increase in programme size as shown in graph.The cause for this exponential increase is human cognitive limitations.

**Other disadvantages of Exploratory sytle of softwre development**
- The  exploratory  style  usually  results  in  unmaintainable  code.  The reason for this is that any code developed without proper design would result in highly unstructured and poor quality code.
- It  becomes very  difficult  to  use  the  exploratory  style  in  a  team development environment. In the exploratory style, the development work  is  undertaken  without  any  proper  design  and  documentation. Therefore it becomes very difficult to meaningfully partition the work among a set of developers who can work concurrently

# Ch 2: Software Life Cycle Models
- Looking at the drawbacks of exploratory style software development, we got to know that.We need to follow a well defined and ordered software development procedure
-  **Definition of Software Development Life Cyle:** The well defined set of activities in software development are **graphically modelled(represented)** and **textually described(documented)** are known as software lifecycle model or software development lifecycle model.

- Classical waterfall model is used as the base of all software development lifecyle models.
- The software development life cycles that we will discuss here are suitable for long term product development projects like  (like building an entire search engine by google)
- Later on when there was rise of small serviced based projects ,these software development models are not suitable,which led to rise of agile models. 
- Agile models are not a result of upgrade in general software development models, it is just suitable for small service based projects. 

## Software Life Cycle
- Generally, while building a software, we face the following phases:
    1. **Inception Phase:** In this phase the customer feels a need for the software and forms rough ideas about the required features.  
    2. **Development Phase:** Starting with the inception stage, a software evolves through a series of identifiable stages (also called phases) on account of the development activities carried out by the developers, until it is fully developed and is released to the customers.
    3. **Maintainance Phase:**  Maintenance phase  usually  involves  continually  making  changes  to  the  software  to accommodate the bug-fix and change requests from the user.
    4. **Operation Phase:** It is the longest phase which constitutes the useful life of the software.
    5. **Termination Phase:** Finally the software is retired, when the users do  not find it any longer useful due to reasons such as changed business scenario, availability of a new software having improved features and working, changed computing platforms, etc.

### Software Development Life Cycle Models
- An SDLC graphically depicts the different phases through which a software evolves. It
is usually accompanied by a textual description of the different activities that need to
be carried out during each phase.

## Process vs Methodology
- A  **process**  usually  describes  all  the  activities starting from the inception of a software to its maintenance and retirement stages, or at  least  a  chunk  of  activities  in  the  life  cycle.
- A **methodology**, in contrast, describes
the steps to carry out only a single or at best a few individual activities.
- Process is an accumulation of a number of methodologies, whereas methodology is a single unit.

## Need of Documentation
- It  is  not  enough  for  an  organisation  to  just  have  a  well-defined development  process,  but  the development  process  needs  to  be properly documented.
- The following reasons support for the same:
    1. A documented process model ensures that every  activity  in  the  life  cycle  is  accurately  defined.Without documentation, the activities and their ordering tend  to  be loosely defined, leading to confusion and misinterpretation by different teams in the organisation. 
    2. It is easier to tailor a documented process model, when it is required to modify certain activities or phases of the life cycle.  
    3. A software company must have a documented process to meet quality standards like ISO 9000 or CMM, or else it may lose customer trust and miss out on contracts.

## Phase Entry and Exit Criteria
- A good SDLC besides clearly identifying the different phases in the life cycle, should unambiguously define the entry and exit criteria for each phase.
-  The phase entry criteria is usually expressed as a set of conditions that needs to be be satisfied for the phase to start (or to complete). 
- The phase exit criteria refers to the expected outcome of a phase.

**99% complete syndrome**
- When the phase entry and exit criteria are not well-defined, the developers might close the activities of a phase much before they are actually complete, giving a false impression of rapid progress. 
- In this case, it becomes very difficult for the project manager to determine the exact status of development and track the progress  of  the  project.
- This  usually  leads  to  a  problem  that  is  usually identified as the 99 per cent complete syndrome, when members feel that their work is 99 per cent complete even when their work is far from completion. 

## Classical Waterfall Model
- Classical waterfall model is intuitively the most obvious way to develop
software. 
- It is simple but completely theoritical.
- Not practical to use in decent software development projects.
- But we study this, since it is the base of all software development models.
- It has the following phases given in the diagram

<p align="center"><img src="Images/Screenshot 2025-05-10 205020.png" width="" height=""></p>

-  The phases starting from the feasibility study to the integration and system testing phase are  known  as  the **development phases**. It takes 40% effort.
- The **maintenance phase** takes 60% effort.
- An  activity  that  spans  all  phases  of  software  development  is **project management**. Since it spans the entire project duration, no specific phase is named after it
- The effort distribution graph given below

<p align="center"><img src="Images/Screenshot 2025-05-10 205756.png" width="" height=""></p>

### 1.Feasibility Study
- The main focus of the feasibility study stage is to determine whether it
would be **financially** and **technically feasible** to develop the software.
- The following activities take place in this phase:
    1. Development of overall understanding of the problem
    2. Formulation  of  the  various  possible  strategies  for  solving  the problem
    3. Evaluation of solutions 

### 2.Requirements analysis and specification
- The  aim  of  the  requirements  analysis  and  specification  phase  is  to understand the exact requirements of the customer and to document them properly.
- This phase consist of 2 activities:
    1. **Requirements  gathering  and  analysis:**
        - First requirements are gathered from the customer and then the gathered requirements are analysed.
        - The goal of requirement analysis is to find the *incompleteness* and *inconsistencies* in the gathered requirements.
        - **Inconsistent requirement**  is  one  in  which some part of the requirement contradicts with some other part.    
        - **Incomplete requirement** is one in which some parts of the actual requirements have been omitted.
    2. **Requirement Specification:**
        - After the requirement gathering  and analysis  activities  are  complete,  the  identified  requirements  are documented. This  is  called  a **software requirements specification (SRS)**.

**Software Requirements Specification(SRS)**
- It is a document which specifies the entire requirement of the software and acts like a contract between the development team and the customer.
- Any future disputes between the customer and the development teamis settled down by examining the SRS document.
- The SRS document is written using **end-user terminology**. This  makes  the  SRS  document  understandable  to the  customer.
- The SRS document not only forms the basis for carrying out all the development activities, but several documents such as users’ manuals, system test plan, etc. are prepared directly  based  on  it. 
- The SRS document has the following specifications:
    1. Functional Requirements(What the software is supposed to do): error message on failure,input given by user,output given by software
    2. Non Functional Requirements(how well the software performs, not what it does): Performance of the system, manpower, effort 
    3. Implementation Details:Time Required
- The SRS document is given to the customer for verification .After customer approves ,it is taken for the next phase. Otherwise the SRS is modified.

### 3.Design
- The goal of the design phase is to transform the requirements specified in the SRS document into a structure that is suitable for implementation in some programming language.
- In technical terms, during the design phase the **software architecture** is derived from the SRS document.
- Two important design approaches are popularly used at present: procedural and object oriented
    1. **Procedural design approach:**
    - It consists of two important activities: structured analysis and structured design.
    - During  structured  analysis, the functional requirements specified in the SRS document are decomposed into subfunctions and the data-flow among these  subfunctions  is  analysed  and  represented  diagrammatically in  the form  of  DFDs.
    - In Structured design the results of structured analysis are transformed into the software design.
    - Structured design consists of two main activities—architectural design (also called high-level design ) and detailed design (also called Low-level design ).
    - **High-level  design**  involves  decomposing  the  system  into modules,  and representing  the  interfaces  and  the  invocation  relationships  among  the modules. This is also known as software architecture.
    - During the detailed design activity, internals of  the individual  modules  such  as  the  data  structures  and  algorithms  of  the modules are designed and documented.
    2. **Object-oriented design approach:**
    - In  this  technique,  various objects that occur in the problem domain and the solution domain are first identified and the different relationships that exist among these objects are identified to create the **object structure**.
    - The object structure is further refined to obtain the detailed design.
    - OOD is credited to have several benefits, such as lower development time and effort ,and better maintainability of the software.

### 4. Coding and Unit Testting
- In coding phase, each component of the design is implemented as a programme module.
- Then unit testing is performed on each module, which include designing test cases, testing, debugging  to fix problems, and management of test cases.

### 5. Integration and system testing
- Here at each step modules are integrated one by one and tested.This is known as **Integration testing**.
- Finally, when all the models have been successfully integrated and tested, the fully working system is obtained.**System testing** is carried out on this fully working system.
- System testing usually consists of three different kind of testing activities:
    1. **$\alpha$-testing:** testing is the system testing performed by the development team.
    2. **$\beta$-testing:** This is the system testing performed by a friendly  set  of customers.
    3. **Acceptance  testing:** After  the  software  has  been  delivered,  the customer performs system testing to determine whether to accept the delivered software or to reject it.
### 6. Maintenance
- The ratio of relative effort of developing a typical software product and the total effort spent on its maintenance is roughly 40:60.
- Maintenance is required in the following three types of situations:
    1. **Corrective maintenance:** This type of maintenance is carried out to correct  errors  that  were  not  discovered  during  the  product development phase.
    2. **Perfective maintenance:** This type of maintenance is carried out to improve  the  performance  of the  system,  or  to  enhance  the functionalities of the system based on customer’s requests.
    3. **Adaptive maintenance:** Adaptive maintenance is usually required for porting  the  software  to  work  in  a  new  environment.  For  example, porting  may  be  required  to  get  the  software  to  work  on  a  new computer platform or with a new operating system.
    