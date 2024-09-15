

Questions:
Most programming language research has been done in the context of sequential computation, and by now we have arguably converged on a core of features that are available in most modern programming languages (e.g. higher-order functions, (partial) type-inference, pattern matching, ADTs, parametric polymorphism) and are well understood. There is as yet no such consensus about programming language features for concurrent and parallel computation.
How has the question been addressed in the past? What are the historical developments?
Which subfields of PL contributed to investigating the question?
How did these subfields influence each other?
Who are the influential researchers who left their mark on the field?
What are some of the most influential research articles, books, software, etc?

References:

A conversation with Chat-GPT 3:
---

### 1. Historical Developments

#### Early Work (1960s-1970s)
- **Multiprogramming and Time-Sharing Systems**: In the 1960s, the focus was on improving the efficiency of computers by allowing multiple users to run programs concurrently on a single machine. This led to the development of **multiprogramming** and **time-sharing** systems. Early languages like **ALGOL** and **Simula** introduced concepts related to concurrent execution, such as processes and simulation of real-world phenomena.
- **Simula**: Developed by Ole-Johan Dahl and Kristen Nygaard, Simula introduced the concept of **coroutines** and **processes**, which were early forms of concurrency in programming languages.

#### Theoretical Foundations (1970s-1980s)
- **Petri Nets** (1962): Carl Adam Petri introduced **Petri Nets**, a mathematical modeling tool used to describe distributed systems and concurrent processes. Petri Nets provide a graphical and formal approach to understanding concurrency and synchronization.
- **CSP (Communicating Sequential Processes)** (1978): Tony Hoare introduced CSP, a formal language for describing patterns of interaction in concurrent systems. CSP uses processes that communicate by passing messages, providing a theoretical framework for concurrency.
- **Actor Model** (1973): Carl Hewitt proposed the Actor Model, which abstracts concurrent computation as a collection of actors that interact through message passing. This model influenced the development of languages like Erlang.

#### Formal Verification and Models (1980s-1990s)
- **Temporal Logic** (1977): Amir Pnueli introduced **temporal logic**, a formal system for specifying and reasoning about the behavior of concurrent systems over time. Temporal logic allows verification of properties such as safety and liveness in concurrent programs.
- **Model Checking** (1981): The advent of **model checking** techniques, developed by Clarke, Emerson, and Sifakis, allowed automated verification of concurrent systems by exploring all possible states of a system to ensure correctness.
- **Pi-Calculus** (1992): Robin Milner’s **Pi-calculus** extended the previous work on process calculi to handle mobile systems, providing a formal model for analyzing the dynamics of concurrent and distributed processes.

#### Languages Designed for Concurrency (1990s-present)
- **Erlang** (1986): Developed by Joe Armstrong and others, Erlang was designed for building scalable and fault-tolerant systems. It uses lightweight processes (actors) for concurrency and message passing for communication.
- **Go** (2009): Designed by Google, Go includes **goroutines** and **channels** as core features for concurrent programming. Goroutines are lightweight threads managed by the Go runtime, and channels provide a way to communicate between goroutines.
- **Rust** (2015): Rust introduced modern concurrency features with a focus on safety and performance. Its ownership and borrowing system prevents data races and ensures memory safety in concurrent contexts.

---

### 2. Subfields that Contributed to Concurrent/Parallel Computation

#### Concurrency Theory
- **Process Calculi**: Theoretical frameworks like **CSP** and **Pi-calculus** model and analyze the behavior of concurrent systems. These models provide tools for reasoning about interactions and communication in systems with multiple processes.
- **Actor Model**: This model abstracts concurrency as a collection of actors that perform computations and communicate through message passing. It has influenced the design of various concurrent programming languages.

#### Formal Methods and Verification
- **Temporal Logic**: Provides a formal language for specifying and verifying properties of concurrent systems. It allows for reasoning about how system states evolve over time, ensuring that systems meet desired specifications.
- **Model Checking**: A verification technique that exhaustively explores all possible states of a system to ensure correctness with respect to specified properties. Model checking is crucial for verifying concurrent and distributed systems.

