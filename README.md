# Candid Core Framework

**A conceptual framework to enhance geospatial catalogs with "Data Candor" - radical honesty, transparency, and user-centric evaluation.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Contributions Welcome](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](CONTRIBUTING.md)

## What is the Candid Core Framework?

The **Candid Core Framework** addresses a fundamental problem in geospatial data: the "**Metadata Mirage**" - when technical metadata exists but crucial context about usability, limitations, and fitness for purpose remains hidden.

While we have abundant geospatial data from satellites, sensors, and models, finding the *right* dataset for your specific needs remains challenging. Current metadata standards tell us *what* and *where* data exists, but often fail to communicate *when* and *why* we should use a particular dataset.

The Candid Core Framework aims to bridge this gap by providing a structured approach to capture the evaluative information experienced users and data creators naturally share about datasets, making this wisdom accessible to all users.

## Key Categories

The Candid Core Framework organizes metadata into five main areas:

### Suitability & Limitations
- **Suitability Summary:** Concise overview of dataset strengths and weaknesses
- **Application Limitations:** Known constraints where using the dataset might lead to inaccurate results
- **Data Quality Metrics:** Quantitative measures of accuracy and uncertainty
- **Known Gaps / Future Work:** Recognized gaps in coverage, methodology, or validation

### Context & Definitions
- **Key Term Definitions:** Critical terms used within the dataset and their specific meanings
- **Methodology Summary:** Overview of algorithms, input data sources, and processing steps
- **Ethics / Bias:** Potential ethical implications or known biases in the data
- **Vibes / Social Context:** Informal context, cultural significance, or community ethos

### Use Cases & Target Users
- **Target Audience:** Primary intended users or groups
- **Recommended Expertise:** Technical skill or domain knowledge needed for effective use
- **Suggested Uses:** Recommended applications for the dataset
- **Example Uses:** Teaching resources, community resources, applications, APIs, and creative uses

### Provenance & Relationships
- **Review Method:** Nature of quality assessment or review the dataset has undergone
- **Candid Core Curation Method:** How the evaluative metadata was populated
- **Related and Competitor Datasets:** Alternatives and complementary datasets
- **Comparison Notes:** Direct comparisons to key alternatives

### Lifecycle & Access
- **Support Status:** Maintenance level and expected longevity
- **Curation/Update Philosophy:** Approach to updates and incorporating feedback
- **Data Access & Providers:** Available access points and ease of access
- **User Feedback Channel:** Designated contact for reporting issues or suggesting improvements
- **Carbon/Energy Cost:** Environmental footprint associated with the dataset

## Implementation

The Candid Core Framework doesn't replace existing metadata standards like STAC (SpatioTemporal Asset Catalog) but complements them with user-focused evaluative information. 

While Large Language Models could help standardize these insights, the Framework emphasizes human curation and expertise to ensure accuracy, relevance, and trustworthiness.

## Why It Matters

Moving beyond simply connecting users to data and beginning to connect them to actionable knowledge, we can fundamentally transform how Earth observation data creates value for science and society.

## Contributing

We welcome contributions to the Candid Core Framework! Please see our [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

The Candid Core Framework emerged from discussions at the AGU Retreat in Washington, D.C., preceding the 2024 American Geophysical Union Fall Meeting. It builds on the foundation of cloud-native geospatial data catalogs and standardized metadata to address the fundamental challenge of data evaluability.
