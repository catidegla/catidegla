# Christ-loisele Atidegla

Cybersecurity, and network and information security. Telecommunications engineering by training, BSc, and that is where the habit comes from: you do not get to assume the link is clean, the peer is who it claims to be, or that the message arrived because you sent it.

Coding is the passion rather than the job title. It is how I take a thing apart. Most of what is here is security tooling for the parts of a stack that are now shipped without review, plus payment code for rails where the problems worth solving are the ones the happy path hides. A callback that never arrives, a timeout you cannot tell apart from a success, a QR that scans and is then refused. English and French.

### Security

- **[mcpaudit](https://github.com/catidegla/mcpaudit)**: security auditing for MCP servers, mapped to the OWASP MCP Top 10. Built around a corpus of real manifests it is not allowed to fire on, because a scanner that is wrong four times in five teaches people to skip the report.
- **[stacksec](https://github.com/catidegla/stacksec)**: Semgrep rules for Laravel and Next.js, each one shipping the code it must stay quiet about alongside the code it must catch.
- **[bumpdiff](https://github.com/catidegla/bumpdiff)**: what a dependency bump changed about what a package can *do*, not how many lines moved. New install scripts, new outbound hosts, a new publisher. Nothing executes and nothing lands on disk.
- **[machinemade](https://github.com/catidegla/machinemade)**: line level authorship recorded in git notes, in a form somebody who does not trust you can verify for themselves.

### Payments

- **[laravel-mobile-money](https://github.com/catidegla/laravel-mobile-money)**: MTN MoMo, Wave and Orange Money behind one Laravel interface, with the driver chosen from the payer's number rather than named by the caller. It writes the row before it calls the provider, so a process that dies mid-call leaves a record rather than a payment nobody knows about, and it reconciles the callbacks that never arrive.
- **[pi-spi-qr](https://github.com/catidegla/pi-spi-qr)**: build, parse and validate the interoperable QR payloads of the BCEAO instant payment platform. Eight countries, one franc, no dependencies. BCEAO publishes official SDKs in four languages and none of them is PHP.

### Also

- **[skillbelt](https://github.com/catidegla/skillbelt)**: portable agent skills for secure coding and translation parity, working across Claude Code, Codex, Cursor, Gemini CLI and Antigravity from one install.
- **[driftline](https://github.com/catidegla/driftline)**: whether your LLM provider swapped the model under a name that did not change. Committed probes, the provider's own fingerprint when it reports one, a G-test on the answer distribution when it does not.
- **[awesome-laravel-ai](https://github.com/catidegla/awesome-laravel-ai)**: every actively maintained Laravel AI package, with star and install counts that refresh themselves daily instead of rotting.

### Stack

PHP and Laravel, TypeScript and Node. Security review is the thread through all of it, and everything ships with the test that proves the awkward case rather than the one that proves the demo.