#### Programming Language Design
- **Threads and Locks**: Early languages introduced basic constructs like threads and locks for managing concurrency. Later developments included more sophisticated synchronization mechanisms.
- **Parallelism Constructs**: Languages and libraries (e.g., **OpenMP**, **MPI**) provided constructs for expressing parallelism, enabling efficient execution on multi-core processors and distributed systems.

#### Distributed Systems
- **Distributed Computing**: Focuses on systems where components located on networked computers communicate and coordinate their actions. Research in this area overlaps with concurrency due to the need for managing communication, synchronization, and fault tolerance in distributed systems.

---

### 3. Influence Between Subfields

- **Theoretical Influence on Practical Languages**: Theoretical models like **CSP** and **Pi-calculus** provided foundational concepts that were incorporated into practical programming languages. For example, Erlang's actor model was inspired by theoretical work on concurrency.
- **Practical Needs Driving Theory**: Practical challenges in distributed and parallel computing led to the development of new theoretical models. For instance, the need for efficient synchronization in distributed systems prompted research into new models of concurrency.

---

### 4. Influential Researchers and Their Contributions

#### Edsger W. Dijkstra
- **Semaphores**: Dijkstra’s work on semaphores provided foundational synchronization primitives for managing concurrency in programs.
- [Dijkstra’s work on semaphores](https://scholar.google.com/scholar?q=dijkstra+semaphores)

#### Tony Hoare
- **CSP**: Hoare’s Communicating Sequential Processes provided a theoretical framework for describing and analyzing concurrent systems.
- [Hoare’s CSP paper](https://scholar.google.com/scholar?q=hoare+csp)

#### Carl Hewitt
- **Actor Model**: Hewitt’s introduction of the Actor Model revolutionized concurrent programming by focusing on message passing between actors.
- [Hewitt’s Actor Model paper](https://scholar.google.com/scholar?q=hewitt+actor+model)

#### Robin Milner
- **Pi-calculus**: Milner’s work on Pi-calculus extended process calculi to handle mobile systems, providing a formal framework for concurrency.
- [Milner’s Pi-calculus paper](https://scholar.google.com/scholar?q=milner+pi-calculus)

#### Amir Pnueli
- **Temporal Logic**: Pnueli’s temporal logic provided a formal approach for specifying and verifying properties of concurrent systems.
- [Pnueli’s Temporal Logic paper](https://scholar.google.com/scholar?q=pnueli+temporal+logic)

#### Joe Armstrong
- **Erlang**: Armstrong’s development of Erlang introduced a practical approach to building reliable concurrent and distributed systems.
- [Armstrong’s Erlang thesis](https://scholar.google.com/scholar?q=joe+armstrong+erlang)

---

### 5. Influential Research Articles, Books, and Software

#### "A Discipline of Programming" by Edsger W. Dijkstra (1976)
- Focuses on formal programming methods, including principles for concurrency.
- [Link to book](https://scholar.google.com/scholar?q=dijkstra+discipline+of+programming)

#### "Communicating Sequential Processes" by Tony Hoare (1985)
- A foundational text on CSP, a formal language for modeling concurrent systems.
- [Link to book](https://scholar.google.com/scholar?q=hoare+communicating+sequential+processes)

#### "The Pi-calculus: A Theory of Mobile Processes" by Robin Milner (1999)
- Provides a formal model for analyzing mobile and concurrent systems.
- [Link to book](https://scholar.google.com/scholar?q=milner+pi-calculus)

#### "The Temporal Logic of Reactive and Concurrent Systems" by Zohar Manna and Amir Pnueli (1992)
- Discusses temporal logic for specifying and verifying concurrent systems.
- [Link to book](https://scholar.google.com/scholar?q=manna+pnueli+temporal+logic)

#### Erlang
- A programming language designed for concurrency and fault tolerance.
- [Link to Erlang documentation](https://www.erlang.org/)

#### Rust
- A modern language focusing on safety and concurrency.
- [Link to Rust documentation](https://www.rust-lang.org/)

#### Go
- A language designed for simplicity and concurrency with goroutines and channels.
- [Link to Go documentation](https://golang.org/)

---
