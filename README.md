# Mutation Tester
This Plugin enables mutation testing in your IDE based on <a href="https://pitest.org">pitest.org</a>.

![build workflow](https://github.com/valantic/mutation-tester/actions/workflows/gradle-build.yml/badge.svg)
[![Software License](https://img.shields.io/badge/license-Apache%202-orange.svg?style=flat-square)](LICENSE.md)
[![HitCount](http://hits.dwyl.com/valantic/mutation-tester.svg?style=flat-square)](http://hits.dwyl.com/valantic/mutation-tester)

This package is developed by [valantic CEC Schweiz](https://www.valantic.com/).


## About
Mutation Testing is also called Fault-based testing strategy as it involves creating a fault in the program and it is a type of White Box Testing which is mainly used for Unit Testing.
When the application code changes, it should produce different results and cause the unit tests to fail. If a unit test does not fail in this situation, it may indicate an issue with the test suite.

This kind of testing helps you to produce better testing results, not only based on line coverage but also on mutation coverage. If less of your code can mutate, you can be sure to have a higher code quality.

This Plugin will help you as developer to run mutation tests easy and fast in your IDE without wasting time in configurations.

For example is a full Pit Mutation Testing report of this plugin <a href="https://htmlpreview.github.io/?https://github.com/valantic/mutation-tester/samples/pitreport-v.0.1.1/index.html">here</a>


## Installation
You can download the plugin from our [github(https://github.com/valantic/mutation-tester)].
Next open your IntelliJ and install the plugin from disk, as seen below.
It is recommended to restart your IDE.
![](./samples/screenshots/install-disk.png)


### IntelliJ Marketplace
The Plugin will be published to the Intellij Marketplace. This should be avaible in the store after our beta testing (est. 2022-04).


## Run the plugin
You can simply create a new RunConfigurations with Mutation Tester
![](./samples/screenshots/create-configuration.png)

This Plugin will save you a lot of time. You don't need to create everytime new configurations by hand to test your new unit test. 
With this tool you can automatically create configuration for your given test, as seen below by just executing the test in the run context of the unit test.

![](./samples/screenshots/run-in-class.png)

![](./samples/screenshots/right-click-in-class.png)

You can also select packages in your test directory and test all classes in this package with all the tests in same named package.

![](./samples/screenshots/run-context-menu.png)

If you still need to adjust the configuration you can do this easily. Each run will create a RunConfiguration you can simply modify.

![](./samples/screenshots/run-as.png)


## Configuration
If you need to adjust the defualt configuration, you can just go into your RunConfiguration and adjust the default settings.

![](./samples/screenshots/settings-1.png)

![](./samples/screenshots/settings-2.png)

In the tab settings the values of targetTests, targetClasses, reportDir, sourceDirs and mutators can not be empty. Otherwise the tests will not run. in the advanced tab you can easily modify default behaviour.

![](./samples/screenshots/advanced-settings.png)


You can get more informations about the configuration fields [here](https://pitest.org/quickstart/commandline/).


## Copyright and Licensing Information
See [LICENSE.md](LICENSE.md) for the complete License.

Copyright [2022] [valantic CEC Schweiz AG]

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

```
http://www.apache.org/licenses/LICENSE-2.0
```

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.


## Contact Information
For any issue with plugin please use the our <a href="https://github.com/valantic/mutation-tester/issues">issueboard on github</a>.

For any information about our company go to <a href="https://valantic.com">valantic.com</a>.


## Credit and Acknowledgments
This Plugin is based on the commandline tools from <a href="https://pitest.org/">pitest.org</a>.
So special credits go out to henry@pitest.org for developing such an amazing tool.

Also the Icon (mutation.png) is based on an icon from flaticon by Freepik.
<a href="https://www.flaticon.com/de/kostenlose-icons/gen" title="gen Icons">Gen Icons erstellt von Freepik - Flaticon</a>

## Change Notes
- <b>0.1.0</b> - 2022-02: Published Beta Version with primary focused on SAP Commerce
- <b>0.1.1</b> - 2022-02: Raised Testcoverage. Fixed issue with missing module on run configuration

## Roadmap
- [ ] testing badges (test and pitest)
- [ ] fix beta issues
- [ ] add to IntelliJ Marketplace
- [ ] cross module testing
- [ ] caching
