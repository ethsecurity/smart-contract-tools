# Fuzzing
Fuzz testers generate random input of some given specification and validate properties
of a given contract by attempting to find a sequence of inputs or series of inputs that
invalidates those properties.
It will then return to the user those sequence of inputs so that design against those inputs.
Fuzzers typically do not report false positives, as each sequence is directly possible to execute.
It is recommended practice to use fuzz testing to ensure that the properties of the contract
you wish to verify are not possible to break.
These properties should be driven by your smart contract's main requirements.

## [Echidna](https://github.com/trailofbits/echidna)
Fuzzer from Trail of Bits. Written in Haskell.
Uses property testing to generate malicious inputs that break smart contracts.

## [Hypothesis-Ethereum]() (No Release Yet!)
Leverages the popular Hypothesis tool as a foundation. Written in Python.
Adds custom types and fields for creating property-based tests.
Provided with the [Twig framework](github.com/ethereum/twig).
