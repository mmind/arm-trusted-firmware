Security Center
===============

Security Disclosures
--------------------

We disclose all security vulnerabilities we find or are advised about that are
relevant for ARM Trusted Firmware (TF). We encourage responsible disclosure of
vulnerabilities and inform users as best we can about all possible issues.

We disclose TF vulnerabilities as Security Advisories. These are listed at the
bottom of this page and announced as issues in the `GitHub issue tracker`_ with
the "security-advisory" tag. You can receive notification emails for these by
watching that project.

Found a Security Issue?
-----------------------

Although we try to keep TF secure, we can only do so with the help of the
community of developers and security researchers.

If you think you have found a security vulnerability, please *do not* report it
in the `GitHub issue tracker`_. Instead send an email to
trusted-firmware-security@arm.com

Please include:

* Trusted Firmware version (or commit) affected

* A description of the concern or vulnerability

* Details on how to replicate the vulnerability, including:

  - Configuration details

  - Proof of concept exploit code

  - Any additional software or tools required

We recommend using `this PGP/GPG key`_ for encrypting the information. This key
is also available at http://keyserver.pgp.com and LDAP port 389 of the same
server. The fingerprint for this key is:

::

    1309 2C19 22B4 8E87 F17B FE5C 3AB7 EFCB 45A0 DFD0

If you would like replies to be encrypted, please provide your public key.

Please give us the time to respond to you and fix the vulnerability before going
public. We do our best to respond and fix any issues quickly. We also need to
ensure providers of products that use TF have a chance to consider the
implications of the vulnerability and its remedy.

Afterwards, we encourage you to write-up your findings about the TF source code.

Attribution
-----------

We will name and thank you in the ``change-log.rst`` distributed with the source
code and in any published security advisory.

Security Advisories
-------------------

+-----------+------------------------------------------------------------------+
| ID        | Title                                                            |
+===========+==================================================================+
| `TFV-1`_  | Malformed Firmware Update SMC can result in copy of unexpectedly |
|           | large data into secure memory                                    |
+-----------+------------------------------------------------------------------+
| `TFV-2`_  | Enabled secure self-hosted invasive debug interface can allow    |
|           | normal world to panic secure world                               |
+-----------+------------------------------------------------------------------+
| `TFV-3`_  | RO memory is always executable at AArch64 Secure EL1             |
+-----------+------------------------------------------------------------------+
| `TFV-4`_  | Malformed Firmware Update SMC can result in copy or              |
|           | authentication of unexpected data in secure memory in AArch32    |
|           | state                                                            |
+-----------+------------------------------------------------------------------+
| `TFV-5`_  | Not initializing or saving/restoring PMCR_EL0 can leak secure    |
|           | world timing information                                         |
+-----------+------------------------------------------------------------------+
| `TFV-6`_  | Arm Trusted Firmware exposure to speculative processor           |
|           | vulnerabilities using cache timing side-channels                 |
+-----------+------------------------------------------------------------------+
| `TFV-7`_  | Trusted Firmware-A exposure to cache speculation vulnerability   |
|           | Variant 4                                                        |
+-----------+------------------------------------------------------------------+
| `TFV-8`_  | Not saving x0 to x3 registers can leak information from one      |
|           | Normal World SMC client to another                               |
+-----------+------------------------------------------------------------------+

.. _GitHub issue tracker: https://github.com/ARM-software/tf-issues/issues
.. _this PGP/GPG key: security-reporting.asc
.. _TFV-1: ./security_advisories/security-advisory-tfv-1.rst
.. _TFV-2: ./security_advisories/security-advisory-tfv-2.rst
.. _TFV-3: ./security_advisories/security-advisory-tfv-3.rst
.. _TFV-4: ./security_advisories/security-advisory-tfv-4.rst
.. _TFV-5: ./security_advisories/security-advisory-tfv-5.rst
.. _TFV-6: ./security_advisories/security-advisory-tfv-6.rst
.. _TFV-7: ./security_advisories/security-advisory-tfv-7.rst
.. _TFV-8: ./security_advisories/security-advisory-tfv-8.rst
