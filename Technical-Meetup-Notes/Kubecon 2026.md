
## Day 1

### Keynote 1
- llm-d
### Keynote 3
 - litmuschaos
### Keynote 4
- LLM models inference on Kubernetes 
- vLLM, Nvidia Dynamo
### Keynote 5
- HAMi - providing GPU slices
- DRA
- vcluster
- gemma 3
### Observability for AI agents
- Semantic conventions for gen AI systems - OTel
- Instrumentation for AI models with OTel
- OpenLIT, Open inference, OpenLLMetry
- OTel eBPF Instrumentation 
- https://github.com/ishanjainn/ai-observability
- evals : agent evaluations. Single turn or multi-turn (maintaining context across a conversation )
- Langfuse?
### Kafka Observability 
- OTel for Kafka Observability 
- Auto Instrumentation before customising 
### Kubernetes Operators
- Deployment is a primary resource and pod corresponding to that deployment is the secondary resource
- Need to watch specific resources with the labels and selectors to reduce the load
### Native Istio and Envoy metrics based Observability
-  Prometheus Adapter to add visibility to the custom metrics API of Kubernetes which can used for HPA
- Envoy logging modes - check verbose logs for packet tracing
### Kubevela
- Open Application Model
### Networking incident walk-through
- Half open TCP connection 
- Keep Alive mechanism
-  MQTT
- tcp_retries2

### Dynamic model selection and semantic routing using CN patterns
- vLLM semantic router (*)
- open responses specification
- ToolRAG
- adding the ability for an agent to critique itself and self correct
- Envoy AI Gateway (*)
- LLM as a judge

## Day-2

#### Keynote 3
- qwen LLM
- https://github.com/cerebro1/vulnerability-check-kubecon2026.git
- teampcp?
### Keynote 4
- Kyverno for Policy as Code
- OpenReports project
- Exceptions/AERs as code
### gRPC transport for MCP
- stdio-sse, streamable-http , json-rpc
- low latency services use gRPC
- SPIFFE?
- dispatcher pattern?
### Zero trust for autonomous agents
- Openchoreo?, ThunderID?
- microsegmentation
- cell based architecture and cell gateway
- nesting the action and the subject in the tokens to pass identity
- CIBA, OBO
- Isolation ane Identity provides enhanced security
### Personal AI cluster
- Nvidia DGX spark
- NVIDIA GPU operator, DRA driver for GPUs
- vLLM is used for inferencing on k8s cluster

### Alternative to kube-proxy
- Publishing custom metrics to k8s metric server and letting HPA make us of them 
- knative?

### Running AI agents on k8s
- emulate GPU devices on local clusters to learn about DRA CR
- agent can be run on gVisor or  Kata to prevent container escape 

### Sandboxing
- Bubblewrap sandbox?
- microVM sandbox
- tokenizing secrets (explore)
- Temporal?
- k8s : agent sandbox project 
- envoy's credentials injector filter