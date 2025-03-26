# DFD(Data Flow Diagrams)
- **Definition:** A DFD is a hierarchical graphical model of a system that shows the different
processing activities or functions that the system performs and the data interchange
among those functions.
- a DFD model only represents the data flow aspects and
does not show the sequence of execution of the different functions and the
conditions based on which a function may or may not be executed
-  In fact, it
completely ignores aspects such as control flow, the specific algorithms used
by the functions, etc

## Symbols used in DFD
<p align="center"><img src="Images/Screenshot 2025-03-17 102745.png" width="" height=""></p>

1. **External entity symbol:** The external entities are
essentially those physical entities external to the software system which
interact with the system by inputting data to the system or by consuming the
data produced by the system.Eg, humans users,external hardwares,software dependant on another software.
2. **Data flow symbol** 
3. **Data store symbol:** A data store symbol can represent either a data structure or a physical file on disk. 
4. **Output Symbol:** The output
symbol is used when a hard copy is produced.

## Important concepts associated with constructing DFD models

**Synchronous and asynchronous operations**
- If two bubbles are directly connected by a data flow arrow, then they are
synchronous. This means that they operate at t h e same speed. An
example of such an arrangement is shown in Figure 6.3(a).Here, the
`validate-number` bubble can start processing only after the `read-number` bubble has supplied data to it; and the `read-number` bubble
has to wait until the `validate-number` bubble has consumed its
data.
- Two functions are asynchronous  if two bubbles are connected through a data store, as in Figure
6.3(b) then the speed of operation of the bubbles are independent. 

<p align="center"><img src="Images/Screenshot 2025-03-17 105544.png" width="" height=""></p>

**Data dictionary**
- Every DFD model of a system must be accompanied by a data dictionary.
- **Def:** A data dictionary lists the purpose of all data items and the definition of all composite
data items in terms of their component data items.

##  DEVELOPING THE DFD MODEL OF A SYSTEM
- The DFD model of a problem consists of many of DFDs and a single data dictionary.
- Level 0 and Level 1
consist of only one DFD each.
-  Level 2 may contain up to 7 separate DFDs,
and level 3 up to 49 DFDs, and so on. 
- there is only a single data
dictionary for the entire DFD model. All the data names appearing in all DFDs
are populated in the data dictionary and the data dictionary contains the
definitions of all the data items.

**Context Diagram**
-  It represents the entire system as a single
bubble. The bubble in the context diagram is annotated with the name of the
software system being developed (usually a noun).

**Level 1 DFD**
- The level 1 DFD usually contains three to seven bubbles
- To develop the level 1 DFD, examine the 3-7 high-level functional
requirements in the SRS document
- If a system has more than seven high-level requirements identified in
the SRS document, in this case some of the related requirements have to be
combined and represented as a single bubble.
- If a system has less than three
high-level functional requirements, then some of the high-level requirements
need to be split into their subfunctions so that we have roughly about five to
seven bubbles represented on the diagram

**Balancing DFDs**
- The data that flow into or out of a bubble must match the data flow at the next level
of DFD. This is known as balancing a DFD.

<p align="center"><img src="Images/Screenshot 2025-03-26 200059.png" width="" height=""></p>

## Common mistakes in DFD
- Many beginners commit the mistake of drawing more than one bubble
in the context diagram. Context diagram should depict the system as a
single bubble.
- Many beginners create DFD models in which external entities
appearing at all levels of DFDs. All external entities interacting with the
system should be represented only in the context diagram. The
external entities should not appear in the DFDs at any other level.
- It is a common oversight to have either too few or too many bubbles in
a DFD. Only three to seven bubbles per diagram should be allowed.
This also means that each bubble in a DFD should be decomposed
three to seven bubbles in the next level.
- Many beginners leave the DFDs at the different levels of a DFD model
unbalanced
- A common mistake committed by many beginners while developing a
DFD model is attempting to represent control information in a DFD.It is important to realise that a DFD represents only data flow, and it does not
represent any control information.
