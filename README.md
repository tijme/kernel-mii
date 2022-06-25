<p align="center">
    <img src="https://raw.githubusercontent.com/tijme/kernel-mii/master/.github/logo.png" width="450"/>
</p>
<p align="center">
    <a href="https://github.com/tijme/kernel-mii/blob/master/LICENSE.md"><img src="https://raw.finnwea.com/shield/?firstText=Source&secondText=Licensed" /></a>
    <br/>
    <b>Cobalt Strike Beacon Object File foundation for kernel exploitation using CVE-2021-21551.</b>
    <br/>
    <sup>Built by <a href="https://www.linkedin.com/in/tijme/">Tijme</a> at <a href="https://github.com/NorthwaveSecurity">Northwave Security</a>. Credits to <a href="https://github.com/lldre">Alex</a> for teaching me!</sup>
    <br/>
</p>

## Description

This is a Cobalt Strike (CS) Beacon Object File (BOF) which exploits CVE-2021-21551. It only overwrites the beacon process token with the system process token. But this BOF is mostly just a good foundation for further kernel exploitation via CS.

## Limitations

* If the vulnerable driver is not installed, you need to be local admin to install it.

## Todo

* Load the vulnerable driver from memory instead of from disk.
* Delete the vulnerable driver if it was not preinstalled.

## Issues

Issues or new features can be reported via the [issue tracker](https://github.com/tijme/kernel-mii/issues). Please make sure your issue or feature has not yet been reported by anyone else before submitting a new one.

## License

Copyright (c) 2022 Tijme Gommers & Northwave Security. All rights reserved. View [LICENSE.md](https://github.com/tijme/kernel-mii/blob/master/LICENSE.md) for the full license.