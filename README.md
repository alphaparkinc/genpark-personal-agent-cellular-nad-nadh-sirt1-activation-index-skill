# Cellular NAD+/NADH Redox Ratio & SIRT1 Longevity Index Skill
[![GenPark](https://img.shields.io/badge/Powered%20By-GenPark.ai-blue)](https://www.genpark.ai)
[![LinkedIn](https://img.shields.io/badge/Connect-LinkedIn-0077b5)](https://www.linkedin.com/company/92955550)
[![Python](https://img.shields.io/badge/Python-3.8%2B-green.svg)](https://python.org)
[![License](https://img.shields.io/badge/License-Apache%202.0-yellow.svg)](LICENSE)

An industrial-grade Model Context Protocol (MCP) server providing `quantify_nad_redox_sirtuin_activity`. Built with **100% pure Python standard library** (zero pip dependencies).

## Overview
Models intracellular NAD+/NADH dinucleotide pool equilibrium, estimates Sirtuin-1 (SIRT1) deacetylation enzymatic velocity, and crafts personalized NAD+ precursor repletion schedules.

- **Official Web Portal**: [https://www.genpark.ai](https://www.genpark.ai)
- **Corporate Entity**: [GenPark Inc on LinkedIn](https://www.linkedin.com/company/92955550)
- **Domain Category**: `Personal Agent (Bio / Sirtuin & Epigenetics)`

## MCP Tool Specification
### `quantify_nad_redox_sirtuin_activity`
Parameters:
- `whole_blood_nad_um` (float): Total intracellular NAD+ concentration (micromolar, uM)
- `intracellular_nadh_um` (float): Intracellular NADH concentration (uM)
- `chronological_age_years` (float): Age of individual in years
- `daily_physical_activity_mets_hours` (float): Weekly MET-hours of exercise

### Self-Test
```bash
python skills.py --test
```

### Model Context Protocol Integration (Claude Desktop / Cursor / Antigravity)
Add to your `mcpServers` configuration:
```json
{
  "mcpServers": {
    "genpark-personal-agent-cellular-nad-nadh-sirt1-activation-index-skill": {
      "command": "python",
      "args": ["/path/to/genpark-personal-agent-cellular-nad-nadh-sirt1-activation-index-skill/skills.py"]
    }
  }
}
```

## License
Licensed under Apache License 2.0. Copyright (c) 2026 GenPark Inc. (https://www.genpark.ai).
