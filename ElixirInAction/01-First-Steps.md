# First Steps
  - Elixir is built on top of Erlang, which is specially good at large, concurrent and scalable applications.
  - Keys for High Availability and reliability:
    * *Fault Tolerance*: Keep the services running, find the issue and the impact and recover fast from it;
    * *Scalability*: Respond gracefully to any load size possible;
    * *Distrubution*: Connecting and balancing the system across multiple machines, for increased stability and easier scaling;
    * *Reponsiveness*:  Request handling should be fast and, ideally, not affect the systems overall perfomance regardless of load or errors
    * *Live Update*:  Updating process should be transparent and smooth, not affecting or disabling functions while performed. 
## Concurrency:
  - Erlang runs on a VM, called BEAM
  - It manages concurrency itself, through internal Erlang processes.
  - The execution of these Erlang processes is delegated to the CPUs by BEAM.
  - Erlang processes are not dependant on the others, and do not have shared state. The only impact of an internal Erlang process crashing is local and Erlang gives you the means to address these crashes.
  - Erlang processes communicate only through messages, asynchronously. (Actor Model)
  - These processes can communicate to each other regardless of being in the same or separate instances or even different machines.
  - The runtime delegates the execution of the Erlang processes in small slices of time, therefore not allowing a single process to lock the whole system. IO is also ran separately, which allows for Node-like non-blocking IO operations;
  - An Erlang webserver can be used for diferent layers of a web application, ranging from Serving HTTP and request processing to background jobs and crash recovery

### About Elixir
  - Elixir compiles to Erlang Bytecode and runs in the BEAM VM
  - It offers the same capabilitise as Erlang, with total compatibility since they compile to the same type of bytecode.
  - Elixir syntax offers a more maintainable and easier to understand option than Erlang
  - Functional language, based on immutability
