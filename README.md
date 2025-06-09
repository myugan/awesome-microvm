# Awesome microVM [![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)

List of awesome resources about microVM included blogs, videos, projects and etc.

## Table of Contents

- [Papers](#papers)
- [Blogs](#blogs)
  - [Getting Started](#getting-started)
  - [Security](#security)
  - [Advanced Usage](#advanced-usage)
- [Videos](#videos)
- [Projects](#projects)
- [SDK](#sdk)
- [Use Cases](#use-cases)
- [Contributing](#contributing)

## Papers

- [Microarchitectural Security of AWS Firecracker VMM for Serverless Cloud Platforms](https://arxiv.org/pdf/2311.15999)
- [Attacks are Forwarded: Breaking the Isolation of MicroVM-based Containers Through Operation Forwarding](https://www.usenix.org/system/files/usenixsecurity23-xiao-jietao.pdf)

## Blogs

### Getting Started

- [The Firecracker virtual machine monitor](https://lwn.net/Articles/775736/)
- [Firecracker: start a VM in less than a second](https://jvns.ca/blog/2021/01/23/firecracker--start-a-vm-in-less-than-a-second/)
- [Building my VMs with Docker](https://jvns.ca/blog/2021/01/22/day-44--got-some-vms-to-start-in-firecracker/)
- [Firecracker internals: a deep dive inside the technology powering AWS Lambda](https://www.talhoffman.com/2021/07/18/firecracker-internals/)
- [Taking Firecracker for a spin](https://gruchalski.com/posts/2021-02-06-taking-firecracker-for-a-spin/)
- [Bridging the Firecracker network gap](https://gruchalski.com/posts/2021-02-17-bridging-the-firecracker-network-gap/)
- [Networking for a Firecracker Lab](https://blog.0x74696d.com/posts/networking-firecracker-lab/)
- [Communicating Between Firecracker microVMs using Linux Bridges](https://devopschops.com/blog/communicating-between-firecracker-microvms-using-bridges/)
- [Thoughts on creating VMMs from Docker images](https://gruchalski.com/posts/2021-03-03-thoughts-on-creating-vmms-from-docker-images/)
- [Firecracker VMM with additional disks](https://gruchalski.com/posts/2021-02-14-firecracker-vmm-with-additional-disks/)
- [Live resize Firecracker VMM drive](https://gruchalski.com/posts/2021-02-16-live-resize-firecracker-vmm-drive/)
- [Build a Firecracker microVM from a container image (Alex Ellis)](https://github.com/alexellis/firecracker-init-lab)

### Advanced Usage

- [Automation to run VMs based on vanilla Cloud Images on Firecracker](https://ongres.com/blog/automation-to-run-vms-based-on-vanilla-cloud-images-on-firecracker/)
- [Scaling Firecracker: Using OverlayFS to Save Disk Space](https://e2b.dev/blog/scaling-firecracker-using-overlayfs-to-save-disk-space)
- [Space Efficient Filesystems for Firecracker](https://parandrus.dev/devicemapper/)
- [Cloning microVMs by sharing memory through userfaultfd](https://codesandbox.io/blog/cloning-microvms-using-userfaultfd)
- [Running Linux microVMs on macOS (M1/M2)](https://slp.prose.sh/running-microvms-on-m1)
- [How to run Firecracker without KVM on cloud VMs](https://blog.alexellis.io/how-to-run-firecracker-without-kvm-on-regular-cloud-vms/)

### Security

- [Attacking Firecracker - AWS' microVM Monitor Written in Rust](https://chomp.ie/Blog+Posts/Attacking+Firecracker+-+AWS'+microVM+Monitor+Written+in+Rust)

## Videos

- [A cracking time: Exploring Firecracker & MicroVMs](https://www.youtube.com/watch?v=CYCsa5e2vqg)
- [Lightning Talk: What Are MicroVMs? And Why Should I Care?](https://www.youtube.com/watch?v=4d0NIfuFLXc&t=698s)
- [Face off: VMs vs. Containers vs Firecracker](https://www.youtube.com/watch?v=pTQ_jVYhAoc)
- [How MicroVMs can take your Kubernetes home lab to the next lvl](https://www.youtube.com/watch?v=4d0NIfuFLXc&t=698s)
- [Deep Dive into firecracker-containerd](https://www.youtube.com/watch?v=0wEiizErKZw)
- [Firecracker, should it work only with a single runtime?](https://youtu.be/n0xtvAMdY1w?si=aNy8uIhY4-b-bPnf)
- [Reusing bazel's analysis cache by cloning micro-VMs](https://www.youtube.com/watch?v=k30xZfiRZYo)
- [Create A Custom Linux Init in Python](https://fosdem.org/2025/schedule/event/fosdem-2025-5260-create-a-custom-linux-init-in-python/)

## Projects

- [rust-vmm](https://github.com/rust-vmm) - Shared Rust crates powering Firecracker and other VMMs.
- [firecracker](https://github.com/firecracker-microvm/firecracker) - Secure and fast microVMs for serverless computing.
- [firecracker-containerd](https://github.com/firecracker-microvm/firecracker-containerd) - Enables containerd to manage containers as Firecracker microVMs.
- [firecracker-task-driver](https://github.com/cneira/firecracker-task-driver) - Nomad task driver that uses firecracker to start micro-vms.
- [firectl](https://github.com/firecracker-microvm/firectl) - A command-line tool to run Firecracker microVMs.
- [buildfs](https://github.com/rust-firecracker/buildfs) - A tool for creating a VM root filesystem image from a reproducible TOML build script easily.
- [Flintlock](https://github.com/liquidmetal-dev/flintlock) - Lock, Stock, and Two Smoking MicroVMs. Create and manage the lifecycle of MicroVMs backed by containerd.
- [Cloud Hypervisor](https://github.com/cloud-hypervisor/cloud-hypervisor) - A Virtual Machine Monitor for modern Cloud workloads.
- [krunvm](https://github.com/containers/krunvm) - Create microVMs from OCI images.
- [vAccel](https://vaccel.org/) - Give your serverless deployments the power of hardware accelerators with vAccel
- [Fireactions](https://github.com/hostinger/fireactions) - BYOM (Bring Your Own Metal) and run self-hosted GitHub runners in ephemeral, fast and secure Firecracker based virtual machines.
- [KubeFire](https://github.com/innobead/kubefire) - Creates and manages Kubernetes Clusters using Firecracker microVMs.
- [Hyperlight](https://github.com/hyperlight-dev/hyperlight) - A lightweight Virtual Machine Manager (VMM) designed to be embedded within applications.

## SDK

- [firecracker-go-sdk](https://github.com/firecracker-microvm/firecracker-go-sdk) - An SDK in Go for the Firecracker microVM API.
- [firecracker-rs-sdk](https://crates.io/crates/firecracker-rs-sdk) - The Firecracker Rust SDK. A pure Rust crate for interacting with Firecracker.
- [firecracker-python](https://github.com/myugan/firecracker-python/) - An SDK in Python for the Firecracker microVM API.

## Who Are Using MicroVMs?

- [actuated](https://actuated.com)
- [architect](https://architect.run/)
- [CodeSandbox](https://codesandbox.io)
- [E2B](https://e2b.dev)
- [Fly.io](https://fly.io)
- [iximiuz Labs](https://labs.iximiuz.com/)

## Use Cases

- [Blazing fast CI with MicroVMs](https://blog.alexellis.io/blazing-fast-ci-with-microvms/)
- [Using Firecracker and Go to run short-lived, untrusted code execution jobs](https://stanislas.blog/2021/08/firecracker/)
- [Building a Firecracker-Powered Course Platform To Learn Docker and Kubernetes](https://iximiuz.com/en/posts/iximiuz-labs-story/)
- [Running containers on Firecracker microVMs using kata on kubernetes](https://blog.cloudkernels.net/posts/kata-fc-k3s-k8s/)
- [Exploring Firecracker MicroVMs for Multi-Tenant Dagger CI/CD Pipelines](https://www.felipecruz.es/exploring-firecracker-microvms-for-multi-tenant-dagger-ci-cd-pipelines/)

## Contributing

Your contributions are always welcome.

## License

[![CC0](https://i.creativecommons.org/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
