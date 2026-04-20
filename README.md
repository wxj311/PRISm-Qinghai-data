# PRISM64 public-release package

This package was prepared from the uploaded analytical dataset for the PRISm study in the western Qinghai plateau region. The manuscript describes a screening dataset of 5,500 adult residents with questionnaire, vital sign, laboratory, and spirometry variables. fileciteturn10file0

## Files
- `prism64_standardized_numeric.csv`: analysis-ready dataset with standardized English snake_case variable names and a de-identified `study_id`.
- `prism64_standardized_labeled.csv`: same data with human-readable labels for categorical variables.
- `data_dictionary.csv`: variable definitions, units, and code mappings.
- `qc_review_flags.csv`: records/variables that merit manual review before public release.
- `PRISM64_standardized_package.xlsx`: Excel workbook containing the same content on separate sheets.

## Standardization steps
1. Added a de-identified record identifier (`study_id`).
2. Renamed all columns to English snake_case.
3. Preserved the original analytical values except for four mixed-unit columns where values recorded as percentages were converted to fractions when `value > 1`:
   - `lymphocyte_fraction`
   - `eosinophil_fraction`
   - `hematocrit_fraction`
   - `plateletcrit_fraction`
4. Preserved binary coding as `0/1` in the numeric file and mapped them to labels in the labeled file.
5. No direct personal identifiers were present in the uploaded CSV. The consent materials and editor letter indicate that any public release should be de-identified before sharing. fileciteturn10file18 fileciteturn10file11

## Source-derived coding
- `sex`: 0=female, 1=male, inferred from Table 1 counts. fileciteturn10file15
- `ethnicity`: 0=other ethnic minority, 1=Han, 2=Hui, 3=Tibetan, inferred from Table 1 counts. fileciteturn10file15
- Residential altitude values are 2850, 2940, and 3176 meters. fileciteturn10file14
- The manuscript lists the variables collected and their intended meanings. fileciteturn10file0

## Important review note
The QC file flags values that appear inconsistent with the manuscript inclusion range or typical lab units. I did **not** automatically correct those records, because that would require source verification. Review `qc_review_flags.csv` before uploading to GitHub.

## Suggested repository structure
```text
data/
  prism64_standardized_numeric.csv
  prism64_standardized_labeled.csv
  data_dictionary.csv
  qc_review_flags.csv
PRISM64_standardized_package.xlsx
README.md
```

## Suggested Data availability statement
> The de-identified dataset, data dictionary, and QC notes supporting the findings of this study are publicly available in the GitHub repository “[REPOSITORY NAME]” at [PERSISTENT LINK].

