# Christ-loisele Atidegla

Payments and application security, in PHP and Node. Most of what I publish comes out of the West African payment rails, where the problems worth solving are the ones the happy path hides: a callback that never arrives, a timeout you cannot tell apart from a success, a QR that scans and is then refused. English and French.

### Currently

- **[laravel-mobile-money](https://github.com/catidegla/laravel-mobile-money)**: MTN MoMo, Wave and Orange Money behind one Laravel interface, with the driver chosen from the payer's number rather than named by the caller. It writes the row before it calls the provider, so a process that dies mid-call leaves a record rather than a payment nobody knows about, and it reconciles the callbacks that never arrive.
- **[pi-spi-qr](https://github.com/catidegla/pi-spi-qr)**: build, parse and validate the interoperable QR payloads of the BCEAO instant payment platform. Eight countries, one franc, no dependencies. BCEAO publishes official SDKs in four languages and none of them is PHP.
- **[mcpaudit](https://github.com/catidegla/mcpaudit)**: security auditing for MCP servers, mapped to the OWASP MCP Top 10. Built around a corpus of real manifests it is not allowed to fire on, because a scanner that is wrong four times in five teaches people to skip the report.
- **[skillbelt](https://github.com/catidegla/skillbelt)**: portable agent skills for secure coding and translation parity, working across Claude Code, Codex, Cursor, Gemini CLI and Antigravity from one install.

Also [awesome-laravel-ai](https://github.com/catidegla/awesome-laravel-ai), which tracks every actively maintained Laravel AI package with star and install counts that refresh themselves daily instead of rotting.

### Stack

PHP and Laravel, TypeScript and Node. Security review is the thread through most of it, and everything ships with the test that proves the awkward case rather than the one that proves the demo.
