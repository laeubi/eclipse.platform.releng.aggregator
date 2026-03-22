# JUnit Version Range Audit

This directory contains audit reports for missing version ranges on JUnit bundles and package imports across the Eclipse Platform repository and all its submodules.

## Overview

As part of the JUnit 6 migration effort, we need to ensure that all MANIFEST.MF files have proper version ranges specified for JUnit-related bundles and packages. Missing version ranges can lead to compatibility issues when JUnit versions change.

## Reports

### JUNIT_VERSION_RANGE_AUDIT.md
A comprehensive markdown report that:
- Lists all 119 issues found across 8 repositories
- Groups issues by repository and bundle
- Provides detailed information about each missing version range
- Includes recommendations for fixing the issues

### JUNIT_VERSION_RANGE_AUDIT.csv
A CSV file containing all issues in a tabular format, useful for:
- Importing into spreadsheet applications
- Tracking progress as issues are fixed
- Filtering and sorting by repository or issue type

## Summary of Findings

- **Total MANIFEST.MF files scanned:** 1,165
- **Total issues found:** 119
- **Affected repositories:** 8

### Issues by Repository

| Repository | Issues |
|------------|--------|
| eclipse.jdt.ui | 42 |
| eclipse.pde | 29 |
| Main Repository (eclipse.platform.releng) | 15 |
| eclipse.platform.ui | 12 |
| eclipse.platform | 10 |
| equinox | 5 |
| eclipse.jdt.core | 4 |
| eclipse.jdt.debug | 2 |

## How to Fix

### For Require-Bundle entries
Add the `bundle-version` attribute with an appropriate version range:

```
# Before:
Require-Bundle: org.junit

# After:
Require-Bundle: org.junit;bundle-version="[4.13.0,5.0.0)"
```

### For Import-Package entries
Add the `version` attribute with an appropriate version range:

```
# Before:
Import-Package: org.junit.jupiter.api

# After:
Import-Package: org.junit.jupiter.api;version="[5.8.0,6.0.0)"
```

## Recommended Approach

1. Address issues repository by repository (not all at once)
2. Start with repositories that have fewer issues to build momentum
3. Create separate PRs for each repository/submodule
4. Test thoroughly after adding version ranges
5. Update this tracking document as issues are resolved

## Repository Links

- [eclipse.jdt.core](https://github.com/eclipse-jdt/eclipse.jdt.core) - 4 issues
- [eclipse.jdt.debug](https://github.com/eclipse-jdt/eclipse.jdt.debug) - 2 issues
- [eclipse.jdt.ui](https://github.com/eclipse-jdt/eclipse.jdt.ui) - 42 issues
- [eclipse.pde](https://github.com/eclipse-pde/eclipse.pde) - 29 issues
- [eclipse.platform](https://github.com/eclipse-platform/eclipse.platform) - 10 issues
- [eclipse.platform.ui](https://github.com/eclipse-platform/eclipse.platform.ui) - 12 issues
- [equinox](https://github.com/eclipse-equinox/equinox) - 5 issues
- [Main Repository](https://github.com/laeubi/eclipse.platform.releng.aggregator) - 15 issues

## Reference

For examples of properly versioned JUnit imports, see:
- https://github.com/eclipse-platform/eclipse.platform.releng.aggregator/pull/3431
