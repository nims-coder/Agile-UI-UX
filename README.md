## **Unit 1**

**Q1: Explain Manifesto for Agile Software Development in detail.**
**A:** The Manifesto for Agile Software Development is a document created by the Agile Alliance that outlines the key values behind the Agile philosophy to help development teams work more efficiently. It emphasizes valuing:
*   **Individuals and interactions** over processes and tools.
*   **Working software** over comprehensive documentation.
*   **Customer collaboration** over contract negotiation.
*   **Responding to change** over following a plan.

***Diagram Description (Page 12):***
*The slide shows a simple flowchart with four blue boxes, illustrating the four core values of the Agile Manifesto in sequence.*
**Page Number(s):** 12, 13

---

**Q2: Explain Principles of Agile Development (12 Principles).**
**A:** The 12 principles inspired by the Agile Manifesto differentiate agile practices from heavyweight processes. They are:
1.  Satisfy the customer through early and continuous delivery.
2.  Welcome changing requirements, even late in development.
3.  Deliver working software frequently.
4.  Business people and developers must work together daily.
5.  Build projects around motivated individuals, providing support and trust.
6.  Face-to-face conversation is the most efficient method of communication.
7.  Working software is the primary measure of progress.
8.  Promote sustainable development; maintain a constant pace indefinitely.
9.  Continuous attention to technical excellence and good design.
10. Simplicity—the art of maximizing the amount of work not done—is essential.
11. The best architectures, requirements, and designs emerge from self-organizing teams.
12. The team regularly reflects on how to become more effective and adjusts its behavior.

***Diagram Description (Page 20):***
*The slide displays a grid of 12 blue icons, each representing one of the 12 Agile Principles, such as "Customer Satisfaction," "Frequent Delivery," and "Self-sufficient Teams."*
**Page Number(s):** 20, 21, 22, 23, 24, 25, 26

---

