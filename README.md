# rx-matching-engine
An implement of a matching engine in Rust. Implementation of a Limit Order Book only. The Limit OrderBook process the ITCH data at 4.89 Million messages per second as tested on my local device.


## Build and Run
### Build
```bash
cargo build
```
or
```bash
cargo build --release
```

### Execution
```bash
## make sure ITCH  binary data and executables are in same dir.
./<executable binary>
```



## Device Specifications
```text
MacBook Air M2

```
## Performance

### ITCH Parser Performance

```text
Parser Metrics:

ITCH Parsing Statistics:
Total Messages: 240017065
Total Time: 8.658 seconds
Rate: 27721741 msg/second
Latency: 36 ns
```

### Limit OrderBook Performance

```text
Metrics:
Total Messages: 240017065
ITCH Latency: 204 ns
Total Time: 49.028 seconds
Rate: 4895546 msg/second

Orderbook State:
Total Add Orders: 117145568
Total Execute Orders: 5722824
Total Cancel Orders: 2787676
Total Delete Orders: 114360997
```
## ITCH Specs
<!-- itch-specs -->
 `Nasdaq TotalView-ITCH 5.0`

- [Protocol Specifications](http://www.nasdaqtrader.com/content/technicalsupport/specifications/dataproducts/NQTVITCHSpecification.pdf)
- ITCH DATA download page: https://emi.nasdaq.com/ITCH/Nasdaq%20ITCH/
