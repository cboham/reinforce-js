# REINFORCE-ts
*REINFORCE-ts* is an object-oriented Typescript port of _Andrej Karpathy's_ Reinforcement Learning library that implements several common RL algorithms.
In particular, the library currently includes:

* *Dynamic Programming* methods
* (Tabular) *Temporal Difference Learning* (SARSA/Q-Learning)
* *Deep Q-Learning* for Q-Learning with function approximation with Neural Networks
* *Stochastic/Deterministic Policy Gradients* and Actor Critic architectures for dealing with continuous action spaces. (_very alpha, likely buggy or at the very least finicky and inconsistent_)

For further Information see the [reinforce-js](https://github.com/karpathy/reinforcejs) repository.

# Dependencies

This Library relies on the object-oriented [recurrent-ts](https://github.com/mvrahden/recurrent-ts) _Deep Recurrent Neural Network_ library.

# Use as `npm`-Project Dependency

## To install as dependency:

```
npm install --save reinforce-ts
```

## To use the Library in Production:

Currently exposed Classes:

* *Solver* - Generic Interface
* *DQNSolver* - Concrete Solver
* *Env* - Environment a Solver
* *Opt* - Options a Solver

These classes can be directly imported from this `npm` module, e.g.:
```typescript
import { Solver, Env } from 'reinforce-ts';
```

# Contribute

1. `Clone` this project to a working directory.
2. `npm install` to setup the development dependencies.
3. To compile the codebase:

```
tsc -p .
```

This project relies on Visual Studio Codes built-in Typescript linting facilities. Let's follow primarily the [Google TypeScript Style-Guide](https://github.com/google/ts-style) through the included *tslint-google.json* configuration file.

# License

As of License-File: *MIT*