**Q3: Explain Whole team, User stories, Iteration plan, Short Cycle, Release plan, Acceptance test, Pair Programming of Extreme Programming in detail.**
**A:**
*   **Whole Team:** An XP team includes customers, managers, and developers working closely together. The customer is a member of the team who defines and prioritizes features.
*   **User Stories:** Requirements are captured as user stories, which are short descriptions of functionality written on index cards. They are a planning tool used by the customer to schedule implementation based on priority and cost.
*   **Short Cycles:** XP projects deliver working software in short, fixed-length iterations, typically lasting two weeks.
*   **Iteration Plan:** For each two-week iteration, the customer selects a collection of user stories to be implemented, based on a budget (velocity) established by the developers.
*   **Release Plan:** A higher-level plan that maps out the next six or so iterations (about three months' worth of work). It consists of a prioritized collection of user stories selected by the customer.
*   **Acceptance Tests:** The details of user stories are captured as automated acceptance tests specified by the customer. These tests become the true requirements document for the project.
*   **Pair Programming:** All production code is written by two programmers working together at the same workstation. One drives (types), while the other observes, finds errors, and suggests improvements. Roles are switched frequently.

***Diagram Description (Page 28):***
*This diagram illustrates the cyclical nature of Extreme Programming. It starts with a "Spike" feeding into "Requirements" and "Stories." This leads to "Release Planning" and then into a repeating "Iteration" loop. Inside the loop, "Acceptance Test" occurs, which, upon customer approval, leads to a "Release" of small increments of software.*
**Page Number(s):** Whole team (29), User stories (30), Short Cycle (31), Iteration plan (32), Release plan (33), Acceptance test (34, 35), Pair Programming (36, 37)

---

**Q4: Explain TDD, Refactoring of Extreme Programming in detail.**
**A:**
*   **Test-Driven Development (TDD):** An iterative development process where test cases are created *before* the code is written. A developer first writes a failing unit test for a new piece of functionality. Then, they write just enough production code to make that test pass. Finally, they refactor the code. This cycle is repeated in very short intervals.
*   **Refactoring:** The practice of improving the internal structure of the code without changing its external behavior. XP teams refactor frequently (every hour or half hour) to reverse code degradation and keep the system clean, simple, and maintainable.

***Diagram Description (Page 38):***
*The slide shows the TDD cycle. An arrow points from a red circle labeled "1 Fail" to a green circle labeled "2 Pass." An arrow then points from "Pass" to a blue circle labeled "3 Refactor." Finally, an arrow from "Refactor" points back to "Fail," completing the cycle.*
**Page Number(s):** TDD (38, 39, 40, 72), Refactoring (53, 54, 83)

---

**Q5: Explain Open Workspace and Planning Game in detail.**
**A:**
*   **Open Workspace:** The entire team works together in an open room with workstations arranged to maximize communication. The walls are covered with status charts and diagrams. This "war room" environment facilitates intense communication and shared awareness.
*   **Planning Game:** This is the process that divides responsibility for planning. Business people (customers) decide how important a feature is (priority and value). Developers decide how much that feature will cost to implement (estimate). The developers provide a budget for each release and iteration, and the customers choose the stories that fit within that budget.
**Page Number(s):** Open Workspace (45, 46), Planning Game (47, 48)

---

**Q6: Explain Spiking, Splitting, and Velocity.**
**A:**
*   **Splitting:** Stories that are too large or too small are difficult to estimate accurately. Therefore, large stories are split into smaller pieces, and stories that are too small are merged with others to create a story of a more estimable size.
*   **Spike:** A short research activity or experiment undertaken by the team to gain knowledge, reduce uncertainty, or make a better decision, often related to estimating a difficult story.
*   **Velocity:** A key metric in XP that measures the sum of the estimates of the stories completed during an iteration. The measured velocity of the previous iteration is used to plan the next one.
**Page Number(s):** 61, 62, 63

---

**Q7: Explain Release Planning, Task Planning in detail.**
**A:**
*   **Release Planning:** The process where customers, given the team's velocity, choose the stories they want implemented for the first release (e.g., in the next 2-4 months). They select stories whose total cost fits within the team's projected velocity for that period. This plan can be adjusted as velocity becomes more accurate.
*   **Task Planning:** At the beginning of each iteration, developers break the selected stories down into smaller development tasks. Each developer then signs up for tasks based on their individual budget (how many task points they completed in the previous iteration). The goal is to get all tasks for the iteration assigned.
**Page Number(s):** Release Planning (64), Task Planning (67, 68, 69)

---

**Q8: Explain Test Isolation in detail.**
**A:** Test Isolation is the practice of testing individual components (e.g., classes) separately from their dependencies. Writing tests before code often exposes areas that should be decoupled. To achieve isolation, mock objects are used. Mock objects are simulated objects that mimic the behavior of real dependencies (like a database or a check printer). This allows a class to be tested to ensure it behaves as it should in isolation, without needing a fully functional environment.

***Diagram Description (Page 75 & 78):***
*Page 75 shows a "Coupled payroll model" where a `Payroll` class directly depends on concrete `CheckWriter`, `Employee`, and `EmployeeDatabase` classes. Page 78 shows a "Decoupled Payroll" model where the `Payroll` class now depends on abstract interfaces. `MockCheckWriter` and `MockEmployeeDatabase` objects are used by `PayrollTest` to test the `Payroll` class in isolation.*
**Page Number(s):** 75, 76, 77, 78, 79

---

**Q9: Define a “sprint” and “agile practices “ in agile development.**
**A:**
*   **Sprint:** The provided material primarily uses the term "iteration," which is a short, time-boxed period (e.g., two weeks) during which the team produces a working increment of software. This is functionally identical to a "sprint" in the Scrum framework.
*   **Agile Practices:** These are the effective methods and techniques that agile teams use to prevent unpredictability, errors, and wasted effort. They are the concrete activities derived from the agile values and principles, such as working in short cycles, writing user stories, pair programming, and TDD.

***Diagram Description (Page 5):***
*The diagram shows the agile development process as a cycle. An arrow flows from "Requirements" to "Design" to "Deploy." A circular arrow encompassing "Test," "Agile," and "Develop" shows the continuous, iterative nature of the development phase.*
**Page Number(s):** Sprint (conceptually covered as "Short Cycles" and "Iteration" on pages 31, 32), Agile Practices (10, 11, and throughout the unit)

## **Unit 2**

**Q1: Explain symptoms/Characteristics of Poor Design. OR Discuss Symptoms of Code smells.**
**A:** The symptoms of poor design (also called design smells) are indicators that the software is becoming difficult to maintain and change. The key symptoms are:
*   **Rigidity:** The system is difficult to change; a single change causes a cascade of dependent changes.
*   **Fragility:** A change in one part of the system causes it to break in other, conceptually unrelated parts.
*   **Immobility:** It is difficult to separate components from the system for reuse elsewhere.
*   **Viscosity:** It is easier to implement a "hack" than to make a change that preserves the integrity of the design.
*   **Needless Complexity:** The design contains elements that are not currently useful.
*   **Needless Repetition:** The same code structures are repeated instead of being unified under a single abstraction.
*   **Opacity:** The code is difficult to understand and not expressive.
**Page Number(s):** 89, 90, 91, 92, 93, 94, 95, 96, 97

---

**Q2: What is spike, splitting and velocity?**
**A:**
*   **Spike:** A short research activity or experiment undertaken by the team to gain knowledge, reduce uncertainty, or make a better decision, often related to estimating a difficult story.
*   **Splitting:** The process of breaking down large user stories into smaller, more manageable ones that are easier to estimate. Small stories can also be merged.
*   **Velocity:** A key metric that measures the sum of the estimates of the stories completed during an iteration. The measured velocity of the previous iteration is used to plan the next one.
**Page Number(s):** 61, 62, 63

---

**Q3: Write a detailed note on “SRP: The Single-Responsibility Principle with appropriate example.**
**A:** The Single-Responsibility Principle (SRP) states that a class should have only one reason to change, meaning it should have only a single responsibility. If a class has more than one responsibility, those responsibilities become coupled.
*   **Example:** A `Rectangle` class that contains both a method to calculate its area (`area()`) and a method to render it on a screen (`draw()`). This class has two responsibilities: computational geometry and graphical rendering. This violates SRP because a change in the GUI could force a change in the class, which might affect the computational geometry application that doesn't even use the GUI. The solution is to separate these responsibilities into two distinct classes.

***Diagram Description (Page 104 & 107):***
*Page 104 shows a UML diagram where a `Rectangle` class with `draw()` and `area()` methods is used by both a `Computational Geometry Application` and a `Graphical Application`. Page 107 shows the corrected design where the responsibilities are separated into a `GeometricRectangle` class (with `area()`) and a `Rectangle` class (with `draw()`).*
**Page Number(s):** 103, 104, 105, 106, 107, 108

---

**Q4: Write a detailed note on “OCP: The Open-Closed Principle” with appropriate example.**
**A:** The Open/Closed Principle (OCP) states that software entities should be open for extension but closed for modification. This means that you should be able to add new functionality without changing existing, working code. This is achieved through abstraction.
*   **Example:** A `Client` class directly depends on a concrete `Server` class. If you want the `Client` to use a different server, you must modify the `Client` class code. This design is not closed for modification. A better design, conforming to OCP, would have the `Client` depend on an abstract `ClientInterface`. New server types can then be created by implementing this interface, and the `Client` class never needs to change.

***Diagram Description (Page 118 & 119):***
*Page 118 shows a diagram labeled "Client is not open and closed," with a `Client` box pointing directly to a `Server` box. Page 119 shows the corrected "STRATEGY pattern," where the `Client` points to an `«interface» Client Interface`, and the `Server` class implements that interface.*
**Page Number(s):** 115, 116, 117, 118, 119

---

**Q5: Write a detailed note on “LSP: Liskov Substitution Principal” With appropriate example.**
**A:** The Liskov Substitution Principle (LSP) states that subtypes must be substitutable for their base types. This means that a child class object should be able to replace its parent class object without breaking the program or causing unexpected behavior. It ensures that an `IS-A` relationship is behaviorally sound.
*   **Example:** A `Square` "is-a" `Rectangle` in geometry, but making a `Square` class inherit from a `Rectangle` class can violate LSP. A user of a `Rectangle` object would assume they can set the width and height independently. However, if that `Rectangle` object is actually a `Square`, setting the width would also force the height to be the same, violating the user's reasonable assumption about the base class's behavior.

***Diagram Description (Page 123):***
*A simple UML inheritance diagram shows a `Square` class with an arrow pointing up to a `Rectangle` class, indicating that `Square` inherits from `Rectangle`.*
**Page Number(s):** 121, 122, 123, 124, 125, 126

---

**Q6: Write a detailed note on DIP: Dependency inversion principle With appropriate example.**
**A:** The Dependency-Inversion Principle (DIP) states that:
1.  High-level modules should not depend on low-level modules. Both should depend on abstractions.
2.  Abstractions should not depend upon details. Details should depend upon abstractions.
This inverts the traditional dependency flow where high-level policy depends on low-level implementation.
*   **Example:** A high-level `Policy` layer should not directly depend on a low-level `Mechanism` layer. Instead, the `Policy` layer should define an abstract interface for the services it needs. The `Mechanism` layer then implements this interface. This way, the high-level policy does not depend on the low-level detail; instead, the detail depends on the abstraction defined by the high-level policy.

***Diagram Description (Page 129 & 130):***
*Page 129 shows a "Naive layering scheme" where a `Policy Layer` box points to a `Mechanism Layer`, which points to a `Utility Layer`. Page 130 shows the corrected design where a `Button` (high-level) depends on a `ButtonServer` interface, which is implemented by the `Lamp` (low-level) class.*
**Page Number(s):** 128, 129, 130, 131

---

**Q7: Write a detailed note on ISP: The Interface-Segregation Principle. With appropriate example.**
**A:** The Interface-Segregation Principle (ISP) states that clients should not be forced to depend on methods they do not use. It advocates for breaking down large, "fat" interfaces into smaller, more specific, client-focused interfaces. This prevents clients from being coupled to changes in methods they don't even use.
*   **Example:** A system where a `TimedDoor` needs to be notified by a `Timer`. A common but flawed solution is to make the base `Door` class inherit from a `TimerClient` interface. This forces *all* types of doors (even those that don't need timing) to depend on `TimerClient` and provide an implementation for its methods. This is a "fat" interface.

***Diagram Description (Page 138):***
*The UML diagram shows the flawed hierarchy. A `TimedDoor` class inherits from `Door`, which in turn inherits from the `«interface» TimerClient`. This forces the general `Door` abstraction to depend on the specific `TimerClient` interface.*
**Page Number(s):** 133, 134, 135, 136, 137, 138, 139

## **Unit 3**

**Q1: Explain UX, UX Design and its importance as well as components of UX and also explain the importance of “Usefulness” and “Emotional impact” in UX design.**
**A:**
*   **UX (User Experience):** The totality of the effects felt by a user before, during, and after interaction with a product or system.
*   **UX Design:** The process of designing that interaction to create a user experience that is productive, fulfilling, satisfying, and even joyful.
*   **Components of UX:** Usability, Usefulness, Emotional Impact, and Meaningfulness.
*   **Importance of Usefulness:** This is the ability to use the system to accomplish work goals. It is crucial because if a product isn't useful, other aspects don't matter.
*   **Importance of Emotional Impact:** This is the affective component of UX, including the user's feelings and satisfaction. It is important because positive emotions can lead to greater user loyalty and engagement.

***Diagram Description (Page 144):***
*A large box labeled "User Experience" is shown to be equal to four stacked blue boxes labeled "Usability," "Usefulness," "Emotional Impact," and "Meaningfulness," each with a brief description.*
**Page Number(s):** 143, 144

---

**Q2: Describe the wheel: UX Processes, Lifecycles, methods and techniques.**
**A:** "The Wheel" is a model representing the UX design lifecycle as an iterative process. It consists of four main activities that form a continuous cycle:
1.  **Understand Needs:** Researching users, their work, and the context to gather data.
2.  **Design Solutions:** Creating design concepts to address the identified needs.
3.  **Prototype Candidates:** Realizing promising design ideas in a tangible form.
4.  **Evaluate UX:** Verifying and refining the prototypes with users to get feedback.
The "wheel" analogy emphasizes that the process is not linear; with each rotation (iteration), the design gets closer to the desired destination. Dotted arrows show that one can "move back to previous development activity" from any stage.

***Diagram Description (Page 149):***
*The slide shows four blue boxes—"Understand user work and needs," "Create design concepts," "Realize design alternatives," and "Verify and refine designs"—arranged in a circle with solid arrows. Dotted arrows show iterative loops within and between these stages.*
**Page Number(s):** 148, 149

---

**Q3: Discuss the significance of Prototyping as a UX lifecycle activity. What is a “clickthrough prototype”?**
**A:** Prototyping is a full-fledged activity to realize and envision design candidates. Its significance lies in its ability to:
*   Provide a tangible platform for evaluation with users.
*   Create a concrete baseline for communication.
*   Allow users to "take the design for a spin."
*   Encourage early user participation and feedback.
*   A **"click-through prototype"** (also called a click-through wireframe prototype) is a prototype that links individual screens or wireframes together, allowing a user to click on buttons and links to navigate through a workflow, simulating the flow of the final application.
**Page Number(s):** 158

---

**Q4: List all UX design techniques which are used as life skills.**
**A:** The UX design techniques listed as life skills include: Observation, Abstraction, Note Taking, Data/Idea Organization, Modeling, Storytelling, Immersion, Brainstorming, Sketching and Drawing, Framing and Reframing, Reasoning and Deduction, Prototyping and Envisioning, Critical Thinking, and Iteration.
**Page Number(s):** 160, 161, 162, 163, 164

---

**Q5: What is meant by “Scope” and “Rigor” of a project? Briefly discuss the factors that influence Rigor during agile project development. Explain scope of delivery in UX process and what the challenges are in building systems.**
**A:**
*   **Scope:** Refers to how the target system is "chunked" for delivery in each iteration.
*   **Rigor:** The degree of formality, thoroughness, precision, and accuracy applied to a UX method or process. The need for rigor is influenced by **Interaction Complexity** and **Domain Complexity**.
*   **Scope of Delivery:** Explained with a house analogy: **large scope** is building the whole house at once; **small scope** is delivering it one room at a time.
*   **Challenges in Building Systems:** The primary challenges are that **change always happens** and there is often a **gap between the reality and the designer's understanding**.

***Diagram Description (Page 172):***
*A 2x2 matrix is shown. The Y-axis is "Interaction complexity" (Low to High), and the X-axis is "Work domain complexity" (Low to High). An arrow labeled "Increasing risk and increasing level of rigor needed" points diagonally from the bottom-left quadrant (Simple/Simple) to the top-right quadrant (Complex/Complex).*
**Page Number(s):** Rigor (167, 169, 170, 172), Scope (173, 174), Challenges (175, 176, 177)

---

**Q6: With the help of a neat diagram, discuss the Funnel Model of Agile.**
**A:** The Funnel Model of Agile UX is a way to envision UX activities in an agile context.
*   **Early Funnel:** This phase happens before syncing with development. It has a larger scope and focuses on overall conceptual design and research.
*   **Late Funnel:** This phase syncs with development sprints. The scope is narrowed, and UX delivers detailed designs for individual features ("chunks") just-in-time for the corresponding SE sprints.

***Diagram Description (Page 181):***
*The diagram shows a large funnel shape on its side. The wide mouth on the left is labeled "Early funnel" and "Possibly larger scope on the UX side." The funnel narrows into a long, straight tube on the right, which is segmented and labeled "Agile sprints" and "Late funnel." This visually represents the scope narrowing from broad design exploration to focused, iterative development.*
**Page Number(s):** 179, 181, 182

---

**Q7: What is agile lifecycle process? Explain syncing agile UX with agile SE sprints.**
**A:** An agile lifecycle process is a small-scope approach where all lifecycle activities are performed for one feature, and then the lifecycle is repeated for the next feature.
*   **Syncing agile UX with agile SE sprints:** This is the process of coordinating the UX and Software Engineering (SE) teams. The UX team provides a "design chunk" for a feature to the SE team. The SE team then implements that design in its development sprint.

***Diagram Description (Page 183):***
*A flowchart shows two parallel streams. The top stream, "UX flow," shows "UX design 1" feeding into "UX design 2." The bottom stream, "SE flow," shows "SE sprint 1" feeding into "SE sprint 2." An arrow from "UX design 1" points down to "SE sprint 1," showing that the UX design (as a "UX specification") is the input for the corresponding development sprint.*
**Page Number(s):** 178, 183

## **Unit 4**

**Q1: What is design? Explain the purpose of design in detail. Explain why a UX Design team should have people with diverse skills and backgrounds. Briefly discuss a real-world example where such a team can have a positive impact on the design of a product.**
**A:**
*   **What is Design:** Design is both a noun (the plan or concept for a product) and a verb (the act of creating something that did not exist before). Its purpose is to create solutions for known problems or to find problems for innovative solutions.
*   **Why a Diverse Team:** A UX team needs diverse skills and backgrounds because UX is the "sum total of all the effects felt by the user." A team with varied expertise can better address the many facets of the user experience.
*   **Example:** When designing a mobile banking app, a diverse team is crucial. Technologists ensure it's feasible, financial experts ensure compliance, graphic designers create an appealing interface, and psychologists can provide insight into user trust and security fears, leading to a more successful product.

***Diagram Description (Page 189):***
*A flowchart branches from the word "Design." One branch goes to "Act of creation (verb)," which "Results in" the other branch, "Plan or structure of product (noun)." This illustrates the dual nature of the word design.*
**Page Number(s):** 187, 188, 189

---

**Q2: Discuss and compare the Top-Down and Bottom-up approaches for design using suitable examples.**
**A:**
*   **Bottom-Up Design:** This approach starts with the details of an existing work practice. The design is then built up to support and improve this known behavior. It is less likely to lead to major innovation.
*   **Top-Down Design:** This approach starts with an abstract, high-level goal. The goal is to create the best possible design solution to support the fundamental nature of the work, irrespective of current practices. It is more likely to be innovative.
*   **Example (Voting):** A **bottom-up** approach to a new voting system would focus on improving the existing physical voting booth. A **top-down** approach would rethink the entire act of voting, leading to potentially innovative solutions like a secure smartphone app.
**Page Number(s):** 190, 191, 192, 193, 194, 195, 196, 197, 198, 199

---

**Q3: Explain Generative Design in detail. Also, Discuss the following concepts with respect to Generative design: a. Ideation b. Sketching c. critiquing**
**A:** Generative Design is an approach to design creation that involves an intertwined and iterative loop of three main activities to explore a design idea. The activities are:
*   **a. Ideation:** The cognitive activity where diverse and innovative design ideas are spawned or created.
*   **b. Sketching:** The externalization activity that captures these ideas in concrete, rapid, freehand visual representations.
*   **c. Critiquing:** The analysis activity used to evaluate the emergent ideas from sketching and ideation, identify tradeoffs, and inform the next steps.

***Diagram Description (Page 202):***
*A circular flow diagram shows the generative design process. "Ideation" spawns "Ideas," which are "Articulated in" "Sketching." This externalizes the ideas, which can then trigger "More ideation and sketching." The results are then subject to "Critiquing," which leads to "Variations and alternative ideas" and "Refined ideas" that feed back into the "Ideation" step.*
**Page Number(s):** 200, 202, 203, 204, 210

---

**Q4: What is prototyping and what are the advantages of it? What are the different types of prototypes that can be built for UX design?**
**A:**
*   **Prototyping:** The creation of a preliminary, tangible representation of a design idea. A prototype is in some way less than a full implementation, allowing it to be created and changed quickly.
*   **Advantages:** They provide a platform for user evaluation, offer a concrete basis for communication, encourage early user participation, and help sell ideas to stakeholders.
*   **Types of Prototypes:**
    *   **Horizontal Prototype:** Broad in features but shallow in detail.
    *   **Vertical Prototype:** Narrow in features but with deep, functional detail.
    *   **Local Prototype:** Narrow in both breadth and depth, for a specific design issue.
    *   **“T” Prototype:** A hybrid of horizontal and vertical prototypes.
    *   **Wireframe Prototype:** A two-dimensional sketch of a single screen.

***Diagram Description (Page 222):***
*A large rectangle represents the "Full system." A wide, shallow rectangle at the top represents a "Horizontal prototype." A narrow, deep rectangle represents a "Vertical prototype." A small square represents a "Local prototype." This diagram clearly shows how each prototype type is a "slice" of the full system.*
**Page Number(s):** Advantages (219, 220), Types (221, 222, 223, 224, 225, 226, 227)```
93.1s
