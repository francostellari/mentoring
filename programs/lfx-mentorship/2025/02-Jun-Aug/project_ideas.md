## Template

```
### CNCF Project Name

#### Mentorship project Title

- Description:
- Expected Outcome:
- Recommended Skills:
- Mentor(s):
  - Mentor Name (@mentor_github, mentor@email.addy) - please use the same email address as you use on the LFX Mentorship Platform at https://mentorship.lfx.linuxfoundation.org
- Upstream Issue:

```

---

## Proposed Project ideas

### Kubernetes

#### Graduate the kubeadm feature gate WaitForAllControlPlaneComponents to GA

- Description:  
The feature gate WaitForAllControlPlaneComponents is used to
enhance the health checks performed by kubeadm on control plane node creation,
to not only check the availability of the kube-apisever, but also check
the kube-controller-manager and kube-scheduler. In kubeadm 1.33, the feature gate
was promoted to Beta. As part of this LFX project it can be promoted to GA,
by finalizing the remaining work, such as, code changes, documentation updates
and e2e test updates.
- Expected Outcome: The feature gate is graduated to GA
- Recommended Skills: golang, Kubernetes, kubeadm
- Mentor(s):
  - Shida Qiu (@SataQiu, shidaqiu2018@gmail.com)
  - Paco Xu (@pacoxu, paco.xu@daocloud.io)
- Upstream Issue (URL): https://github.com/kubernetes/kubeadm/issues/2907

### KubeStellar

#### Building a Marketplace for KubeStellar Plugins

- Description:  
This project aims to develop a marketplace system for KubeStellar that will allow users to discover, install, and manage plugins that extend KubeStellar's functionality. The marketplace will provide a centralized hub for community-contributed plugins, enhancing KubeStellar's extensibility and user experience. The implementation will include a backend API written in Go and a frontend interface built with React.

- Expected Outcome
  - A fully functional plugin marketplace integrated into KubeStellar's UI
  - Backend API for plugin management (upload, discovery, installation, updates)
  - Frontend components for browsing, searching, and installing plugins
  - Plugin versioning and compatibility checking
  - User ratings and reviews for plugins
  - Documentation for plugin developers and users

- Recommended Skills
  - Go
  - React.ts
  - REST API
  - Kubernetes
  - KubeStellar
  - Docker
  - containerization
  - Git
  - GitHub workflow

- Mentor
  - Rishi Mondal (@MAVRICK-1 , mavrickrishi@gmail.com)
  - Andy Anderson (@clubanderson , andy@clubanderson.com)
  - Rahul Vishwakarma (@manzil-infinity180 , rahulvs2809@gmail.com)
