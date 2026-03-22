# JUnit Version Range Audit Report
## Summary
This report identifies MANIFEST.MF files in the Eclipse Platform repository and its submodules that have missing version ranges on JUnit bundles and package imports.
**Total MANIFEST.MF files scanned:** 1165
**Total issues found:** 119
**Affected repositories:** 8

## Overview by Repository
| Repository | Issues |
|------------|--------|
| [Main Repository (eclipse.platform.releng)](https://github.com/laeubi/eclipse.platform.releng.aggregator) | 15 |
| [eclipse.jdt.core](https://github.com/eclipse-jdt/eclipse.jdt.core) | 4 |
| [eclipse.jdt.debug](https://github.com/eclipse-jdt/eclipse.jdt.debug) | 2 |
| [eclipse.jdt.ui](https://github.com/eclipse-jdt/eclipse.jdt.ui) | 42 |
| [eclipse.pde](https://github.com/eclipse-pde/eclipse.pde) | 29 |
| [eclipse.platform](https://github.com/eclipse-platform/eclipse.platform) | 10 |
| [eclipse.platform.ui](https://github.com/eclipse-platform/eclipse.platform.ui) | 12 |
| [equinox](https://github.com/eclipse-equinox/equinox) | 5 |

## Detailed Issues by Repository

### [Main Repository (eclipse.platform.releng)](https://github.com/laeubi/eclipse.platform.releng.aggregator)
**Total issues in this repository:** 15

#### `eclipse.platform.releng/bundles/org.eclipse.ant.optional.junit/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.ant.optional.junit`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform.releng/bundles/org.eclipse.releng.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.releng.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform.releng/bundles/org.eclipse.test.performance/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.test.performance`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

**Missing `version` on Import-Package:**
- `org.junit.jupiter.api`
- `org.junit.platform.suite.api`

#### `eclipse.platform.releng/bundles/org.eclipse.test/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.test`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

**Missing `version` on Import-Package:**
- `org.junit.jupiter.api`
- `org.junit.platform.engine`
- `org.junit.platform.engine.discovery`
- `org.junit.platform.engine.reporting`
- `org.junit.platform.engine.support.descriptor`
- `org.junit.platform.launcher`
- `org.junit.platform.launcher.core`
- `org.junit.platform.commons`
- `org.junit.jupiter.engine`

### [eclipse.jdt.core](https://github.com/eclipse-jdt/eclipse.jdt.core)
**Total issues in this repository:** 4

#### `eclipse.jdt.core/org.eclipse.jdt.apt.pluggable.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.jdt.apt.pluggable.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.jdt.core/org.eclipse.jdt.apt.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.jdt.apt.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.jdt.core/org.eclipse.jdt.compiler.apt.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.jdt.compiler.apt.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.jdt.core/org.eclipse.jdt.compiler.tool.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.jdt.compiler.tool.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

### [eclipse.jdt.debug](https://github.com/eclipse-jdt/eclipse.jdt.debug)
**Total issues in this repository:** 2

#### `eclipse.jdt.debug/org.eclipse.jdt.debug.jdi.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.jdt.debug.jdi.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.jdt.debug/org.eclipse.jdt.debug.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.jdt.debug.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

### [eclipse.jdt.ui](https://github.com/eclipse-jdt/eclipse.jdt.ui)
**Total issues in this repository:** 42

#### `eclipse.jdt.ui/org.eclipse.jdt.text.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.jdt.text.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

**Missing `version` on Import-Package:**
- `org.junit.jupiter.api`
- `org.junit.jupiter.api.extension`
- `org.junit.jupiter.migrationsupport`
- `org.junit.jupiter.migrationsupport.conditions`
- `org.junit.jupiter.migrationsupport.rules`
- `org.junit.jupiter.params`
- `org.junit.jupiter.params.aggregator`
- `org.junit.jupiter.params.converter`
- `org.junit.jupiter.params.provider`
- `org.junit.jupiter.params.support`
- `org.junit.platform.suite.api`
- `org.junit.platform.suite.commons`
- `org.junit.platform.suite.engine`

#### `eclipse.jdt.ui/org.eclipse.jdt.ui.tests.refactoring/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.jdt.ui.tests.refactoring`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

**Missing `version` on Import-Package:**
- `org.junit.jupiter.api`
- `org.junit.jupiter.api.extension`
- `org.junit.jupiter.migrationsupport`
- `org.junit.jupiter.migrationsupport.conditions`
- `org.junit.jupiter.migrationsupport.rules`
- `org.junit.jupiter.params`
- `org.junit.jupiter.params.aggregator`
- `org.junit.jupiter.params.converter`
- `org.junit.jupiter.params.provider`
- `org.junit.jupiter.params.support`
- `org.junit.platform.suite.api`
- `org.junit.platform.suite.commons`
- `org.junit.platform.suite.engine`

#### `eclipse.jdt.ui/org.eclipse.jdt.ui.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.jdt.ui.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

**Missing `version` on Import-Package:**
- `org.junit.jupiter.api`
- `org.junit.jupiter.api.extension`
- `org.junit.jupiter.migrationsupport`
- `org.junit.jupiter.migrationsupport.conditions`
- `org.junit.jupiter.migrationsupport.rules`
- `org.junit.jupiter.params`
- `org.junit.jupiter.params.aggregator`
- `org.junit.jupiter.params.converter`
- `org.junit.jupiter.params.provider`
- `org.junit.jupiter.params.support`
- `org.junit.platform.suite.api`
- `org.junit.platform.suite.commons`
- `org.junit.platform.suite.engine`

### [eclipse.pde](https://github.com/eclipse-pde/eclipse.pde)
**Total issues in this repository:** 29

#### `eclipse.pde/apitools/org.eclipse.pde.api.tools.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.pde.api.tools.tests`

**Missing `version` on Import-Package:**
- `junit.framework`
- `org.junit`
- `org.junit.runner`
- `org.junit.runners`

#### `eclipse.pde/build/org.eclipse.pde.build.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.pde.build.tests`

**Missing `version` on Import-Package:**
- `org.junit`
- `org.junit.runner`
- `org.junit.runners`

#### `eclipse.pde/ds/org.eclipse.pde.ds.annotations.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.pde.ds.annotations.tests`

**Missing `version` on Import-Package:**
- `org.junit`
- `org.junit.runner`
- `org.junit.runners`

#### `eclipse.pde/ua/org.eclipse.pde.ua.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.pde.ua.tests`

**Missing `version` on Import-Package:**
- `org.junit`
- `org.junit.runner`
- `org.junit.runners`

#### `eclipse.pde/ui/org.eclipse.pde.genericeditor.extension.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.pde.genericeditor.extension.tests`

**Missing `version` on Import-Package:**
- `org.junit`
- `org.junit.runner`
- `org.junit.runners`

#### `eclipse.pde/ui/org.eclipse.pde.junit.runtime.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.pde.junit.runtime.tests`

**Missing `version` on Import-Package:**
- `org.junit`
- `org.junit.rules`
- `org.junit.runner`
- `org.junit.runners`

#### `eclipse.pde/ui/org.eclipse.pde.ui.templates.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.pde.ui.templates.tests`

**Missing `version` on Import-Package:**
- `org.junit`
- `org.junit.runner`
- `org.junit.runners`

#### `eclipse.pde/ui/org.eclipse.pde.ui.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.pde.ui.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit.source`

**Missing `version` on Import-Package:**
- `org.junit`
- `org.junit.rules`
- `org.junit.runner`
- `org.junit.runners`
- `org.junit.runners.model`

### [eclipse.platform](https://github.com/eclipse-platform/eclipse.platform)
**Total issues in this repository:** 10

#### `eclipse.platform/ant/org.eclipse.ant.tests.ui/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.ant.tests.ui`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform/debug/org.eclipse.debug.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.debug.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform/debug/org.eclipse.debug.ui.launchview.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.debug.ui.launchview.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform/resources/tests/org.eclipse.core.tests.resources.saveparticipant1/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.core.tests.resources.saveparticipant1`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform/resources/tests/org.eclipse.core.tests.resources.saveparticipant2/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.core.tests.resources.saveparticipant2`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform/resources/tests/org.eclipse.core.tests.resources.saveparticipant3/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.core.tests.resources.saveparticipant3`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform/resources/tests/org.eclipse.core.tests.resources/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.core.tests.resources`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform/runtime/tests/org.eclipse.core.tests.harness/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.core.tests.harness`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform/runtime/tests/org.eclipse.core.tests.runtime/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.core.tests.runtime`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform/team/examples/org.eclipse.compare.examples.xml/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.compare.examples.xml`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

### [eclipse.platform.ui](https://github.com/eclipse-platform/eclipse.platform.ui)
**Total issues in this repository:** 12

#### `eclipse.platform.ui/tests/org.eclipse.jface.tests.databinding.conformance/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.jface.tests.databinding.conformance`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform.ui/tests/org.eclipse.jface.tests.databinding/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.jface.tests.databinding`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform.ui/tests/org.eclipse.ltk.core.refactoring.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.ltk.core.refactoring.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform.ui/tests/org.eclipse.ltk.ui.refactoring.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.ltk.ui.refactoring.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform.ui/tests/org.eclipse.ui.ide.application.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.ui.ide.application.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform.ui/tests/org.eclipse.ui.tests.browser/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.ui.tests.browser`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform.ui/tests/org.eclipse.ui.tests.harness/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.ui.tests.harness`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform.ui/tests/org.eclipse.ui.tests.navigator/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.ui.tests.navigator`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform.ui/tests/org.eclipse.ui.tests.performance/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.ui.tests.performance`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform.ui/tests/org.eclipse.ui.tests.rcp/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.ui.tests.rcp`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform.ui/tests/org.eclipse.ui.tests.views.properties.tabbed/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.ui.tests.views.properties.tabbed`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `eclipse.platform.ui/tests/org.eclipse.ui.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.ui.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

### [equinox](https://github.com/eclipse-equinox/equinox)
**Total issues in this repository:** 5

#### `equinox/bundles/org.eclipse.equinox.common.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.equinox.common.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `equinox/bundles/org.eclipse.equinox.ds.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.equinox.ds.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `equinox/bundles/org.eclipse.equinox.preferences.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.equinox.preferences.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `equinox/bundles/org.eclipse.equinox.security.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.equinox.security.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

#### `equinox/bundles/org.eclipse.osgi.tests/META-INF/MANIFEST.MF`
**Bundle:** `org.eclipse.osgi.tests`

**Missing `bundle-version` on Require-Bundle:**
- `org.junit`

## Recommendations

### For Require-Bundle entries
Add `bundle-version` attribute with appropriate version range. Examples:
```
Require-Bundle: org.junit;bundle-version="[4.13.0,5.0.0)"
Require-Bundle: org.junit;bundle-version="3.8.1"
```

### For Import-Package entries
Add `version` attribute with appropriate version range. Examples:
```
Import-Package: org.junit.jupiter.api;version="[5.8.0,6.0.0)"
Import-Package: org.junit.platform.engine;version="[1.8.0,2.0.0)"
```

## Notes
- This audit is part of the JUnit 6 migration effort
- Version ranges help ensure compatibility and prevent issues when JUnit versions change
- Each repository should be addressed individually to maintain proper version control
