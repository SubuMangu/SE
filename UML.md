# UML
- UML (Unified Modeling Language) is like a blueprint for building software. It helps developers, designers, and even non-technical people visualize, plan, and understand how a software system will work before it's actually built — just like architects use building plans before constructing a house.
- If a single model is made to capture all the required perspectives, then it would be as
complex as the original problem, and would be of little use.
- Hence, we divide uml diagrams to capture the following things:
    1. User’s view
    2. Structural view
    3. Behaviourial view
    4. Implementation view
    5. Environmental view
## Different Types of UML Diagrams
<p align="center"><img src="Images/Screenshot 2025-05-05 111759.png" width="" height=""></p>

## Class Diagrams
- A class diagram describes the static structure of a system.
- It shows how a system is structured rather than how it behaves.
- The main constituents of a class diagram are classes and their  relationships—generalisation,  aggregation,  association,  and various  kinds  of  dependencies.

**Classes**
- Classes  are  represented  as  solid  outline  rectangles  with compartments.
- The class name is usually written using mixed case convention and begins with an uppercase (e.g. LibraryMember). Object names on the other hand, are written using a mixed  case  convention,  but  starts  with  a  small  case  letter  (e.g., studentMember)
- Class  names  are  usually  chosen  to  be  singular
nouns.
- Classes can have optional attributes and operation compatments.

<p align="center"><img src="Images/Screenshot 2025-05-05 113759.png" width="" height=""></p>

**Association**
- An arrowhead may be placed on the association  line  to  indicate  the  reading  direction  of  the  association. 
- On each side of the association relation, the multiplicity is noted as an individual number or as a value range. The multiplicity indicates how many instances of one class are associated with the other.
- Value ranges of multiplicity are noted by specifying the minimum and maximum value, separated by two dots, e.g. 1..5. 
- An asterisk is used as a wild card and means many (zero or more). The association of Figure 7.24 should  be  read  as  “Many  books  may  be  borrowed  by  a  LibraryMember”.Usually, associations (and links) appear as verbs in the problem statement.

<p align="center"><img src="Images/Screenshot 2025-05-05 121959.png" width="" height=""></p>

**Aggregation**
- Aggregation is a special type of association relation where the involved classes  are  not  only  associated  to  each  other,  but  a  whole-part relationship  exists  between  them.
-  An example of aggregation, a book register is an aggregation of book objects. Books can be added to the register and deleted as and when required.
-  Observe that the number 1 is annotated at the diamond end, and a * is annotated at the other end. This means that one document can have many paragraphs.
-  On the other hand, if we wanted
to indicate that a document consists of exactly 10 paragraphs, then we would
have written number 10 in place of the (*).

<p align="center"><img src="Images/Screenshot 2025-05-05 123635.png" width="" height=""></p>

- The aggregation relationship cannot be reflexive (i.e. recursive). That is, an object  cannot  contain  objects  of  the  same  class  as  itself.
- Also,  the aggregation relation is not symmetric. That is, two classes A and B cannot contain instances of each other
- However, the aggregation relationship  can be transitive. 

**Composition**
- Stricter form of aggregation
- When the whole is created, the parts are
created and when the whole is destroyed, the parts are destroyed.
- As an example, consider the example of an order consisting many order items. If the order once placed, the items cannot be changed at all. In this case, the order is a composition of order items. However, if order items can be changed (added, delete, and modified) after the order has been placed, then aggregation relation can be used to model it.

**Inheritance**
- The inheritance relationship is represented by means of an empty arrow pointing from the subclass to the superclass.
- Alternatively, when there are many subclasses of a base class, the inheritance arrow from the subclasses may be combined to a single line (see Figure 7.27) and is labelled with the aspect of the class that is abstracted.

<p align="center"><img src="Images/Screenshot 2025-05-05 124605.png" width="" height=""></p>

**Dependency**
- Represented by dotted line

<p align="center"><img src="Images/Screenshot 2025-05-05 212054.png" width="" height=""></p>

**Constraints**
- A constraint describes a condition or an integrity rule. 
- For  example,  to  denote  that  the  books  in  a library are sorted on ISBN number we can annotate the book class with the constraint {sorted}.
- UML  allows  you  to  use  any free  form  expression  to  describe
constraints.  The  only rule  is  that  they  are  to  be  enclosed  within  braces {}.
-  However,  UML  also
provides **object constraint language (OCL)** to specify constraints. In OCL the
constraints are specified a semi-formal  language,  and  therefore  it is more
amenable to automatic processing as compared to the informal constraints
enclosed within {}. 

<p align="center"><img src="Images/Screenshot 2025-05-05 125543.png" width="" height=""></p>

## Object Diagrams
<p align="center"><img src="Images/Screenshot 2025-05-05 125819.png" width="" height=""></p>

## Interaction Diagrams
- Interaction diagrams, as their name itself implies, are models that describe how groups of objects interact among themselves through message passing to realise some behaviour.
- It is of 2 types: Sequence Diagram and Collaboration Diagram

### Sequence Diagram
- Inside the box the name of the object is written with a colon separating it from the name of the class and both the name of the object and the class are underlined. This signifies that we are referring any arbitrary instance of the class. For example, in Figure 7.30 :Book represents any arbitrary instance of the Book class.
- A  rectangle  called  the activation  symbol is drawn on the lifeline of an object to indicate the points of time at which the object is active. 
- Two important types of control information
are:
1. A condition (e.g., [invalid]) indicates that a message is sent, only if the condition is true.
2. An iteration marker(*) shows that the message is sent many times to multiple receiver objects as would happen when you are iterating over a collection or the elements of an array. You can also indicate the basis of the iteration, e.g., [for every book object].

<p align="center"><img src="Images/Screenshot 2025-05-05 174833.png" width="" height=""></p>

### Collaboration Diagram
<p align="center"><img src="Images/Screenshot 2025-05-05 175352.png" width="" height=""></p>

## Activity Diagram
- Activity  diagrams  are  similar  to  the  procedural  flow  charts.  The  main difference is that activity diagrams support description of parallel activities and synchronisation aspects involved in different activities.
- Parallel activities are represented on  an  activity  diagram  by  using swim lanes. Swim lanes enable you to group activities based on who is performing them, e.g., academic department vs. hostel office. Thus swim lanes subdivide activities based on the responsibilities of some components.

<p align="center"><img src="Images/Screenshot 2025-05-05 180549.png" width="" height=""></p>

## State Chart Diagram
- A state chart diagram is normally used to model how the state of an object  changes  in  its  life  time. 
- State  chart  diagrams  are  based  on  the finite  state  machine (FSM) formalism. An FSM consists of a finite number of states corresponding to those  of  the  object  being  modelled.
- The basic elements of the state chart diagram are as follows:
1. **Initial state:** This represented as a filled circle.
2. **Final state:** This is represented by a filled circle inside a larger circle.
3. **State:** These are represented by rectangles with rounded corners.
4. **Transition:** A transition is shown as an arrow between two states.The  syntax  for  the  label  of  the  transition  is  shown  in  3  parts— [guard]event/action

<p align="center"><img src="Images/Screenshot 2025-05-05 193105.png" width="" height=""></p>