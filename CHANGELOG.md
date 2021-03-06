## 0.6.0 (2014-09-11)

  - Fix schema bug preventing use of 'description', 'is_shared', 'dns_suffix' options
  - Upgrade dependency on vCloud Core to 0.11.0 which prevents plaintext
    passwords in FOG_RC. Please use tokens via vcloud-login as per
    the documentation: http://gds-operations.github.io/vcloud-tools/usage/

## 0.5.1 (2014-08-12)

  - Upgrade dependency on vCloud Core to 0.10.0 for parity with other vCloud
    Tools gems and prevent problems resolving dependencies.

## 0.5.0 (2014-08-08)

This release bumps the dependency to vCloud Core 0.9.0:

  - New vcloud-login tool for fetching session tokens without the need to
    store your password in a plaintext FOG_RC file.
  - Deprecate the use of :vcloud_director_password in a plaintext FOG_RC
    file. A warning will be printed to STDERR at load time. Please use
    vcloud-login instead.
  - This gem no longer directly references fog, instead using vCloud Core's
    API for its interaction with the vCloud API.

## 0.4.0 (2014-07-25)

  - Remove the command line option to enable fog mocking.
  - Add documentation for public API methods.

## 0.3.0 (2014-07-14)

Features:

  - `vcloud-net-launch --version` now only returns the version string
      and no usage information.

## 0.2.0 (2014-05-14)

Features:

  - Depend on version 0.3.0 of vcloud-core which introduces breaking changes to OrgVdcNetwork

## 0.1.0 (2014-04-30)

Features:

  - Depend on version 0.2.0 of vcloud-core which introduces breaking changes to namespacing

## 0.0.3 (2014-05-01)

  - Use pessimistic version dependency for vcloud-core

## 0.0.2 (2014-04-22)

Bugfixes:

  - Requires vCloud Core v0.0.12 which fixes issue with progress bar falling over when progress is not returned

## 0.0.1 (2014-03-24)

  - First release of gem
