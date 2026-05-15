OpenArmature is a workflow framework for LLM pipelines and tool-calling agents. Its primitives compose into both deterministic LLM pipelines and autonomous tool-calling agents, with the same observable behavior across implementations.

What makes it distinctive: bad graph shapes fail at compile time, not at run time, and node-boundary observer hooks make every transition inspectable without buy-in from individual nodes. The framework ships typed, frozen state with structural graph checks, composable middleware, first-class checkpoint/resume, and OpenTelemetry observability.

The framework exists because most LLM workflow tooling locks you into one library, in one language, with semantics that drift between releases. OpenArmature inverts that: the contract lives in a language-agnostic specification with canonical conformance fixtures, and reference implementations in each language port to the same observable behavior.

The Python reference implementation is in active development at [openarmature-python](https://github.com/openarmature/openarmature-python). The language-agnostic specification, governance, and proposal history live at [openarmature.org](https://openarmature.org); implementation documentation and guides are at [openarmature.ai](https://openarmature.ai).

## Projects

- **openarmature-python** — the Python reference implementation (active)
- **spec** — the language-agnostic specification and conformance fixtures (in progress)
- **openarmature-typescript** — the TypeScript port (planned)
