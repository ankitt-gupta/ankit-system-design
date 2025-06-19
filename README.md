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



##### Document Concepts in Repo:

1. Create a concepts/ directory.
2. For each concept, create a Markdown file: concepts/caching.md, concepts/load-balancing.md, etc.
3. In each file:

		1. Define the concept.
		2. Explain its purpose and benefits.
		3. Describe different types/strategies.
		4. Discuss pros and cons/trade-offs.
		5. Include diagrams (exported from Excalidraw/draw.io or generated with Mermaid) illustrating the concept.
		6. Link to external resources (articles, videos) where you learned about it.


#### Phase 2: Problem Solving (Applied Design)

Once you have a grasp of the concepts, start tackling common system design interview problems.

##### Problem Selection:

		Start with simpler problems: "Design TinyURL," "Design a Pastebin," "Design a Key-Value Store."
		Move to more complex ones: "Design Twitter," "Design Netflix," "Design a Ride-Sharing App."
		Resources: "Grokking System Design Interview" (paid course, highly recommended), "System Design Interview – An Insider's Guide" (book), various YouTube channels (e.g., Gaurav Sen, ByteByteGo, Hussein Nasser).
		Structured Problem-Solving Approach (for each problem):
		For each problem, create a dedicated folder (e.g., problems/design-tinyurl/) and a README.md inside it.

##### Step 1: Understand the Requirements:

		Functional requirements (what it must do).
		Non-functional requirements (scale, latency, availability, consistency, durability).
		Estimations (users, QPS, storage, bandwidth).
		Document in README.md: "Requirements" section.

##### Step 2: High-Level Design (HLD):

		Identify core components (API Gateway, Load Balancer, Web Servers, Databases, Caches, Message Queues).
		Show data flow.
		Draw a High-Level Diagram: Embed it in your README.md. Explain each component's role.

##### Step 3: Deep Dive (Low-Level Design - LLD):

		API Design: Endpoints, request/response formats.
		Database Schema: Table structures, indexing, choice of DB (SQL vs. NoSQL) with justification.
		Data Partitioning/Sharding: How to distribute data.
		Caching Strategy: Where to cache, what to cache, invalidation.
		Load Balancing Details: Specific algorithms.
		Asynchronous Processing: If using message queues.
		Error Handling/Resiliency: How to handle failures.
		Security: Basic authentication/authorization considerations.
		Monitoring: How to observe the system.
		Document in README.md: Detailed sections for each. Add more granular diagrams.

##### Step 4: Trade-offs & Alternatives:

		Discuss decisions made and why (e.g., "Chose NoSQL for scalability over SQL for strong consistency here").
		Mention alternative approaches and their pros/cons.
		Document in README.md: "Trade-offs" or "Alternatives" section.

##### Step 5: Scalability Bottlenecks & Future Improvements:

		What are the potential bottlenecks in your design?
		How would you scale it further?
		Document in README.md: "Future Considerations" section.

