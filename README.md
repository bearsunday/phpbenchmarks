# A repository for [phpbenchmarks](http://www.phpbenchmarks.com/en/) 

## Frameworks

 * [Symfony 4.2](https://github.com/phpbenchmarks/symfony/tree/symfony_4.2_hello-world) 
 * [BEAR.Sunday](https://github.com/bearsunday/BEAR.HelloworldBenchmark)

## Benchmarking
 
Symfony 4.2 + Apache

```
wrk http://localhost/benchmark/helloworld
Running 10s test @ http://localhost/benchmark/helloworld
  2 threads and 10 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency    24.34ms   40.86ms 253.81ms   85.63%
    Req/Sec     0.95k   218.40     1.50k    68.50%
  18964 requests in 10.01s, 4.16MB read
Requests/sec:   1894.52
Transfer/sec:    425.86KB
```

BEAR.Sunday + Apache

```
wrk http://localhost/
Running 10s test @ http://localhost/
  2 threads and 10 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency    26.00ms   46.96ms 288.33ms   85.90%
    Req/Sec     1.47k   415.95     2.69k    72.16%
  28417 requests in 10.01s, 5.83MB read
Requests/sec:   2837.67
Transfer/sec:    596.31KB
```

BEAR.Sunday + Swoole

```
wrk http://127.0.0.1:8080/
Running 10s test @ http://127.0.0.1:8080/
  2 threads and 10 connections
  Thread Stats   Avg      Stdev     Max   +/- Stdev
    Latency   582.27us  280.98us  10.59ms   85.88%
    Req/Sec     8.72k   837.17    10.95k    69.80%
  175266 requests in 10.10s, 33.43MB read
Requests/sec:  17353.27
Transfer/sec:      3.31MB
```