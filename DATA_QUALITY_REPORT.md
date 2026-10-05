# Data Quality Report

## Missing Values
- PoolQC: filled with "None" because missing means no pool.
- MiscFeature: filled with "None" because missing means no feature.
- Alley: filled with "None" because missing means no alley.
- Fence: filled with "None" because missing means no fence.
- FireplaceQu: filled with "None" because missing means no fireplace.
- Garage columns: filled with "None" or 0 because missing means no garage.
- Basement columns: filled with "None" because missing means no basement.
- MasVnrType: filled with "None" because missing means no veneer.
- MasVnrArea: filled with 0 because missing means no veneer.
- Electrical: filled with mode because only 1 missing, likely not recorded.
- LotFrontage: filled with median because likely not recorded.

## Duplicates
- 0 exact duplicates.
- 0 near-duplicates.

## Outliers
- GrLivArea: flagged outliers >4000. Real extreme values.
- LotArea: kept outliers. Genuine large lots.
- TotalBsmtSF: kept outliers. Genuine large basements.

## Type Corrections
- MSSubClass converted from number to string because it is a category code.

## Leakage Note
- Any future imputation must use training data only.

## Target Note
- SalePrice was not used in any cleaning decision.
