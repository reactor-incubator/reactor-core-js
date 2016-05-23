# Reactor-Core-JS

The Reactive-Streams based implementation of Reactor-Core in TypeScript

# Usage

```javascript
import { Flux } from './node_modules/reactor-core-js/flux';

Flux.range(1, 10)
.take(5)
.map(v => v * 2)
.flatMap(v => Flux.range(v, 2))
.consume(v => console.log(v));
```

# Operator support

Import `flux` package.

## Reactive Entry points

  - `combineLatest`, `combineLatest2`, `combineLatest3`, `combineLatest4`
  - `concat`
  - `concatArray`
  - `defer`
  - `empty`
  - `fromArray`
  - `fromCallable`
  - `interval`
  - `just`
  - `merge`
  - `mergeArray`
  - `never`
  - `range`
  - `timer`
  - `zip`, `zip2`, `zip3`, `zip4`

## Reactive stay

  - `as`
  - `collect`
  - `combineWith`
  - `compose`
  - `concatWith`
  - `doOnAfterNext`
  - `doOnAfterTerminated`
  - `doOnCancel`
  - `doOnComplete`
  - `doOnError`
  - `doOnNext`
  - `doOnSubscribe`
  - `filter`
  - `flatMap`
  - `hide`
  - `lift`
  - `map`
  - `onErrorReturn`
  - `onErrorResumeNext`
  - `reduce`
  - `take`
  - `toArray`
  - `withLatestFrom`
  - `zipWith`

## Reactive Leave

  - `consume`
  - `subscribe`

## Scheduler

Import `scheduler` package.

  - `DefaultScheduler.INSTANCE`