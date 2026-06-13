# Atlas

---

## **Description:**

1. Take a series of input nodes
2. processing layer takes connects to input nodes and does some processing and passes the results down to the next layer.
3. repeat 2 until the desired results are reached.

---

## **Components**

- threadpool (worker)
- NodeSpec:
  - graph def (wasm) each node -> bin -> load in rust
  - memory cell
  - entry node agnostic

## **Notes:**

- Entry of newer data invalidates the current processes. (cancellation policy)
- Possible extension to handle computations on the gpu?
- parents are defined by tyoes (labels for now). more generally said defining edges between nodes decleratively.
- do we reload the whole graph everytime the data trickles down the graph or do we cache?
- edge nodes for distributed computation


## **Modules**