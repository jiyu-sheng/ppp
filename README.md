# ppp
[![License](https://img.shields.io/badge/License-Apache%202.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)  
[![Build Status](https://travis-ci.org/misalcedo/ppp.svg?branch=master)](https://travis-ci.org/misalcedo/ppp)
[![Crates.io Version](https://img.shields.io/crates/v/ppp.svg)](https://crates.io/crates/ppp)

A Proxy Protocol Parser written in Rust.
See [HAProxy](https://www.haproxy.org/download/1.8/doc/proxy-protocol.txt) for the protocol specification.

## Benchmark
Ran `cargo bench` on a desktop with a hexa-core i7 processor with hyper-threading.

```bash
test binary::tests::bench_header_with_tlvs ... bench:         277 ns/iter (+/- 0)
test text::tests::bench_parse_tcp4         ... bench:         337 ns/iter (+/- 0)
test text::tests::bench_parse_tcp6         ... bench:         843 ns/iter (+/- 10)
test text::tests::bench_parse_tcp6_compact ... bench:         661 ns/iter (+/- 10)
```
