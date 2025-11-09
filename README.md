## Software Testing Study Notes

### Important terms

**SDLC** - software development lifecycle.

#### Importance of SW Testing

1. Ensuring Quality and Reliability
   Throughly tested software ➡️ saves time and money.

2. Improving User Experience(UX)
   To create software that is easy to navigate and use.

3. Strong Security
   To find vulnerabilities in the software.

4. Ensuring Regulatory Requirements
   To ensure that software follows safety and security standards.

**Integration testing** - how well different components work together;
**System testing** - if a software includes all requirements;
**End-to-end Testing** - makes sure that everything works as intended;
**Performance testing** - if a system manages different levels of usage;
**Security testing** - if there are any potential vulnerabilities.

**Software systems**

**Multiple interconnected components:** Many parts that depend on each other(payment system, inventory system).

**Diverse technologies:** Uses different languages, tools, frameworks or platforms.

**Complex integrations:** Parts must work together across systems or services(API, db, cloud platforms - third-party).

#### Testing Stretegies

**Test automation:** Using tools/scripts to run tests automatically instead of manually.

✔️ Advantages:
Faster testing;
Fewer human errors;
Repeatable and reliable;
Saves time and cost;

➖ Drawbacks of test automation:
High initial setup cost
Maintenance effort when tests break
Not suitable for all tests (e.g., exploratory testing)

**Risk-based testing:**
A testing approach that prioritizes testing based on the risk and impact of potential failures, focusing more on high-risk areas first.

**Strategic resource allocation** - optimization of tool use, training programs for testers.

**Continuous monitoring and feedback**

#### Software Rewuirements in context of Testing

**BDD** (Behavior-Driven Development) -
A development approach where software behavior is defined in plain language (**Given-When-Then**) before coding.

Why it’s needed:
🔸Improves communication between developers,testers, and business;
🔸Ensures software meets user expectations;
🔸Reduces misunderstandings and defects;

**User story:**
A short, simple description of a feature from the user’s perspective.

It must be:
🔹Clear and simple;
🔹User-focused;
🔹Testable;
🔹Small and achievable;
🔹Has acceptance criteria;

✔️ Why testers need it:
✔️ Understand user needs and expectations;
✔️ Create relevant test cases;
✔️ Validate real user behavior;

**RTM** (Requirement Traceability Matrix):
A document that maps requirements to their corresponding test cases in software testing.

Why it’s important:
Ensures all requirements are tested
Helps track test coverage
Identifies missing or untested requirements
Aids in impact analysis when requirements change

**Agile** can be challenging for testers:

🌱 **Frequent changes:** Requirements evolve rapidly, making tests quickly outdated(**test case rework**);
🌱 **Short iterations:** Less time for thorough testing(**maintaining traceability** - if all changes reflect test cases);
🌱 **Continuous integration:** Tests must be automated and fast;
🌱 **Collaboration demands:** Testers must work closely with developers and stakeholders constantly;
