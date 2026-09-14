MCP AI Defense Test Lab

This repository contains intentionally adversarial MCP servers for authorized security testing with Cisco AI Defense MCP Scanning.

All malicious behavior is simulated. The MCPs do not use real credentials, perform destructive actions, or send data externally.

Test MCPs
MCP	Attack Type
capability_chaining.py	Capability chaining
data_exfiltration.py	Data exfiltration
indirect_injection.py	Indirect prompt injection
malicious_resource.py	Malicious resource
memory_poisoning.py	Memory poisoning
privilege_escalation.py	Privilege escalation
sensitive_data_solicitation.py	Sensitive-data solicitation
tool_poisoning.py	Tool poisoning
tool_shadowing.py	Tool shadowing
GitHub Integration

AI Defense uses the Cisco AI Defense GitHub App to scan MCP code hosted in GitHub.

Prerequisites:

GitHub Organization
Organization Admin
Cisco AI Defense GitHub App authorization

Connect GitHub in:

AI Defense → Administration → Integrations → GitHub → Connect GitHub

Follow the GitHub authorization flow and select the organization containing this repository.

MCP Scanning

After the GitHub integration is connected, run the repository through:

AI Defense → Supply Chain Security → MCP Scanning

Record the findings and compare them with the expected attack types listed above.

Cisco documentation:
{"fallbackMarkdown":"AI Defense — MCP Scanning
","reference":{"matched_text":"","prefix":null,"start_idx":1591,"end_idx":1682,"safe_urls":[],"refs":[],"alt":"AI Defense — MCP Scanning
","prompt_text":"AI Defense — MCP Scanning
","type":"url","title":"AI Defense — MCP Scanning","item":{"title":"AI Defense — MCP Scanning","url":"https://securitydocs.cisco.com/docs/ai-def/user/168859.dita?utm_source=chatgpt.com","attribution":"securitydocs.cisco.com","pub_date":null,"snippet":null,"attribution_segments":null,"supporting_websites":null,"refs":[],"hue":null,"attributions":null},"layout":null,"logo":null},"showLoginRequiredCard":false}

Safety

Use this repository only in an isolated test environment.

Do not add real credentials, customer data, production systems, destructive commands, or real exfiltration endpoints.
