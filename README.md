# SGP4 library for Go

[![Go Reference](https://pkg.go.dev/badge/github.com/SharkEzz/sgp4.svg)](https://pkg.go.dev/github.com/SharkEzz/sgp4)

## Background

The C++ SGP4 library is ported from [here](https://github.com/dnwrnr/sgp4)

Initial port was done by [sataas](https://github.com/akhenakh/sataas)

### How to update the bindings

- You will need [SWIG](http://www.swig.org)
- Clone the original [C++ SGP4 repository](https://github.com/dnwrnr/sgp4/tree/master/libsgp4)
- Run: `swig -c++ -intgosize 64 -go SGP4.i`
- The generated file will be `cppsgp4/cppsgp4.go`

## TODO

- [x] Remove all unnecessary dependencies for testing
- [ ] Enhance SGP4 Go API by adding more native C++ library functions
- [ ] Enhance documentation
