---
name: Bug in your system
about: Only OpenCore and Lilu configurations are supported.
title: ''
labels: ''
assignees: ''

---

Please stop and read this carefully. Otherwise your issue will be left **unanswered** and **closed**.

* Only the latest released versions of OpenCore, Lilu, and other KEXTs are supported.
* Bug reports involving Chameleon, Clover, Ozmozis or alike are not accepted.
* Include your `EFI` directory with OpenCore.
* Include OpenCore DEBUG log (refer to `Target` in [Configuration.pdf](https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/Configuration.pdf) or here: [OpenCore Debugging](https://dortania.github.io/OpenCore-Desktop-Guide/troubleshooting/debug.html)).
* Include Lilu DEBUG log (refer to `-liludbgall liludump=60` boot arguments in Lilu's [README](https://github.com/acidanthera/Lilu/blob/master/README.md)).


When to use issue [Acidanthera's tracker](https://github.com/acidanthera/bugtracker):

* You have new resources or patches to add but cannot make a pull request
* You have kernel panics, crashes, hangs and believe it is not a configuration issue
* You want to discuss technical or legal stuff

_If you have a kernel panic, please ensure that you have a DEBUG version of the extension and you have `-v keepsyms=1 debug=0x100` boot arguments added. On 10.13 or higher to avoid kext names scrolling over the panic log you should also set `PanicNoKextDump=YES` in OpenCore. Use `ApplePanic=YES` for write a kernel panic log to file._
