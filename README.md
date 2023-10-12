# SRE Roadmap

An opinionated roadmap to become an SRE (Concepts > Tools)


## Distributed systems

* _Concepts_
  * Fallacies of distributed computing
  * Synchronous vs. asynchronous
  * Event log vs. message queue
  * Exactly-once delivery
  * Different types of message failure
  * Orchestration vs. choreography
  * Causality
  * CDN
  * _Hashing_
    * Consistent hashing
    * Geohashing
    * Perfect hashing
  * Read-heavy vs. write-heavy impacts
  * Federation
  * _Latency_
    * Latency, throughput, goodput
    * Latency numbers every programmer should know
    * How to prevent latency variability
    * Tail latency
  * How to reduce sharing
  * Idempotency
  * _Load balancer_
    * Concepts
    * Layer 4 vs. layer 7 load balancer
  * Liveness vs. safety properties
  * Microservices: pros and cons
  * REST
  * gRPC
  * Service mesh
  * Source of truth
  * Stateful vs. stateless
  * Total vs. partial order
  * Why can't we rely on the system clock in distributed systems
  * Vector clock
* _Cache_
  * When to use a cache
  * Cache-aside vs. read-through
  * Eviction policy
  * Refresh-ahead
  * Write-through vs. write-back
  * Distributed cache
  * Performance cache vs. capacity cache
* _Databases_
  * _Different types of databases_
    * NoSQL vs. SQL databases
    * Relational vs. document
    * Column-oriented databases
    * Graph databases
    * Vector database
    * Objects-based storage
  * ACID
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
  * Serializability
  * Linearizability
  * CRDT
  * _Indexes_
    * Tradeoff
    * Primary vs. secondary indexes
  * Denormalization
  * View & materialized view
  * Transaction
  * Distributed transactions downsides
  * Strategies to handle rebalancing
  * Leader election
  * MVCC
  * N+1 select problem
  * Quorum
  * Raft
  * Read repair
  * Single-leader, multi-leader, leaderless replication
  * Split-brain
  * 2PC
  * 3PC
  * WAL
  * Write and read amplification
* _Data structure_
  * _Probabilistic data structures_
    * Bloom filter
    * Count-min sketch
    * HyperLogLog
  * _Storage_
    * LSM tree
    * B-tree
    * SSTable
      
## Reliability

* _Concepts_
  * Difference between availability, resiliency, robustness, fault-tolerance, and reliability
  * Why is it wrong to target 100% availability
  * Blast radius
  * Failure domain
  * Cascading failures
  * Hard vs. soft dependencies
  * _Scalability_
    * Concepts
    * Knee point
    * Ceiling
  * Number one source of outages
  * Tail tolerance
  * Toil
* _Patterns/Anti-patterns_
  * Bulkhead pattern
  * Circuit breaker
  * Exponential backoff
  * Jitter
  * Graceful degradation
  * Load shedding
  * Retry amplification
  * Backpressure
  * Rate limiting
  * Request hedging
* _Practices_
  * Chaos engineering 
    
## Observability
 
* _Concepts_
  * What's the difference between monitoring and observability
  * Trace vs. metric vs. log
  * Golden signals
  * Observer effect
  * Percentile
  * Streetlight anti-method
  * Time-series based monitoring lies
  * USE method
  * Main metrics for cache
  * Why should we be careful about average performance metrics
* _Alerting_
  * Alerting strategy
  * Alerting fatigue concept
  * Characteristic of a good alert
  * Slow vs. fast burn alert
     
## Rollout
 
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
  
## SLI/SLO/SLA

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
     
## Container

* Container
* Container orchestration
   
## Linux

* Scripting
* Filesystem
* Memory
* Processes
* Resource utilization
* Network
   
## Network

* ARP protocol
* Bandwidth
* BGP
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
* Switch
* Network topologies
* What happens if you type google.com in your browser
   
## Security
 
* Authentication
* Certificate
* Certificate authority
* Cipher
* Confidentiality
* Encryption
* TLS
* PKI
* Signature

## Incident management

* How to address an incident (assess, mitigate, resolve)
* Incident response roles
  * Incident Commander (IC)
  * Communications Lead (CL)
  * Operations Lead (OL)
* How to write an incident state document
* How to write a postmortem
* 3C principles (Coordinate, Communicate, maintain Control)
* RACI vs SRE

## Analysis
  * Core analysis loop
  * Correlation vs. causation
  * First principle
  * Five whys technique
  
## Other

* SRE role
* Version control

## Soft skills

* _Communication_
  * Writing
  * Oral
  * Presentation
  * First of Five
* Collaboration
* Problem solving
* Curiosity
* Navigating ambiguity
* Staying humble
