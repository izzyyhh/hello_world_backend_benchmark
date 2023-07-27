# Benchmark on Mac Air M2 16GB | Node (Express) vs Go | Hello World endpoint

Express
```
~ » wrk -t8 -c100 -d30s http://localhost:4000
Running 30s test @ http://localhost:4000
  8 threads and 100 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency     5.79ms  768.81us  29.76ms   91.08%
    Req/Sec     2.08k   123.74     2.91k    96.75%
  498353 requests in 30.06s, 113.11MB read
Requests/sec:  16578.62
Transfer/sec:      3.76MB
```

Go
```
~ » wrk -t8 -c100 -d30s http://localhost:8000
Running 30s test @ http://localhost:8000
  8 threads and 100 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency     1.44ms    2.38ms  50.10ms   89.67%
    Req/Sec    14.63k     6.56k   34.38k    63.74%
  3495212 requests in 30.10s, 426.66MB read
Requests/sec: 116103.09
Transfer/sec:     14.17MB

```
