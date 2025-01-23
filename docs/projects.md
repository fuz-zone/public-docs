# Projects

A project in our fuzzing framework is defined by a set of target artifacts that you want to fuzz. Projects help organize related fuzzing targets and their associated harnesses.

## Project Types

### Source Code Projects
- **Git Repository**: Connect directly to your Git repository (GitHub, GitLab, Bitbucket)
- **Source Upload**: Upload source code as a zip/tar archive
- **Copy/Paste**: Directly paste source code for quick testing

### Binary Projects
- Standalone executables
- Shared libraries
- Object files
- Firmware images

### Docker Projects
- **Single Container**: Projects based on a Dockerfile or existing image
- **Multi-Container**: Complex environments requiring multiple interconnected containers
- **Custom Networks**: Support for custom Docker networking configurations

### System Image Projects
- **Raw Disk Images**: Full system testing with raw disk images
- **QCOW2 Images**: KVM/QEMU virtual machine images
- **VMDK**: VMware disk format support

## Project Organization

Each project can contain multiple fuzzing harnesses targeting different components or entry points of your system. This allows you to:

- Organize related fuzzing targets
- Share configuration between harnesses
- Track coverage across multiple entry points
- Manage permissions and access control
- Generate comprehensive reports

## Best Practices

1. Use meaningful project names and descriptions
2. Organize related targets in the same project
3. Document project setup and requirements
4. Maintain separate projects for different versions or branches
5. Regular project backup and maintenance
