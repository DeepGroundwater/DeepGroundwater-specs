# Deep Groundwater Spec v0

!!! Warning
    This spec has not been accepted, and is subject to change

## Version

v0.0.1

## Editors
- Tadd Bindas (@taddyb), Earth Resources Technology (ERT)

## Issue Tracking

[Github Issues](https://github.com/DeepGroundwater/DeepGroundwater-specs/labels/V0%20Spec)

## License

This work is licensed under an Apache 2.0 [License](https://www.apache.org/licenses/LICENSE-2.0)

## Abstract

This specification defines the dataset formats for streamflow input ingestion, and geospatial references, to be used in DDR routing.

## Introduction

This specification defines a format for datasets used in the DeepGroundwater Open Source Repositories. In the field of hydrology, there is a notion that "if a dataset can be opened in Pandas, or xarray, then it is good enough to share." The primary motication for the development of DeepGroundwater is to address the problems within the hydrological open source community through ensuring easy-to-reproduce experiments, maintaining consistency between data products, and providing logical interfaces to environmental models.

The format of this specification draws from the [Zarr v3 Spec](https://zarr-specs.readthedocs.io/en/latest/v3/core/index.html). This specification defines a format for multidimensional array data. 

We highlight the following areas motivating the development of this specification.

## Extensibility

The development of hydrological datasets, and models, is a very active field of research and development with a lot to be explored with the introduction of Deep Learning, Differentiable Modeling, and the constant innvoation of data products/open source services. A goal of this speficiation is to define a format with a clear structure that can be scaled to the global/continental level, while maintaining the [FAIR Principles](https://www.go-fair.org/fair-principles/). We aim to make this possible, whilst also providing pathways for a graceful degradation of functionality where possible, in order to retain interoperability.

## Stability Policy

This core specification adheres to a `MAJOR.MINOR` version numbering format. When incrementing the minor version, only additional features can be added. Breaking changes require incrementing the major version.

## Document Conventions
Conformance requirements are expressed with a combination of descriptive assertions and [RFC2119](https://zarr-specs.readthedocs.io/en/latest/v3/stores/filesystem/index.html#rfc2119) terminology. The key words “MUST”, “MUST NOT”, “REQUIRED”, “SHALL”, “SHALL NOT”, “SHOULD”, “SHOULD NOT”, “RECOMMENDED”, “MAY”, and “OPTIONAL” in the normative parts of this document are to be interpreted as described in [RFC2119](https://zarr-specs.readthedocs.io/en/latest/v3/stores/filesystem/index.html#rfc2119). However, for readability, these words do not appear in all uppercase letters in this specification.

All of the text of this specification is normative except sections explicitly marked as non-normative, examples, and notes. Examples in this specification are introduced with the words “for example”.

## Concepts and Terminology


