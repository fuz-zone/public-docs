# Fuzzing Harnesses

A fuzzing harness is the interface between your target application and our fuzzing engine. It defines how inputs are delivered to your target and how results are collected.

## What is a Fuzzing Harness?

A fuzzing harness is a specialized piece of code that:
- Accepts input from the fuzzer
- Delivers that input to the target
- Monitors execution
- Reports crashes and other interesting behaviors
- Collects coverage information

## Supported Platforms

### Native Applications
- [Linux ELF/Shared Libraries](linux.md)
- [Windows EXE/DLL](windows.md)
- [Rust Applications](rust.md)

### Managed Runtimes
- [Python Applications](python.md)
- [JVM Applications](jvm.md)

### Special Environments
- [Embedded Systems](embedded.md)
- [Full System Emulation](embedded.md#system-emulation)

### Automated Creation
- [AI-Assisted Generation](ai-generation.md)

## Best Practices

1. Keep harnesses focused and minimal
2. Properly handle cleanup and resources
3. Implement robust input validation
4. Monitor memory usage
5. Enable relevant sanitizers
6. Document harness assumptions and limitations

## Choosing the Right Harness Type

Select your harness type based on:
- Target platform and runtime
- Access to source code
- Performance requirements
- Coverage needs
- Resource constraints
