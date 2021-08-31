This branch actually restructures the benchmark so that to run it only against: FastJSON.

Specifically all the libraries and source files that are not involved with the execution of the benchmark against FastJSON have been removed. As well, also some statements in the classes that execute the benchmark (e.g. [BenchmarkRunner](tpc/src/serializers/BenchmarkRunner.java) ) have been commented out. Finally, the [Makefile](tpc/Makefile) have been modified so that to build only the classes that are needed for running the benchmark against FastJSON.

The branch also includes an extra [JAR](tpc/built-jar/jvm-serializer-FastJSONBenchmarkOnly.jar) which distributes a pre-built version of the benchmark on FastJSON.

Look in the "tpc" directory for source code; or see https://github.com/eishay/jvm-serializers/wiki for current results.
