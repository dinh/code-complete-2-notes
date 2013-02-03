Notes and reflections on Code Complete, Second Edition
=====================================================

## 3: Upstream prerequisites
### 3.1 Importance of prerequisites
1. Software can not overcome plan flaws (“Can’t design a Pontiac and get a Rolls Royce”).
1. Quality at beginning (design), middle (construction) and end (testing) of process.
1. Planning as a form of risk reduction: The most common risks are poor planning.

1. Common reasons for poor planning: 
  1. Inexperienced or untrained developers.
  1. Unenlightened boss wants to see developers coding, because *planning isn’t work*. Good counter-arguments: 
    * Simple logic - planning saves time, reduces risks, helps estimate costs
    * Analogy to non-software projects
    * Coordination between developers (UI waiting for BE on so on)
    * Hard data (page 29): The cost of fixing an error grows (exponentially?) over time.

#### My thoughts
Huge open-source projects, most notably the Kernel, are not planned, at least not in the usual architect-designer-developer flow.


### 3.2 Determine the kind of software You’re working on (pp. 31)
The development approach is derived from the type of software used. An internet site is fault-tolerant and has frequent spec changes. A pace maker can not tolerate faults, and its spec never changes. Therefore, an internet site should be developed iteratively, while a pacemaker should be developed sequentially.

Combining iterative design with prerequisites is very effective.

#### My thoughts
Prerequisites are interfaces: Between customer and code, and between code components.

### 3.3 Problem-definition prerequisite (pp. 36)
A "clear statement of the *problem*" is the first step. It should not be stated in software terms (unless it's a software project like a compiler), but in the client's terms, e.g. *"We don't know where are all the company's vehicles during the day."*. Note that the problem can sometimes be solved without a software. Without a clear problem, the entire development process might be wasted on irrelevant issues.

### 3.4 Requirements prerequisite (pp. 38)
The requirements are still phrased in the user, rather than the developer, language: *"The vehicles' location should be updated every 5 minutes."*

The requirements are seldom frozen. Therefore, a change mechanism should be agreed on with the client before the development process begins, with a clear price and time tags for each requested change.

#### My thoughts
The requirement checklist is the important part of the section.

### 3.5 Architecture prerequisite (pp. 43)
Architecture: "The high level part of software design."


