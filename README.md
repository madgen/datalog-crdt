# CmRDT implementations in Datalog

A collection of Commutative Replicated Data Type (CmRDT) implementations in
Datalog ([Souffle](http://souffle-lang.org) syntax).

So far...

 - Positive-Negative counter
 - Last-Writer-Wins register
 - Multi-Value register
 - Grow-Only set
 - Two-Phase set
 - Last-Writer-Wins set
 - Positive-Negative set
 - Two-Phase-Two-Phase graph
 - Add-Only-Monotonic graph
 - Add-Remove partial order

## Observed-Remove set

So this set is tricky/pointless to implement in Datalog as the crucial bit of
the algorithm is to remove only the locally observed elements (made unique with
an identifier).
