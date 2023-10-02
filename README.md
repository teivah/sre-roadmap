# SRE Roadmap

An Opinionated Roadmap to Become SRE

Concepts > Tools

* _Distributed systems_
  * _Concepts_
    * Fallacies of distributed computing
    * Different types of message failure
    * Average connection speed of a user
    * Byzantine fault-tolerance
    * Causality
    * CDN
    * Consistent hashing
    * Geohashing
    * Perfect hashing
    * Event log vs. message queue
    * CQRS
    * Event sourcing
    * Read-heavy vs. write-heavy impacts
    * Exactly-once delivery
    * Federation
    * FLP impossibility
    * _Latency_
      * Latency, throughput, goodput
      * Latency numbers every programmer should know
      * How to prevent latency variability
      * Tail latency
    * How to reduce sharing
    * HDFS
    * Idempotency
    * Layer 4 vs. layer 7 load balancer
    * Liveness vs. safety proprties
    * Locality performance optimization
    * MapReduce
    * Microservices: pros and cons
    * Multi-tenant vs. multi-single-tenant
    * Orchestration vs. choreography
    * REST
    * gRPC
    * Service mesh
    * Source of truth
    * Stateful vs. stateless
    * Synchronous vs. asynchronous
    * Total vs. partial order
    * Why can't we rely on the system clock in distributed systems
  * _Cache_
    * When to use a cache
    * Cache-aside vs. read-through
    * Eviction policy
    * Refresh-ahead
    * Write-through vs. write-back
    * Different cache locations (client caching, CDN, in-memory, database, etc.)
    * Distributed cache
    * Performance cache vs. capacity cache
  * _Databases_
    * _Different types of databases_
      * NoSQL vs. SQL databases
      * Relational vs. document
      * Column-oriented databases
      * Graph databases
      * Objects-based storage
      * Vector database
    * ACID
    * Anti-entropy
    * _Partitioning_
      * Criteria
      * Methods
      * Replication vs. partition
    * Hotspot
    * CALM theorem
    * CAP theorem
    * PACELC theorem
    * Cardinality
    * Chain replication
    * Consensus
    * Concurrency control
    * Consistency models
    * Isolation levels
    * CRDT
    * _Indexes_
      * Tradeoff
      * Primary vs. secondary indexes
    * Denormalization
    * View & materialized view
    * Transaction
    * Distributed transactions downsides
    * Fencing token
    * Gossip
    * Durability in objects-based storage
    * Hinted handoff
    * Strategies to handle rebalancing
    * LWW
    * Leader election
    * MVCC
    * N+1 select problem
    * Quorum
    * Raft
    * Read repair
    * Serializability
    * Linearizability
    * Single-leader, multi-leader, leaderless replication
    * Split-brain
    * 2PC
    * 3PC
    * WAL
    * Write and read amplification
  * _Data structure_
    * Bloom filter
    * Count-min sketch
    * HyperLogLog
    * LSM tree
    * B-tree
    * Merkle tree
    * Quadtree
    * SSTable
    * Vector clock
* _Reliability_
  * _Concepts_
    * Difference between availability, resiliency, robustness, fault-tolerance, and reliability
    * Blast radius
    * Failure domain
    * Cascading failures
    * Hard vs. soft dependencies
    * _Scalability_
      * Concepts
      * Knee point
      * Ceiling
    * Number one source of outages (change)
    * Tail tolerance
    * Why is it wrong to target 100% availability
    * SRE role
    * Toil
    * MTTR/MTTD
  * _Patterns/Anti-patterns_
    * Bulkhead pattern
    * Circuit breaker
    * Exponential backoff
    * Jitter
    * Graceful degradation
    * Load shedding
    * Retry amplification
    * Phi-accrual failure detector
    * Query of death
    * Backpressure
    * Rate limiting
    * Request hedging
  * _Practices_
    * Chaos engineering 
* _Observability_
  * _Concepts_
    * What's the difference between monitoring and observability
    * Trace vs. metric vs. log
    * Golden signals
    * Observer effect
    * Percentile
    * Streetlight anti-method
    * Time-series based monitoring lies
    * USE method
    * VALET dashboard
    * Why should we be careful about average performance metrics
    * Main metrics for cache
  * _Alerting_
    * Alerting strategy
    * Alerting fatigue concept
    * Characteristic of a good alert
    * Slow vs. fast burn alert
* _Rollout_
  * _Concepts_ 
    * Bake time
    * Feature flag
    * Feature freeze
    * Rollout supervision
  * _Rollout types_
    * Blue green rollout
    * Canary rollout
    * Progressive rollout
    * Shadow rollout
* _SLI/SLO/SLA_
  * _Concepts_
    * SLI vs. SLO vs. SLA
    * Error budget
  * _SLO_
    * Difference between KPIs and SLOs
    * Benefits of having alerts based on SLOs
    * Why is exceeding an SLO not necessarily a good thing
    * SLO for data (freshness, completeness, consistency, etc.)
    * SLO for mobiles
    * SLO for services
* _Analysis_
  * Core analysis loop
  * Correlation vs. causation
  * First principle
  * Five whys technique
  * _Incident management_
    * How to address an incident (assess, mitigate, resolve)
    * Incident roles
    * How to write a postmortem
    * 3C principles (Coordinate, Communicate, maintain Control)
* _Network_
  * ARP protocol
  * Bandwidth
  * BGP
  * Bufferbloat
  * CoDel
  * CORS
  * DNS
  * Ping vs. heartbeat
  * _TCP_
    * TCP vs. UDP
    * Congestion control
    * Connection backlog
    * Flow control
    * Handshake
  * HTTP
  * HTTP/2
  * Head of line blocking
  * Health checks: passive vs. active
  * Internet model
  * NTP
  * OSI model
  * Routers
  * STP
  * Switch
  * Network topologies
  * What happens if you type google.com in your browser
* _Security_
  * Authentication
  * Certificate
  * Certificate authority
  * Cipher
  * Confidentiality
  * Encryption
  * TLS
  * PKI
  * Signature
* _Other_
  * Backward vs. forward compatibility
