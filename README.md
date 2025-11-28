# CORINT Decision Engine

**High-performance, deterministic real-time decision engine.**  
Part of the **CORINT – Cognitive Risk Intelligence Framework**.

## 🚀 Overview

`corint-decision` is the real-time risk decision engine of the CORINT framework.  
It is responsible for evaluating rules, executing strategies, orchestrating decision flows, and returning risk outcomes with millisecond-level latency.

It powers the core online risk pipeline, including:

- Rule execution (Rules Engine)
- Strategy & pipeline orchestration
- Feature computation
- Risk scoring
- Deterministic decisioning
- Real-time API decision service

## ✨ Features

- ⚡ **Low-latency real-time processing**
- 🔍 **Deterministic and fully auditable**
- 🧩 **Modular rules and pipeline architecture**
- 📡 **REST / gRPC compatible**
- 🛡️ **Safe sandboxed execution (planned)**
- 📈 **Explainable decisions**

## 📐 Architecture

```
Request → Feature Compute → Rules Engine → Pipeline → Decision → Response
```

## 📦 Example Use Cases

- Fraud detection  
- Identity risk  
- Transaction monitoring  
- Account takeover prevention  
- Credit risk decisioning  

## 📚 Documentation

### DSL Documentation

The CORINT Risk Definition Language (RDL) documentation is available in `doc/dsl/`:

**Overview & Architecture:**
- [`overall.md`](doc/dsl/overall.md) - High-level overview and introduction
- [`ARCHITECTURE.md`](doc/dsl/ARCHITECTURE.md) - Three-layer decision architecture (design philosophy)

**Core Components:**
- [`expression.md`](doc/dsl/expression.md) - Expression language (fundamental syntax)
- [`rule.md`](doc/dsl/rule.md) - Rule specification
- [`ruleset.md`](doc/dsl/ruleset.md) - Ruleset and decision logic
- [`pipeline.md`](doc/dsl/pipeline.md) - Pipeline orchestration

**Data & Schema:**
- [`event.md`](doc/dsl/event.md) - Standard event types and schemas
- [`schema.md`](doc/dsl/schema.md) - Type system and data schemas
- [`context.md`](doc/dsl/context.md) - Context and variable management

**Advanced Features:**
- [`feature.md`](doc/dsl/feature.md) - **Feature engineering and statistical analysis** ⭐
- [`llm.md`](doc/dsl/llm.md) - LLM integration guide
- [`service.md`](doc/dsl/service.md) - **Internal service integration** ⭐
- [`external.md`](doc/dsl/external.md) - External API integration (third-party services)

**Operational:**
- [`error-handling.md`](doc/dsl/error-handling.md) - Error handling strategies
- [`observability.md`](doc/dsl/observability.md) - Monitoring and logging
- [`test.md`](doc/dsl/test.md) - Testing framework
- [`performance.md`](doc/dsl/performance.md) - Performance optimization

**Examples:**
- [`examples/`](doc/dsl/examples/) - Real-world pipeline examples
- [`examples/statistical-analysis.yml`](doc/dsl/examples/statistical-analysis.yml) - Comprehensive statistical analysis example

### Quick Links

- **Feature Engineering**: For statistical analysis like "login count in the past 7 days" or "number of device IDs associated with the same IP in the past 5 hours", see [`feature.md`](doc/dsl/feature.md)
- **Internal Services**: For database queries, cache access, microservice calls, and message queue integration, see [`service.md`](doc/dsl/service.md)
- **External APIs**: For third-party API integration (Chainalysis, MaxMind, etc.), see [`external.md`](doc/dsl/external.md)

## 🤝 Contributing

Contributions are welcome!  
Please open issues, start discussions, or submit pull requests.

---

© 2025 CORINT Project — Elastic License
