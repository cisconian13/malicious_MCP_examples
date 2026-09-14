MCP Security Test Lab

This repository contains intentionally adversarial MCP server code and test fixtures for authorized security testing with Cisco AI Defense.

The fixtures simulate common MCP/agent security risks without accessing real credentials, modifying production systems, executing destructive commands, or sending data externally.

Test Categories
Tool poisoning
Direct and indirect prompt injection
MCP resource poisoning
Tool shadowing
Rug-pull / supply-chain changes
Privilege escalation
Sensitive-data solicitation
Data-exfiltration intent
Memory poisoning
Capability chaining
Tool argument abuse
Obfuscated/hidden instructions
GitHub Integration

AI Defense can integrate with GitHub for MCP code scanning, MCP registry scanning, and model repository scanning.

Use this repository only in an isolated test environment.

Do not add:

Real credentials or secrets
Production customer data
Production MCP servers
Real external exfiltration endpoints
Destructive commands
Persistence mechanisms

All malicious behavior should remain simulated and use synthetic test data.

Expected Outcome

The objective is to verify that AI Defense can:

Detect malicious MCP code and metadata
Identify prompt-injection and tool-poisoning techniques
Detect suspicious changes to previously trusted MCP code
Identify attempts to access or disclose sensitive information
Distinguish malicious fixtures from benign MCP implementations

See expected-results/test-matrix.csv for the test cases and expected classifications.
