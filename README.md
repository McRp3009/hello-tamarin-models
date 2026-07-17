# Hellō Tamarin Models

This repository contains the Tamarin Prover models developed as part of the master's thesis on the formal verification of the Hellō authentication protocol.

## Contents

* `hello.spthy` – Formal model of the original Hellō protocol analyzed under the baseline and stronger threat models.
* `moshi.spthy` – Formal model of the privacy-enhanced Hellō protocol variant presented and analyzed in the thesis.

## Requirements

* Tamarin Prover 1.12.0

## Usage

To open a model in the interactive interface:

```bash
tamarin-prover interactive hello.spthy
```

or

```bash
tamarin-prover interactive moshi.spthy
```

To verify a model from the command line:

```bash
tamarin-prover hello-original.spthy
```

or

```bash
tamarin-prover hello-enhanced.spthy
```

### Running with Compromise configuration

To run a model with the option to compromise a single internal service:

```bash
tamarin-prover -D=Compromise hello.spthy
```

or

```bash
tamarin-prover -D=Compromise moshi.spthy
```

## Thesis

These models accompany the master's thesis:

> *A Formal Analysis of the Hellō Distributed Authentication Protocol*

The original protocol model corresponds to the formal analysis presented in Chapters 4–6 of the thesis, while the privacy-enhanced protocol model corresponds to the analysis presented in Chapter 7.

## License

This repository is provided for research and educational purposes.
