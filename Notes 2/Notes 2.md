# Other Software Development Models
## Shortcomings of the classical waterfall model
1. **No feedback paths:** 
    - The classical waterfall model is idealistic in the sense that it assumes that no error is ever committed by the developers during any of the life cycle phases, and therefore, incorporates no mechanism for error correction.
2. **Difficult to accommodate change requests:**
    - This model assumes that all customer  requirements  can  be  completely  and  correctly  defined  at  the beginning  of  the  project.
    - The customers requirements usually keep on changing with time.
3. **Inefficient error corrections:**  
    - Errors or bugs (in design or code) are often discovered very late in the process—during the testing phase.
    - But in this model, there is no scope to backtrack ,if any error is occurred.
4. **No overlapping of phases:** 
    - This  model recommends that the phases be carried out sequentially—new phase can start only after  the  previous  one completes.
    - But in reality some phases need to overlap

### When is classical waterfall model used?
- Even though, while actually developing a software, we don't strictly follow the classical waterfall model. 
- But, as suggested by Parnas [1972] the final documents for the product  should  be  written  as  if  the  product  was  developed  using  a  pure classical waterfall for simplicity.
- Just imagine, A mathematician presents a proof as a single chain of deductions, even though the proof might have come from a convoluted set of partial attempts, blind alleys and backtracks. Imagine how difficult it would be to understand, if a mathematician presents a proof by retaining all the backtracking, mistake corrections, and solution refinements he made while working out the proof.

## Iterative Waterfall Model
- The  main  change  brought about  by  the  iterative  waterfall  model  to the  classical waterfall model is in the form of providing feedback paths from every phase to its preceding phases.

<p align="center"><img src="Images/Screenshot 2025-05-11 183755.png" width="" height=""></p>

- Almost every life cycle model that we discuss are iterative in nature, except the  classical  waterfall  model  and  the  V-model—which are  sequential  in nature.

### Phase containment of errors
- The principle of detecting errors as close to thier point of commitment is called **phase contentment of error**.
- For example, if a design problem is detected in the design phase itself, then the problem can be taken care of much more easily than if the error is identified, say, at the end of the testing phase. 
- It is done by rigorously reviewing the documents produced at the end of each phase.

### Phase Overlap
- There are two reasons for phase overlapping.
    1. In spite of the best effort to detect errors in the same phase in which they are committed, some errors escape detection and are detected in a later phase.
    2. Some members may complete their part of the work earlier than other members. If strict phase  transitions  are  maintained,  then  the  team members who complete their work early would  idle waiting  for  the phase to be complete, and are said to be in a blocking state.

### Shortcomings of Iterative Waterfall Model
1. **Incremental delivery not supported:** In the iterative waterfall model, the full software is completely developed and tested before it is delivered to the customer. There is no provision for any intermediate deliveries to occur.  By  the  time  the software is delivered, installed, and becomes ready for use, the customer’s business  process  might  have  changed  substantially.  This  makes  the developed application a poor fit to the customer’s requirements.
2. **Phase  overlap  not  supported:**  For  most  real  life  projects,  it becomes difficult to follow the rigid phase sequence prescribed by the waterfall model. By the term a rigid phase sequence, we mean that a phase can start only after the previous phase is complete in all respects. As already discussed, strict adherence to the waterfall model creates blocking states. 
3. **Error  correction  unduly  expensive:**  In  waterfall  model,  validation  is delayed  till  the  complete  development  of  the  software.  As  a  result,  the defects that are noticed at the time of validation incur expensive rework and result in cost escalation and delayed delivery.
4. **Limited customer interactions:** This model supports very limited customer interactions.As a result, the developed software usually turns out to be a misfit to the customer’s actual requirements.  
5. **No support for risk handling and code reuse:** It becomes difficult to use the waterfall model in projects that are susceptible to various types of risks, or those involving significant reuse of existing development artifacts. 

## Agile Models
- Suitable for designing small service based products.
- The agile model was primarily designed to help a project to adapt to change requests quickly.
- In the  agile  model,  the  requirements  are  decomposed  into  many  small parts  that  can  be  incrementally developed.
- The  agile  model  adopts  an iterative approach. Each incremental part is developed over an iteration.Each iteration is intended to be small and easily manageable and lasting for a couple of weeks only.
- The time to complete an iteration is called a **time box**.
- A central principle of the agile model is the delivery of an increment to the customer after each time box.
- Agile development projects usually deploy **pair programming**.
- In pair programming, two programmers work together at one work station. One types in code while the other reviews the code as it is typed in. The two  programmers switch their roles every hour or so.

- There are several types of Agile Models: Crystal,Atern,Scrum,Kanban,XP