# @backstage/plugin-jenkins-backend

## 0.1.14

### Patch Changes

- c77c5c7eb6: Added `backstage.role` to `package.json`
- 377fce4677: The `DefaultJenkinsInfoProvider.fromConfig` now requires an implementation of the `CatalogApi` rather than a `CatalogClient` instance.
- Updated dependencies
  - @backstage/backend-common@0.10.8
  - @backstage/catalog-client@0.7.0
  - @backstage/catalog-model@0.10.0
  - @backstage/config@0.1.14

## 0.1.13

### Patch Changes

- Updated dependencies
  - @backstage/catalog-client@0.6.0
  - @backstage/backend-common@0.10.7

## 0.1.13-next.0

### Patch Changes

- Updated dependencies
  - @backstage/backend-common@0.10.7-next.0

## 0.1.12

### Patch Changes

- Updated dependencies
  - @backstage/backend-common@0.10.6

## 0.1.12-next.0

### Patch Changes

- Updated dependencies
  - @backstage/backend-common@0.10.6-next.0

## 0.1.11

### Patch Changes

- Updated dependencies
  - @backstage/backend-common@0.10.4
  - @backstage/config@0.1.13
  - @backstage/catalog-model@0.9.10
  - @backstage/catalog-client@0.5.5

## 0.1.11-next.0

### Patch Changes

- Updated dependencies
  - @backstage/backend-common@0.10.4-next.0
  - @backstage/config@0.1.13-next.0
  - @backstage/catalog-model@0.9.10-next.0
  - @backstage/catalog-client@0.5.5-next.0

## 0.1.10

### Patch Changes

- eb3fd85d3e: feature: add crumbIssuer option to Jenkins (optional) configuration, improve the UI to show a notification after executing the action re-build
- Updated dependencies
  - @backstage/backend-common@0.10.0
  - @backstage/catalog-client@0.5.3

## 0.1.9

### Patch Changes

- b055a6addc: Align on usage of `cross-fetch` vs `node-fetch` in frontend vs backend packages, and remove some unnecessary imports of either one of them
- Updated dependencies
  - @backstage/backend-common@0.9.12

## 0.1.8

### Patch Changes

- bab752e2b3: Change default port of backend from 7000 to 7007.

  This is due to the AirPlay Receiver process occupying port 7000 and preventing local Backstage instances on MacOS to start.

  You can change the port back to 7000 or any other value by providing an `app-config.yaml` with the following values:

  ```
  backend:
    listen: 0.0.0.0:7123
    baseUrl: http://localhost:7123
  ```

  More information can be found here: https://backstage.io/docs/conf/writing

- Updated dependencies
  - @backstage/backend-common@0.9.11

## 0.1.7

### Patch Changes

- e8a1c1afe2: Don't require a validation pattern for the Jenkins base URL.
- Updated dependencies
  - @backstage/backend-common@0.9.9
  - @backstage/catalog-client@0.5.1

## 0.1.6

### Patch Changes

- Updated dependencies
  - @backstage/catalog-model@0.9.4
  - @backstage/backend-common@0.9.6
  - @backstage/catalog-client@0.5.0

## 0.1.5

### Patch Changes

- Updated dependencies
  - @backstage/catalog-client@0.4.0
  - @backstage/catalog-model@0.9.3
  - @backstage/backend-common@0.9.4
  - @backstage/config@0.1.10

## 0.1.4

### Patch Changes

- 4c86555a2: Fix the case where lastBuild is null.
- Updated dependencies
  - @backstage/backend-common@0.9.0
  - @backstage/config@0.1.8

## 0.1.3

### Patch Changes

- efbb82dd3: Extract `JenkinsConfig` to make writing a custom `JenkinsInfoProvider` easier.
- Updated dependencies
  - @backstage/backend-common@0.8.10
  - @backstage/config@0.1.7

## 0.1.2

### Patch Changes

- eee05803a: Update `@backstage/backend-common` to `^0.8.6`
- Updated dependencies
  - @backstage/catalog-client@0.3.17
  - @backstage/backend-common@0.8.7
