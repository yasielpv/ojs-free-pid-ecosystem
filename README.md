# OJS Free PID Ecosystem

An open-source ecosystem of plugins for implementing free persistent identifiers in Open Journal Systems (OJS).

## Overview

This repository provides a unified distribution of three interoperable plugins that enable the assignment and resolution of persistent identifiers without relying on commercial infrastructures.

The ecosystem supports:

- ARK (Archival Resource Key)
- PURL (Persistent Uniform Resource Locator)
- Internal resolution of multiple PID types

## Components

### 1. ARK Public Identifier Plugin
Generates and manages ARK identifiers for:
- Issues
- Articles
- Galleys

### 2. PURL Public Identifier Plugin
Provides PURL-based identifiers for journal content.

### 3. PubId Resolver Gateway Plugin
Acts as a resolver for persistent identifiers within OJS.

Supports:
- ARK
- PURL
- DOI
- URN

## Key Features

- Fully integrated with OJS editorial workflow
- Plugin-based architecture (no core modifications required)
- Support for multiple identifier schemes
- Local and external PID resolution
- Compatible with OJS 3.1 and 3.2

## Installation

Plugins can be installed using:

### Option 1: Plugin Gallery (Recommended)
1. Go to:
   - Website > Plugins > Plugin Gallery
2. Search for:
   - ARK
   - PURL
   - PubId Resolver
3. Install and activate each plugin

### Option 2: Manual Installation

1. Download the plugins from releases
2. Go to:
   - Website > Plugins > Installed Plugins
3. Click "Upload a New Plugin"
4. Activate the plugins

## Configuration

After installation:

1. Go to plugin settings
2. Configure:
   - Identifier assignment (issues, articles, galleys)
   - Prefix (NAAN for ARK)
   - Suffix patterns
   - Resolver URL

Identifiers can be assigned automatically or manually.

## Resolver Usage

The resolver is accessible through: /index.php/journal/gateway/plugin/pubIdResolver/PID

Examples:

- ARK: /gateway/plugin/pubIdResolver/ark:/12345/abc
- DOI: /gateway/plugin/pubIdResolver/10.1234/example


## Impact

The ecosystem is actively used by scientific journals in multiple countries across Latin America, Europe, Africa, and Asia.

It enables journals to implement persistent identifiers without incurring operational costs, supporting sustainable open-access publishing.

## Contributing

Contributions are welcome. Please open issues or submit pull requests.

## Authors

- Yasiel Pérez Vera

## Acknowledgements

Special thanks to the ARK community and contributors supporting open persistent identifier infrastructures.

## License

GNU GPL v3
