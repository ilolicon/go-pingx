# go-ping

[![GoDoc](https://godoc.org/github.com/digineo/go-ping?status.svg)](https://godoc.org/github.com/digineo/go-ping)
[![Build Status](https://github.com/digineo/go-ping/workflows/build/badge.svg?branch=master)](https://github.com/digineo/go-ping/actions)
[![Codecov](https://codecov.io/gh/digineo/go-ping/branch/master/graph/badge.svg)](https://codecov.io/gh/digineo/go-ping)
[![Go Report Card](https://goreportcard.com/badge/github.com/digineo/go-ping)](https://goreportcard.com/report/github.com/digineo/go-ping)

## Notice

**Forked** from [digineo/go-ping](https://github.com/digineo/go-ping.git)

A simple ICMP Echo implementation, based on [golang.org/x/net/icmp][net-icmp].

Some sample programs are provided in `cmd/`:

- [**`ping-test`**][ping-test] is a really simple ping clone
- [**`multiping`**][multiping] provides an interactive TUI to ping multiple hosts
- [**`ping-monitor`**][monitor] pings multiple hosts in parallel, but just prints the summary every so often
- [**`pingnet`**][pingnet] allows to ping every host in a CIDR range (e.g. 0.0.0.0/0 :-))

[net-icmp]: https://godoc.org/golang.org/x/net/icmp
[ping-test]: https://github.com/digineo/go-ping/tree/master/cmd/ping-test
[multiping]: https://github.com/digineo/go-ping/tree/master/cmd/multiping
[monitor]: https://github.com/digineo/go-ping/tree/master/cmd/ping-monitor
[pingnet]: https://github.com/digineo/go-ping/tree/master/cmd/pingnet

## Features

- [x] IPv4 and IPv6 support
- [x] Unicast and multicast support
- [x] configurable retry amount and timeout duration
- [x] configurable payload size (and content)
- [x] round trip time measurement
- [x] configurable outbound interface to specified (like `ping -I`)
- [x] configurable outbound mark to specified (like `ping -m`)

## Contribute

Simply fork and create a pull-request. We'll try to respond in a timely
fashion.

## Software using this library

* [Ping Exporter for Prometheus](https://github.com/czerwonk/ping_exporter)

Please create a pull request to get your software listed.

## License

MIT License, Copyright (c) 2018 Digineo GmbH

<https://www.digineo.de>
