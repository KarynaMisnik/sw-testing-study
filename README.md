## Software Testing Study Notes

**Content:**

- [Importance of SW Testing](#importance-of-sw-testing)
- [Test Process](#test-process)
- [Designing Test Cases](#designing-test-cases)
- [Black Box Testing](#black-box-testing)
  - [Dynamic Testing](#dynamic-testing)
    - [Black box Testing](#black-box-testing)
- [White Box Testing](#white-box-testing)

## Importance of SW Testing

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

## Test Process

**SDLC** - software development lifecycle(Software
Test Process).

<ins>The Software Test Life Cycle (STLC)</ins> is a sequence of specific testing phases, they are carried out systematically to ensure that software is tested <b>efficiently</b> and <b>effectively</b>.

The testing process - from planning to closure.

#### Testing Phases

       Planning
          ↓
       Analysis
          ↓
        Design
          ↓
    Implementation
          ↓
      Execution
          ↓
      Completeion

1️⃣ **Planning**
Purpose: Decide what, how, and when testing will be done.

Activities:
Define scope, objectives, testing types.
Identify resources, tools, effort, and schedule.

Output: Test plan document.

**Analysis**
Purpose: Understand requirements and what needs to be tested.

Activities:
Analyze functional and non-functional requirements.
Identify testable requirements.
Prepare requirement traceability matrix (RTM).

Output: List of testable requirements, RTM.

2️⃣ **Design**
Purpose: Create detailed test cases and data.

Activities:
Write test cases and test scripts.
Prepare test data.
Review and get approvals.

Output: Test cases, test scripts, test data.

3️⃣ **Implementation**
Purpose: Prepare the testing environment and get ready for execution.

Activities:
Set up test environment (hardware, software, network).
Configure tools, servers, databases.
Ensure everything is ready for test execution.

Output: Ready-to-run test environment, test scripts finalized.

4️⃣ **Execution**
Purpose: Run the tests and report results.

Activities:
Execute test cases.
Log defects and track their status.

Retest after fixes.

Output: Test execution reports, defect logs.

5️⃣ **Closure**
Purpose: Conclude testing and evaluate quality.

Activities:
Assess test coverage and effectiveness.
Document lessons learned and best practices.

Output: Test closure report.

## Designing Test Cases

1. Understand the Program
   Before designing test cases, clearly understand:
   What the program does
   Its inputs
   Its outputs

Consider different categories of input:
Valid inputs — expected to work
Invalid inputs — should be rejected or handled safely
Boundary / edge values — limits that may cause errors

Focus on expected behavior, not on the source code implementation.

2. What Makes a Good Test Case
   Ask yourself: Why did I choose this test case?

A good test case:
Helps reveal a fault
Is unique (not redundant)
Is meaningful (neither too trivial nor unnecessarily complex)

A poor test case:
Tests the same behavior as another test
Uses inputs with unclear expected results
Uses random values without a clear purpose

3. Identify Test Inputs
   Ask: What does this test case check?

Each test case should include:
Input values
Expected results
A clear reason for the test

4. Order of Test Cases
   4.1 Test-to-Pass (Verify Normal Behavior)
   Valid inputs
   Typical use cases
   Expected to succeed

4.2 Test-to-Fail (Try to Break the System)
Invalid inputs
Boundary conditions
Error-forcing scenarios

Exhaustive testing is impossible — quality matters more than quantity.

5. Document Test Cases
   Each documented test case should include:
   Inputs
   Expected results
   A short explanation of what it verifies

6. Review Test Coverage
   Ask: Are all main behaviors covered?

If two test cases check the same behavior, keep the stronger one
Remove redundant or low-value tests

## Black Box Testing

**Test case execution strategy**

| **Testing Approach**                         | **Purpose / Focus**                                                                                          | **Example (ATM Withdrawal)**                                                                                                |
| -------------------------------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------- |
| **1. Test-to-pass (Positive Testing)**       | Verify normal functionality, “happy path”                                                                    | Enter correct PIN, withdraw $100 → ATM dispenses money, balance updated                                                     |
| **2. Test-to-fail (Negative / Destructive)** | Provide invalid inputs to ensure system handles them gracefully                                              | Enter wrong PIN, withdraw more than balance, withdraw zero or negative amount → ATM blocks card or shows error              |
| **3. Error-forcing**                         | Force system into error conditions to reveal hidden defects; deliberately break rules                        | Remove network connection during withdrawal, tamper with card, simulate cash shortage → ATM handles errors without crashing |
| **4. Exhaustive Testing**                    | Test all possible valid & invalid scenarios (impractical for big systems, usually applied to critical areas) | Test **all PIN combinations, all withdrawal amounts, all card types, all error states** → ensures nothing is missed         |

> NOTE: Positive → Negative → Forced errors → Exhaustive coverage is a
> logical “defect-hunting ladder.”

### Dynamic Testing

**Dynamic testing** is a type of software testing where the actual code is executed to verify that the software behaves as expected.

<ins>Key Points about Dynamic Testing:</ins>
🔸Execution-based: You actually run the program.
🔸Validates behavior: Checks whether the software produces correct results.
🔸Detects defects: Finds errors, crashes, incorrect outputs, performance issues, etc.
🔸Can be functional or non-functional:
🔸Functional: Verify features like ATM withdrawal, login, borrowing books
🔸Non-functional: Test performance, load, stress, security

💡 Remember:

Static Testing: Code is not executed (reviews, walkthroughs, inspections)
Dynamic Testing: Code is executed with inputs to check results

#### Black Box Testing

**Black Box Testing** is a software testing technique where the tester does not look at the internal code or logic of the application. The focus is entirely on inputs and outputs.

<ins>Key Points about Black Box Testing</ins>

1. No knowledge of internal code
   Testers interact with the software as an end user would.
2. Focus on functionality
   Ensures the system meets requirements and specifications.
3. Test based on requirements
   Often derived from specifications, user stories, or use cases.
4. Detects
   Missing functionality
   Incorrect outputs
   User interface issues
   Performance or security issues (if functional)

**Types:**

1. Equivalence Partitioning (EP)

<ins>Idea:</ins> Divide input data into groups (partitions) where all values are expected to be treated the same by the system.

<ins>Purpose:</ins> Reduce the number of test cases while still covering scenarios.

**Example (ATM Withdrawal):**
Partition 1: Valid PINs → 4-digit numbers 0000–9999
Partition 2: Invalid PINs → non-numeric, 3-digit numbers, blank input
You test one value from each partition instead of every possible input.

2. Boundary Value Analysis (BVA)

<ins>Idea:</ins> Errors often occur at the edges of input ranges, so test minimum, maximum, just below, and just above values.

<ins>Purpose:</ins> Catch off-by-one and range-related errors.

**Example (ATM Withdrawal):**
Min withdrawal = $10, Max withdrawal = $2000
Test cases: $9 (just below), $10 (min), $2000 (max), $2001 (just above)

3. Combinatorial Testing

<ins>Idea:</ins> Test all possible combinations of multiple inputs or factors.

<ins>Purpose:</ins> Ensure system behaves correctly when multiple conditions interact.

**Example (ATM Withdrawal):**
Inputs: PIN (correct/incorrect), Withdrawal amount (valid/invalid), Account type (savings/current)
Combinations: Test all possible scenarios like correct PIN + valid amount + savings account, incorrect PIN + invalid amount + current account, etc.

4. Decision Table Testing

<ins>Idea:</ins> Represent different combinations of inputs (conditions) and corresponding actions in a table to systematically create test cases.

<ins>Purpose:</ins> Handle complex business logic with multiple rules.

**Example (ATM Withdrawal):**
| Condition 1 | Condition 2 | Action |
| ------------- | -------------------- | --------------------------- |
| Correct PIN | Sufficient balance | Dispense cash |
| Correct PIN | Insufficient balance | Show error |
| Incorrect PIN | Any balance | Block card after 3 attempts |

### White Box Testing

**White Box Testing** (also called structural or glass box testing) is a testing technique where the tester has knowledge of the internal code, logic, and structure of the software and designs tests based on that.

Instead of only checking inputs and outputs, white box testing checks how the code works internally.

<ins>Key Characteristics</ins>
🔹Tester knows the source code
🔹Focuses on logic, control flow, and data flow
🔹Usually performed by developers or testers with coding knowledge
🔹Ensures the code is correct, complete, and efficient

<ins>What White Box Testing Verifies</ins>
🔹All statements are executed at least once
🔹All branches/decisions are tested (if–else, loops)
🔹Loops run correctly (0 times, 1 time, many times)
🔹Internal error handling works
🔹Code paths don’t contain unreachable or dead code

<ins>When White Box Testing Is Used</ins>
🔺Unit testing
🔺Integration testing
🔺Security testing (finding hidden vulnerabilities)
🔺Code optimization and refactoring

1. **Statement Coverage**

**What it means:**
Ensures every executable statement (line of code) is run at least once.

**Goal:**
Check that no line of code is completely untested.

**Example:**

```bash
IF PIN is valid
   show "Welcome"
show "Insert amount"
```

Test with valid PIN → both statements execute
Statement coverage = 100%

⚠️ Limitation:

Doesn’t guarantee all decisions (true/false) are tested.

2. **Branch (Decision) Coverage**

**What it means:**
Ensures every decision outcome (true and false) is executed at least once.

**Goal:**
Verify logic correctness of if, else, switch, loops.

**Example:**

```bash
IF balance >= amount
   dispense cash
ELSE
   show error
```

Test cases:

balance ≥ amount → TRUE branch
balance < amount → FALSE branch

✅ Both branches tested → full branch coverage.

3. **Path Coverage**

**What it means:**
Ensures all possible execution paths in the program are tested.

**Goal:**
Catch defects caused by specific sequences of decisions.

**Example:**

```bash
IF PIN valid
   IF balance sufficient
      dispense cash
   ELSE
      show error
ELSE
   block card
```

Possible paths:
Valid PIN → sufficient balance
Valid PIN → insufficient balance
Invalid PIN

All paths must be tested for 100% path coverage.

⚠️ Note:
Can be very expensive or impossible for complex programs.

4. **Multiple Condition Coverage**

**What it means:**
Ensures all combinations of conditions inside a decision are tested.

**Goal:**
Validate complex boolean logic.

**Example:**

```bash
IF (PIN valid AND account active)
   allow withdrawal
```

Conditions:
PIN valid (T/F)
Account active (T/F)

Test combinations:
T, T → allow withdrawal
T, F → reject
F, T → reject
F, F → reject

✅ All combinations tested → full multiple condition coverage.

**Summary:**

| Coverage Type               | Focus                      | Strength                       |
| --------------------------- | -------------------------- | ------------------------------ |
| Statement Coverage          | Lines of code              | Finds unexecuted code          |
| Branch Coverage             | True/False decisions       | Validates logic flow           |
| Path Coverage               | All execution paths        | Catches complex logic errors   |
| Multiple Condition Coverage | All condition combinations | Best for complex boolean rules |
