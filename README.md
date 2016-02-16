# TU Delft CS4110: Software Testing and Reverse Engineering

2015-2016 Q3 — [TU Delft Study Guide](http://studiegids.tudelft.nl/a101_displayCourse.do?course_id=37845)

## Collaboration

### Communication

We are using Slack! Use [cs4110.slack.com](https://cs4110.slack.com/) and sign-up with your TU Delft or UTwente email address.

### GitHub

GitHub is used for collaboration on assignments. Teams (project groups) can be formed through the Classroom for GitHub interface; please find the invitation link in the Blackboard announcement. For your convenience, we also provide [an overview of all teams and their topics](https://github.com/TUDelft-CS4110/syllabus/blob/master/TEAMS.md).

An empty, public repository is created for each team and we request you use that for work on the assignments. **Please create at least a README.md file with the team member names and the topic of choice.** If you have any questions, ask on Slack.

## General

### Motivation
Software is one of the most complex artifacts that mankind has ever created, but complexity is the enemy of correctness. Modern software testing tools use a multitude of automated techniques geared towards correct computer code, amongst others:

 * Concrete and symbolic (concolic) testing
 * Execution monitoring
 * Mutation testing
 * Reverse engineering and binary analysis
 * Search-based and model-based test case generation
 * State machine learning or inference
 * Web testing

### Synopsis
In this course, we learn state-of-the-art techniques for testing the correctness of software. The main content of the course will be a lab assignment in which we will apply a modern testing technique to a software component. This testing lab can be performed in two flavours:

 * Black-box: testing and monitoring the software’s interactions without trying to understand its internal logic. Fuzz testing, state machine learning, and tainting are typical examples.
 * White-box: directly testing the software’s internal logic through code analysis and writing specific test cases. Typical examples are unit testing, concolic testing, mutation testing, and binary analysis.

The different testing techniques will be studied based on recent scientific literature. Pairs of students will then choose one of the flavors and apply one state-of-the-art testing technique to real software code.

### Aim
To get knowledge, understanding and skills with respect to modern software testing of real software systems.

### Learning outcomes
The student will acquire:

* Understanding of different advanced software testing techniques
* Ability to test and improve the correctness of existing systems
* Ability to analyze and reverse-engineer software code

### Examination
Lab work 50% including a written report 30% and presentation of the results 20%.

### Contents
The main part of the course will consist of a lab assignment where the students will need to test a real software system using state-of-the-art techniques described in the scientific literature. This will be supported by a few lectures covering the tools and techniques that are required for these tasks, such as SAGE, Pitest, CWSandbox, LearnLib, Torx, Sulley, Crawljax, Valgrind, and Z3. There will be many instruction sessions where students can work on their assignment and ask the teachers and TAs for assistance.

### Core text
Various papers from the literature.

## Topics & papers

We are currently building the literature overview. Depending on the number of students, you will work in groups of 2-3 students, discussing papers from a selected topic and then testing the topic in a lab with real software. The topics and software will be posted here in the next few days.

### Mutation testing

 * Jia Yue, Mark Harman. An Analysis and Survey of the Development of Mutation Testing. IEEE Transactions on Software Engineering,  vol.37, no.5, pp.649-678, Sept.-Oct. 2011
 * J.H. Andrews,  L.C. Briand, Y. Labiche,  A.S. Namin. Using Mutation Analysis for Assessing and Comparing Testing Coverage Criteria. IEEE Transactions on Software Engineering, , vol.32, no.8, pp.608-624, Aug. 2006
 * René Just, Darioush Jalali, Laura Inozemtseva, Michael D. Ernst, Reid Holmes, and Gordon Fraser. 2014. Are mutants a valid substitute for real faults in software testing?. In Proceedings of the 22nd ACM SIGSOFT International Symposium on Foundations of Software Engineering (FSE 2014). ACM, New York, NY, USA, 654-665.

### Automated test case generation


 * Phil McMinn. Search-Based Software Test Data Generation: A Survey. Software Testing, Verification and Reliability, vol. 14, no. 2, pp. 105–156, 2004.
 * Paolo Tonella. Evolutionary testing of classes. In Proceedings of the 2004 ACM SIGSOFT international symposium on Software testing and analysis (ISSTA '04). ACM, New York, NY, USA, 119-128.
 * G. Fraser and A. Arcuri. Whole Test Suite Generation. IEEE Transactions on Software Engineering, vol. 39, iss. 2, pp. 276-291, 2013.


### Automated reverse engineering 1 - Active state machine learning

 * Howar, Falk, Malte Isberner, and Bernhard Steffen. "Tutorial: Automata Learning in Practice." Leveraging Applications of Formal Methods, Verification and Validation. Technologies for Mastering Change. Springer Berlin Heidelberg, 2014. 499-513.
 * De Ruiter, Joeri, and Erik Poll. "Protocol state fuzzing of TLS implementations." USENIX Security. 2015.
 * Aarts, Fides, et al. "Improving active Mealy machine learning for protocol conformance testing." Machine learning 96.1-2 (2014): 189-224.
 * Bauer, Oliver, Maren Geske, and Malte Isberner. "Analyzing program behavior through active automata learning." International Journal on Software Tools for Technology Transfer 16.5 (2014): 531-542.
 * Cho, Chia Yuan, Eui Chul Richard Shin, and Dawn Song. "Inference and analysis of formal models of botnet command and control protocols." Proceedings of the 17th ACM conference on Computer and communications security. ACM, 2010.

### Automated reverse engineering 2 - Passive state machine learning

 * Marijn J.H. Heule and Sicco Verwer. 2013. Software model synthesis using satisfiability solvers. Empir. Softw. Eng. 18, 4 (August 2013), 825–856.
 * Walkinshaw, Neil, Russell Taylor, and John Derrick. "Inferring extended finite state machine models from software executions." Reverse Engineering (WCRE), 2013 20th Working Conference on. IEEE, 2013.
 * Comparetti, Paolo Milani, et al. "Prospex: Protocol specification extraction." Security and Privacy, 2009 30th IEEE Symposium on. IEEE, 2009.
 * Cui, Weidong, Jayanthkumar Kannan, and Helen J. Wang. "Discoverer: Automatic Protocol Reverse Engineering from Network Traces." USENIX Security. 2007.

### Malware analysis

 * Egele, Manuel, et al. "A survey on automated dynamic malware-analysis techniques and tools." ACM Computing Surveys (CSUR) 44.2 (2012): 6.
 * Rossow, Christian, et al. "Prudent practices for designing malware experiments: Status quo and outlook." Security and Privacy (SP), 2012 IEEE Symposium on. IEEE, 2012.
 * Caballero, Juan, et al. "Dispatcher: Enabling active botnet infiltration using automatic protocol reverse-engineering." Proceedings of the 16th ACM conference on Computer and communications security. ACM, 2009.
 * Wagener, Gérard, Radu State, and Alexandre Dulaunoy. "Malware behaviour analysis." Journal in Computer Virology 4.4 (2008): 279-287.

### Fuzzing and concolic testing

 * Godefroid, Patrice, Michael Y. Levin, and David Molnar. "SAGE: whitebox fuzzing for security testing." Queue 10.1 (2012): 20.
 * Cadar, Cristian, and Koushik Sen. "Symbolic execution for software testing: three decades later." Communications of the ACM 56.2 (2013): 82-90.
 * Yan Shoshitaishvili, Ruoyu Wang, Christophe Hauser, Christopher Kruegel, and Giovanni Vigna. 2015. Firmalice - Automatic Detection of Authentication Bypass Vulnerabilities in Binary Firmware. In Proceedings 2015 Network and Distributed System Security Symposium. Reston, VA: Internet Society.
 * Holler, Christian, Kim Herzig, and Andreas Zeller. "Fuzzing with Code Fragments." USENIX Security Symposium. 2012.

### Reverse engineering

 * Kruegel, C., Robertson, W., Valeur, F., & Vigna, G. (2004, August). Static disassembly of obfuscated binaries. In USENIX security Symposium (Vol. 13, pp. 18-18).
 * Kinder, J., & Veith, H. (2008, January). Jakstab: A static analysis platform for binaries. In Computer Aided Verification (pp. 423-427). Springer Berlin Heidelberg.
 * Willems, C., & Freiling, F. C. (2012). Reverse Code Engineering—State of the Art and Countermeasures. it-Information Technology Methoden und innovative Anwendungen der Informatik und Informationstechnik, 54(2), 53-63.
 * Conti, G., Dean, E., Sinda, M., & Sangster, B. (2008). Visual reverse engineering of binary and data files. In Visualization for Computer Security (pp. 1-17). Springer Berlin Heidelberg.
