# Jmeter Basic Test Templates

This repo contains some simple Jmeter test templates for running load tests against a web endpoint.

All tests use env files to configure them for ease of use between sites. Read the env.test.txt file as its self-explanitory.

# Usage

Simple start Jmeter with the following command.

```
./jmeter.sh -Duser.dir=/pat/to/my/test/dir/ -DTEST_ENV=test
```

The user.dir is optional, but if you dont do it, and you run a lot of tests, your jmeter/bin dir will fill up with lots of results.
The second property, tells Jmeter to set the enviroment to test, which we use to locate a file called env.test.txt located in the user.dir