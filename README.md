# ankit-system-design
System Design

### Learning Strategy:

System design learning typically follows two paths: Concepts and Problems.

#### Phase 1: Concepts Deep Dive

Start by understanding the fundamental building blocks and principles. For each concept, create a dedicated Markdown file (e.g., concepts/scalability.md, concepts/databases.md).

#### Foundation:

Networking Basics: DNS, HTTP/HTTPS, Load Balancers, Proxies.
Scalability: Vertical vs. Horizontal Scaling, Load Balancing strategies (Round Robin, Least Connections, etc.).
Availability: Redundancy, Failover, Disaster Recovery.
Reliability: Error handling, Retries, Circuit Breakers.
Performance: Caching (levels, strategies), CDNs, Latency, Throughput.
Core Components:

##### Databases:
Relational (SQL): When to use (ACID, complex queries), scaling challenges. (e.g., PostgreSQL, MySQL, Oracle)
NoSQL: When to use (scalability, flexibility), types (Key-Value, Document, Column-Family, Graph). (e.g., Redis, MongoDB, Cassandra, Neo4j)
Message Queues/Streaming: Why use them (decoupling, async processing, backpressure), types (Kafka, RabbitMQ, SQS).
Caching Systems: (e.g., Redis, Memcached) Local, Distributed, CDN.
APIs: REST, GraphQL, gRPC.
Authentication/Authorization: OAuth, JWT, Session-based.
Search Engines: (e.g., Elasticsearch, Solr) Indexing, querying.

#### Advanced Topics:

Microservices vs. Monoliths: Trade-offs, communication patterns.
Distributed Systems Challenges: Consistency models (CAP Theorem), Consensus (Paxos, Raft), Distributed Transactions.
Containerization & Orchestration: Docker, Kubernetes.
Monitoring & Alerting: Logging, Metrics.



##### Document Concepts in Your Repo:

1. Create a concepts/ directory.
2. For each concept, create a Markdown file: concepts/caching.md, concepts/load-balancing.md, etc.
3. In each file:

		1. Define the concept.
		2. Explain its purpose and benefits.
		3. Describe different types/strategies.
		4. Discuss pros and cons/trade-offs.
		5. Include diagrams (exported from Excalidraw/draw.io or generated with Mermaid) illustrating the concept.
		6. Link to external resources (articles, videos) where you learned about it.

