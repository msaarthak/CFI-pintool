# cfipintool
In today's world, there are a lot of software vulnerabilities. We study Control Flow Integrity that prevents a widely-known attack called Return-Oriented Programming.  CFI restricts the control flow  of an application to valid execution traces. We used Intel Pin Tool, C Programming Language and Linux OS (Ubuntu) to help demonstrate CFI. 

CFI detects control-flow hijacking attacks by limiting the targets of control-flow transfers. In a control-flow hijack attack an attacker redirects the control-flow of the application to locations that would not be reached in a benign execution, e.g., to injected code or to code that is reused in an alternate context.
Any CFI mechanism consists of two abstract components: the (often static) analysis component that recovers the Control-Flow Graph (CFG) of the application (at different levels of precision) and the dynamic enforcement mechanism that restricts control flows according to the generated CFG. If implemented correctly, CFI is a strong defense mechanism that restricts the freedom of an attacker. Attackers may still corrupt memory and data-only attacks are still in scope.

For the forward-edge, a strong mechanism must consider language-specific semantics to restrict the set of valid targets as much as possible. Limiting the size of the target sets constrains the attacker on the forward edge. For the backward edge, a context-sensitive approach that enforces stack integrity guarantees full protection.


All the work in this repository was created under the mentorship of Dr. Arvind Mallari Rao who is a scientist at DRDO( Defence Reserach and Development Organization). Check out his papers here :- https://scholar.google.com/citations?user=RTGwMqgAAAAJ&hl=en
