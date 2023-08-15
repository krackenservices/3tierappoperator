# Demo Operator for 3 Tier App





## Setup Commands
- mkdir operator && cd operator
- go mod init github.com/krackenservices/3tierappoperator
- kubebuilder init --owner "Ryan McLean" --domain k8s.krackenservices.com
- kubebuilder edit --multigroup true
- kubebuilder create api --group api --version v1alpha1 --kind FailOverConfiguration
- kubebuilder create api --group core --version v1 --kind Pod
