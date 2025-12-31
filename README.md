# Microsoft Air-Related Repositories Issue Analysis

This repository contains an analysis of Microsoft Air-related repositories to identify open issues that lack proper labeling.

## Analysis Summary

I analyzed 11 Microsoft repositories containing "Air" in their names and counted the number of open issues that have no labels assigned. This data helps identify repositories that may need better issue management practices.

## Results

The analysis revealed significant variation in issue labeling practices across repositories:

| Repository | Open Issues Without Labels |
|------------|---------------------------|
| AirSim | 679 |
| ContosoAir | 0 |
| AirSim-NeurIPS2019-Drone-Racing | 27 |
| AirSim-Drone-Racing-VAE-Imitation | 3 |
| AirSim-Drone-Racing-Lab | 15 |
| AIReferenceArchitectures | 6 |
| AirSim-Drone-Racing-Lab-Source | 2 |
| apache-airflow-microsoft-fabric-plugin | 10 |
| airflow-providers-microsoft-fabric | 0 |
| AirbandData | 1 |
| woodgrove-airline | 2 |

## Key Findings

1. **AirSim** has the highest number of unlabeled issues (679), which is concerning given its popularity and active development.

2. Several smaller repositories have good labeling practices with 0-3 unlabeled issues.

3. Some repositories appear to be inactive or archived, which may explain the lack of labeling efforts.

## Recommendations

1. **AirSim repository** should prioritize implementing better issue labeling practices given the large number of unlabeled issues.

2. Consider implementing automated labeling workflows or issue templates to improve organization.

3. Regular issue triage and labeling should be part of repository maintenance practices.

## Methodology

The analysis was performed using the GitHub API to search for repositories under the 'microsoft' organization containing "Air" in their names, then counting open issues without labels for each repository.

## Data File

The raw data is available in `microsoft_air_no_label_report.json` in the format:
```json
{
  "repository_name": open_issue_count,
  ...
}
```