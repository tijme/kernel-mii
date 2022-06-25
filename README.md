<p align="center">
    <img src="https://raw.githubusercontent.com/tijme/kernel-mii/master/.github/logo.png" width="450"/>
</p>
<p align="center">
    <a href="https://github.com/tijme/kernel-mii/blob/master/LICENSE.md"><img src="https://raw.finnwea.com/shield/?firstText=Source&secondText=Licensed" /></a>
    <br/>
    <b>Cobalt Strike Beacon Object File foundation for kernel exploitation using CVE-2021-21551.</b>
    <br/>
    <sup>Built by <a href="https://www.linkedin.com/in/tijme/">Tijme</a>. Credits to <a href="https://github.com/lldre">Alex</a> for teaching me! Made possible by <a href="https://northwave-security.com/">Northwave Security</a> <img src="https://raw.githubusercontent.com/tijme/kernel-mii/master/.github/northwave.png"/></sup>
    <br/>
</p>

## Description

This is a Cobalt Strike (CS) Beacon Object File (BOF) which exploits CVE-2021-21551. It only overwrites the beacon process token with the system process token. But this BOF is mostly just a good foundation for further kernel exploitation via CS.

<p align="center">
    <img src="https://raw.githubusercontent.com/tijme/kernel-mii/master/.github/output.png" />
</p>

## Usage

Clone this repository first. Then review the code, compile from source and use it in Cobalt Strike.

**Compiling**

	cl.exe /c .\KernelMii.c /Fo.\KernelMii.o

**Usage**

Load the `KernelMii.cna` script using the Cobalt Strike Script Manager. Then use the command below to execute the exploit.

    $ kernel_mii

## Limitations

* If the vulnerable driver is not installed, you need to be local admin to install it.

## Todo

* Load the vulnerable driver from memory instead of from disk.
* Delete the vulnerable driver if it was not preinstalled.
* Make the exploit stable & compatible with multiple Windows versions.

## Issues

Issues or new features can be reported via the [issue tracker](https://github.com/tijme/kernel-mii/issues). Please make sure your issue or feature has not yet been reported by anyone else before submitting a new one.

## License

Copyright (c) 2022 Tijme Gommers & Northwave Security. All rights reserved. View [LICENSE.md](https://github.com/tijme/kernel-mii/blob/master/LICENSE.md) for the full license.