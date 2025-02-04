# Reconciling Accuracy, Cost, and Latency of Inference Serving Systems

## Abstract:

Machine Learning (ML) inference services are at the heart of many applications, serving user requests in real-time. These services require rapid and accurate responses while adapting to dynamic workloads and fluctuating resource availability. The challenges in achieving this include balancing latency, cost, and accuracy in the face of an exponentially large design space, multiple interacting system components, and the inherent uncertainty in dynamic environments. This talk introduces three cutting-edge solutions to address these challenges:

### InfAdapter
By combining model-switching and auto-scaling, InfAdapter enables a granular design space to trade accuracy, cost, and latency. It serves multiple model variants rather than a single one, allowing for fine-grained adaptation and superior trade-offs between conflicting objectives.

### IPA (Inference Pipeline Adaptation)
IPA extends InfAdapter to dynamically configure ML inference pipelines composed of multiple services arranged in a directed acyclic graph (DAG). Using Integer Programming, it optimizes batch size, resource allocation, and model variants to balance accuracy, latency, and cost. IPA’s multi-objective optimization adapts effectively to dynamic workloads and traffic patterns.

### Sponge
Sponge enhances resource efficiency by applying dynamic batching, request reordering, and in-place vertical scaling to guarantee dynamic service-level objectives (SLOs). Its Integer Programming-based resource allocation captures the intricate relationship between latency, batch size, and resources.

The talk will conclude with discussions on the broader implications of these methods, highlighting the paradigm shift from monolithic ML models to modular-composed systems. Modular systems, while unlocking vast optimization opportunities, bring challenges such as high-dimensional configuration spaces, dynamic uncertainty, and the need for real-time multi-objective optimization.

## Key Takeaways:

- The shift towards modular-composed systems introduces new opportunities and challenges in AI/ML system design.
- Multi-objective optimization is essential for reconciling conflicting goals of accuracy, latency, and cost.
- Solutions such as InfAdapter, IPA, and Sponge showcase practical advancements in addressing the above challenges through innovative methods like model-switching, DAG-level optimization, and dynamic resource scaling.

## Bio:

Pooyan Jamshidi is an assistant professor at the University of South Carolina's Department of Computer Science and Engineering. With experience as a visiting researcher at Google and postdoctoral researcher at Carnegie Mellon University and Imperial College London, Pooyan’s research spans software systems, AI/ML, and robotics. His work focuses on developing algorithms and tools for resilient systems that handle trade-offs, incorporate user preferences, and self-adapt to dynamic environments.

## Discussion Topics:

- How do modular-composed ML systems compare with monolithic models in terms of optimization complexity and flexibility?
- What are the practical implications of implementing multi-objective optimization in real-world systems?
- How can future research build on these advancements to further enhance modular-composed AI systems?