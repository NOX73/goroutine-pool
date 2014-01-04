goroutine-pool
==============

My bicycle for managing pool of goroutines

Api smth like this:
```go

func Worker (a, b int) int {
  return a*b
}

p := pool.NewPool(Worker, 10)

// ....

w := p.GetWorker()
result, _ := w.Perform(1,2)

```
