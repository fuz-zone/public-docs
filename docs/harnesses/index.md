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
- Linux ELF executables and shared libraries
- Windows PE executables and DLLs
- Rust applications with native compilation

### Managed Runtimes
- Python applications and modules
- Java and JVM-based applications
- .NET applications

### Special Environments
- Embedded systems
- Full system emulation
- IoT devices
- Mobile applications

### AI-Assisted Generation
Our platform can automatically generate harnesses using AI technology for:
- Common APIs and protocols
- Standard file formats
- Network services
- Web applications

## Best Practices

1. Keep harnesses focused and minimal
2. Properly handle cleanup and resources
3. Implement robust input validation
4. Monitor memory usage
5. Enable relevant sanitizers
6. Document harness assumptions and limitations

## Platform-Specific Guidelines

### Linux
- Support for both static and dynamic linking
- ASAN/UBSAN integration
- syscall interception

### Windows
- PE/COFF binary instrumentation
- DLL injection capabilities
- Exception handling

### Python
- Module-level fuzzing
- Custom import hooks
- Coverage tracking

### JVM
- Bytecode instrumentation
- Custom classloaders
- JNI support

## Choosing the Right Harness Type

Select your harness type based on:
- Target platform and runtime
- Access to source code
- Performance requirements
- Coverage needs
- Resource constraints
