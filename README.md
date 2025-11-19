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

Why it’s needed:<br>
🔸Improves communication between developers,testers, and business;<br>
🔸Ensures software meets user expectations;<br>
🔸Reduces misunderstandings and defects;

**User story:**
A short, simple description of a feature from the user’s perspective.

It must be:<br>
🔹Clear and simple;<br>
🔹User-focused;<br>
🔹Testable;<br>
🔹Small and achievable;<br>
🔹Has acceptance criteria;<br>

Why testers need it:<br>
✔️ Understand user needs and expectations;<br>
✔️ Create relevant test cases;<br>
✔️ Validate real user behavior;<br>

**RTM** (Requirement Traceability Matrix):
A document that maps requirements to their corresponding test cases in software testing.

Why it’s important:
Ensures all requirements are tested
Helps track test coverage
Identifies missing or untested requirements
Aids in impact analysis when requirements change

**Agile** can be challenging for testers:

🌱 **Frequent changes:** Requirements evolve rapidly, making tests quickly outdated(**test case rework**);<br>
🌱 **Short iterations:** Less time for thorough testing(**maintaining traceability** - if all changes reflect test cases);<br>
🌱 **Continuous integration:** Tests must be automated and fast;<br>
🌱 **Collaboration demands:** Testers must work closely with developers and stakeholders constantly;

**CI/CD in DevOps**

**Continuous Integration (CI):** Automatically building and testing code every time changes are made, to catch issues early.

**Continuous Deployment (CD):** Automatically deploying tested code to production or staging, ensuring rapid delivery of updates.

**Shift-left testing:**
Testing earlier( during the design and development
phases) in the development cycle (instead of at the end) in CI/CD pipelines ➡️ reduces cost, effort, improves sw quality.

Purpose:<br>
🍀Catch defects sooner;<br>
🍀Reduce cost and effort of fixing bugs;<br>
🍀Improve software quality and delivery speed;<br>

**Manual testing**(preferred for exploratory and usability scenarios) are not for DevOps workflow. **Test automation** is more usable(tools like **Selenium**, **JUnit**, **Cypress**).

**Fast feedback loop** is crucial for Agile and DevOps methodologies(real-time reporting, clear communication, test result analysis).

**Parallel testing:**
Running multiple tests at the same time on different environments, browsers, or data sets.

Purpose:
Speeds up testing
Saves time compared to sequential testing
Helps ensure consistency across platforms

New technologies such as the Internet of Things (IoT), AI, and cloud computing require testers to develop new approaches and strategies to ensure software reliability, scalability, and security.

Testing AI requires the focus on:

**Fairness:** Ensuring the AI does not produce biased or discriminatory results for different users or data groups.

**Explainability:** Verifying that AI decisions can be understood, interpreted, and justified.

**Robustness:** Checking that the AI behaves correctly under unexpected, noisy, or edge-case inputs.

IoT in the context of testing requires(network, hardware, swintegrations):

device interoperability, network stability, data integrity, real-time responsiveness, and attention to security vulnerabilities.

Cloud Computing(must be scalable, secure, resilient):

**Scalability testing:** Verifies that cloud applications can handle increasing users or workloads by scaling resources up or down.

**Resilience testing:** Ensures the system continues to work or recovers quickly when cloud components fail.

Testers should adopt tools for testing:

<ins>AI</ins> - TensorFlow Model Analysis, Fairlearn;

<ins>IoT</ins> - WS IoT Device Tester, IoTIFY;

<ins>cloud testing </ins> - Apache JMeter, Locust, Chaos Monkey;

Test Data Management Solutions:

**Data masking:** Hides sensitive data while keeping it usable for testing.

**Synthetic data generation:** Creates artificial test data that mimics real data.

**Data virtualization:** Provides access to test data without copying or moving it.

#### Cybersecurity and Software Testing

In software testing, the following are required:

**Security testing:** Ensures the system protects data and prevents unauthorized access.

**Penetration testing:** Simulates real attacks to find exploitable weaknesses.

**Vulnerability scanning:** Automatically detects known security flaws in the system.

The biggest challenge for testers to balance security and usability.

Security testing tools: OWASP ZAP, Burp Suite, Nessus.

#### Trends in Software Testing(2026)

**🔘 AI-Powered Test Automation:** Uses AI/ML to create, execute, and maintain tests more efficiently.

**🔘 Shift-Left Testing:** Starts testing early in the development lifecycle to find defects sooner.

**🔘 DevOps and Continuous Testing:** Integrates testing continuously into CI/CD pipelines.

**🔘 Cloud-Based Testing Environment:** Uses cloud infrastructure to test at scale and on demand.

**🔘 Big Data and Analytics in Testing:** Analyzes large test and system data to improve quality and decisions.

**🔘 Test Data Management Solutions:** Manages, prepares, and secures test data for reliable testing.
