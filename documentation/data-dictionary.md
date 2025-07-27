# AP210 Research Data Dictionary

## File Format Specifications

### AP210 STEP Files
- **Extensions**: `.stp`, `.210`, `.step`
- **Standard**: ISO 10303-210 Electronic Assembly, Interconnect and Packaging Design
- **Content**: 3D geometric models, assembly structures, electrical connectivity, material properties

### IDF Files  
- **Extensions**: `.idf`, `.brd`, `.lib`
- **Standard**: Intermediate Data Format for PCB design
- **Content**: Board outline, component placement, electrical connectivity

### SPICE Files
- **Extensions**: `.cir`, `.sp`, `.net`
- **Standard**: Simulation Program with Integrated Circuit Emphasis
- **Content**: Circuit netlists, simulation parameters, analysis directives

## Data Structure

### Directory Organization
```
datasets/
├── nist-ap210-cfd/         # CFD analysis data
├── nist-ap210-gdt/         # GDT tolerance data  
├── nist-ap210-spice/       # SPICE integration data
├── pdes-ap210viewer/       # Viewer tool data
└── pdes-idf2ap210/         # Format conversion data
```

### Naming Conventions
- Test cases: `test_*.210`, `test_*.stp`
- Reference designs: `ref_*.210`
- Example assemblies: `example_*.210`

## Metadata Fields
Common data attributes across all datasets:
- **Project**: Research project identifier
- **Organization**: NIST, PDES Inc.
- **Date**: Creation/modification date
- **Version**: Data version number
- **Description**: Human-readable description
- **Related**: Links to related datasets

## Usage Guidelines
- All data files are read-only archival versions
- For modification, copy to local environment
- Maintain attribution when redistributing
- Report issues via GitHub repository