# XOSC to Scenic Converter

## Overview

This tool converts OpenSCENARIO (.xosc) files into Scenic 3 scenarios compatible with the MetaDrive simulator.

It parses XML-based driving scenarios and generates executable Scenic scripts including:

* Entities (ego + NPCs)
* Behaviors
* Speed profiles
* Weather conditions
* Map configuration

---

## Features

* Works on generic OpenSCENARIO files
* Automatic ego vehicle detection
* Extracts waypoints and routes
* Converts speed profiles into Scenic behaviors
* Supports weather and time-of-day
* Generates MetaDrive-compatible Scenic code

---

## Installation

```bash
git clone https://github.com/your-username/xosc-to-scenic.git
cd xosc-to-scenic
```

---

## Usage

### Basic usage:

```bash
python xosc_to_scenic.py input.xosc
```

### Custom output:

```bash
python xosc_to_scenic.py input.xosc output.scenic
```

---

## Example

Input:

```
scenario.xosc
```

Output:

```
scenario.scenic
```

---

## How It Works

1. Parses OpenSCENARIO XML
2. Extracts entities, behaviors, environment
3. Builds internal scenario representation
4. Generates Scenic 3 script for MetaDrive

---

## Limitations

* Waypoint mapping may not perfectly align with MetaDrive lanes
* Limited support for non-vehicle entity types
* Complex behaviors may require manual adjustment

---

## Future Improvements

* Better lane alignment
* Support for more entity types
* Improved behavior generation

---

## Author

Ayaz Ahmed

---

## License

MIT License