- Upstream Issue: [https://github.com/kubestellar/ui/issues/606](https://github.com/kubestellar/ui/issues/606)


#### Implementing a Model Context Protocol for KubeStellar MCP Server

- Description:  
This project aims to develop a Model Context Protocol for KubeStellar's Management Control Plane (MCP) server. The protocol will establish a standardized communication framework between KubeStellar's internal components and the AI models used for command interpretation. By defining clear context boundaries, semantic structures, and state management patterns, the protocol will enable the MCP server to maintain consistent understanding of the multi-cluster environment while processing natural language management commands across KubeStellar deployments.

- Expected Outcome
  - A fully specified Model Context Protocol defining the interaction between KubeStellar and AI models
  - Implementation of protocol handlers in TypeScript or Python for the MCP server
  - Context management system that maintains KubeStellar state information for accurate command interpretation
  - Serialization and deserialization mechanisms for efficiently passing cluster state to models
  - Protocol extension mechanisms for supporting different AI providers
  - Performance optimizations for minimizing latency in command processing
  - Comprehensive test suite validating protocol reliability under various operational conditions

- Recommended Skills
  - KubeStellar
  - Model Context Protocol
  - protocol design and implementation
  - TypeScript
  - Python
  - AI model
  - GenAi
  - serialization formats
  - efficient data structures
  - distributed systems state management

- Mentor
  - Rishi Mondal (@MAVRICK-1 , mavrickrishi@gmail.com)
  - Andy Anderson (@clubanderson , andy@clubanderson.com)

- Upstream Issue: [https://github.com/kubestellar/ui/issues/607](https://github.com/kubestellar/ui/issues/607)


#### Enhancing KubeStellar: UI Modernization & Marketplace Integration

- Description:
This project aims to significantly transform the KubeStellar experience through comprehensive UI modernization with a central focus on introducing a robust Marketplace feature. The implementation will deliver a seamless way for users to discover and integrate extensions while also improving installation workflows, enhancing UI/UX elements, upgrading topology visualizations, and modernizing documentation. The marketplace will serve as a pivotal community hub that accelerates adoption and extensibility of the KubeStellar platform.

- Expected Outcome
  - A comprehensive Marketplace integrated directly into KubeStellar UI that pulls from kubestellar/galaxy, showcasing project cards with repository links, related blogs, star counts, categorization (Kubeflow, Argo Workflows, Keueu, etc.), and providing valuable social/usage insights to drive community engagement
  - Installation and Setup Guide integrated directly into KubeStellar UI with cluster readiness checker, guided installation wizard, and real-time error feedback and resolution flows
  - UI/UX Enhancements including performance optimizations, responsive design for various screen sizes, skeleton loading for improved perceived performance, and user management with role-based access controls
  - Topology Visualization Enhancements with improved graphical representations, more intuitive navigation, and enhanced interaction models
  - KubeStellar UI Documentation featuring integration of React components within the existing documentation site, interactive examples and demos, and component showcases

- Recommended Skills
  - React
  - TypeScript
  - Kubernetes
  - KubeStellar
  - UI/UX Design
  - REST API
  - Golang
  - GitHub workflow

- Mentor
  - Rishi Mondal (@MAVRICK-1 , mavrickrishi@gmail.com)
  - Andy Anderson (@clubanderson , andy@clubanderson.com)

- Upstream Issue: [https://github.com/kubestellar/ui/issues/615](https://github.com/kubestellar/ui/issues/615)


#### Enhancing KubeStellar core Helm chart by reducing its reliance on initContainers

- Description:
This project aims to investigate and implement ideas for improving KubeStellar Core Helm chart reliance by contributing improvements to Helm project and reducing its reliance on initContainers for waiting/gathering/processing Kubernetes resources that are used by other containers (for example, KubeFlex Control Planes and their kubeconfigs).
- Introduce an annotation that would make Helm wait for user-specified resources
- Introduce priority/coordination of Helm resource creation
- Introduce an alternative path for dependence chart override values
- Introduce a mechanism for a chart to require a specified Helm min version or range
- Introduce an alternative to kubectl initContainers

- Expected Outcome
  - A comprehensive investigation of potential alternative methods and approaches
  - Contributions to Helm project to introduce new features that would allow to improve the quality of KubeStellar Core chart
  - A solution implementation that reduces the reliance on kubectl initContainers

- Recommended Skills
  - Helm
  - Go
  - REST API
  - Kubernetes
  - KubeStellar
  - Docker
  - containerization
  - Git
  - GitHub workflow

- Mentor
  - Franco Stellari (@francostellari , fstellari@gmail.com)
  - Andy Anderson (@clubanderson , andy@clubanderson.com)

- Upstream Issues:
  - [https://github.com/kubestellar/kubestellar/issues/2890](https://github.com/kubestellar/kubestellar/issues/2890)
  - [https://github.com/helm/helm/issues/30669](https://github.com/helm/helm/issues/30669)
  - [https://github.com/helm/helm/issues/30670](https://github.com/helm/helm/issues/30670)
  - [https://github.com/helm/helm/issues/30671](https://github.com/helm/helm/issues/30671)
  - [https://github.com/helm/helm/issues/30672](https://github.com/helm/helm/issues/30672)
