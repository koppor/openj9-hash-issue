# Demonstration of [Semeru-Runtimes#3](https://github.com/ibmruntimes/Semeru-Runtimes/issues/3)

For IBM Semeru releases before mid of Octoboer 2025, when executing `./gradlew jlinkZip` on macOS one gets

    java.lang.module.FindException: Hash of java.rmi (03f539ebf91c81cfc7a81236d2c1109e0d050c839d03c6f757022b99a10cb819) differs to expected hash (07126a5cefcc6c19d9059cfa4b42ec832f3714a1ef89f103afc2d1ab61b79bc7) recorded in java.base

This is resolved for JDK 25.

See also the build output of the workflow <https://github.com/koppor/openj9-hash-issue/actions/workflows/build.yaml>.
