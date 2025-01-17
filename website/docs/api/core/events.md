---
sidebar_position: 2
---

# Events

Events are generated by service servers and can be subscribed with a callback.

## subscribe

The `subscribe` method registers a callback that runs when the event is received.

```ts
const button = new ds.Button()

button.down.subscribe(() => {
    console.log("click!")
})
```

## wait

The `wait` method blocks the tread until the event is received.

```ts
const button = new ds.Button()

await button.down.wait()
console.log("click!")
```
