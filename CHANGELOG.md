## CHANGELOG

### v0.10.6 (2018-03-20)

* Fix script issues due to file permissions (#81)

### v0.10.5 (2018-02-27)

* cargo make audit will only be invoked if a Cargo.lock file exists (#74)

### v0.10.4 (2018-02-26)

* Fix composite environment variables resolution order (#78)

### v0.10.3 (2018-02-24)

* update_check_minimum_interval default changed be weekly (#76)
* Added test_ files to kcov test coverage invocation
* Update dependencies documentation (#72)

### v0.10.2 (2018-02-08)

* Check for update minimum interval definition in global configuration (#68)

### v0.10.0 (2018-02-02)

* Search for makefile.toml in parent directories (#65)
* Global configuration file to define default log level, task name (#64)
* Reformat changelog (#66)

### v0.9.5 (2018-01-22)

* fixed critical loading issue due to #56

### v0.9.4 (2018-01-19)

* support new skip_core_tasks config flag (#56)

### v0.9.3 (2018-01-05)

* Coverage test files user level pattern (#59 and #60)

### v0.9.2 (2017-12-29)

* Coverage will execute all test files without any need for specific naming conventions or configuration (#50 and #51)

### v0.9.1 (2017-12-28)

* Bug fixes for git info loading and coverage on workspace level (#49 and #52)

### v0.9.0 (2017-12-18)

* Disabled tasks should be skipped including dependencies (#47)

### v0.8.0 (2017-12-17)

* Support multiple rustfmt versions (#45)

### v0.7.11 (2017-12-14)

* Fixed rustfmt backward compatability break issue

### v0.7.10 (2017-12-06)

* Workspace support fixes for windows

### v0.7.5 (2017-12-03)

* Support conditional skipping of workspace members from flow (#42)

### v0.7.4 (2017-10-25)

* kcov support for excluding lines/blocks from coverage report

### v0.7.2 (2017-10-23)

* Added workspace level coverage task without the need to run full CI flow (workspace-coverage)

### v0.7.1 (2017-10-21)

* Added support for cross platform scripts using script runner @shell

### v0.7.0 (2017-10-20)

* Refactored how rust code based scripts are defined to enable future expansion of this feature.

### v0.6.5 (2017-10-12)

* ci-flow and build-flow will build/run benches and examples based on new environment variables: CARGO_MAKE_BUILD_EXAMPLES, CARGO_MAKE_BUILD_BENCH and CARGO_MAKE_RUN_BENCH

### v0.6.1 (2017-10-08)

* Tasks can now run rust code using rust_script attribute and tasks can no longer hold multiple different action definitions.

### v0.5.3 (2017-09-29)

* Added support to evaluate env var values from script output and define cwd on task level

### v0.5.2 (2017-09-24)

* Added various check and build tasks

### v0.5.0 (2017-09-21)

* Disable by default coverage flow on mac

### v0.4.1 (2017-09-18)

* Added watch-flow task

### v0.3.77 (2017-09-17)

* Automatically define install_crate and enable cargo install arguments via install_crate_args

### v0.3.76 (2017-09-16)

* Build failure will not cause panic but will exit

### v0.3.75 (2017-09-12)

* By default build and test should work with "--all-features" flag

### v0.3.66 (2017-08-23)

* Add support for workspace glob members

### v0.3.64 (2017-08-22)

* Cargo.toml parsing fix

### v0.3.63 (2017-08-21)

* Add support for Cargo.toml workspace.exclude

### v0.3.62 (2017-08-21)

* Add workspace member detection based on dependency paths

### v0.3.59 (2017-08-20)

* Support load_script platform overrides

### v0.3.58 (2017-08-19)

* Added load_script capability

### v0.3.56 (2017-08-18)

* Set environment variables during task invocation

### v0.3.53 (2017-08-09)

* Added new condition types: env, env_set and env_not_set

### v0.3.51 (2017-08-09)

* Added experimental cli arg to enable access unsupported experimental predefined tasks

### v0.3.49 (2017-08-08)

* Added condition attribute

### v0.3.46 (2017-08-06)

* Added bintray upload task

### v0.3.43 (2017-08-02)

* Added --env/-e cli args to set environment variables via command line

### v0.3.41 (2017-08-01)

* Added github-publish task

### v0.3.38 (2017-07-28)

* Added run_script which allows executing sub tasks

### v0.3.37 (2017-07-25)

* Added condition script capability for tasks

### v0.3.36 (2017-07-22)

* Added coverage-lcov task (not fully tested)

### v0.3.34 (2017-07-21)

* Added coverage-tarpaulin task

### v0.3.33 (2017-07-21)

* Added more environment variables for workspace support

### v0.3.32 (2017-07-20)

* Added --list-all-steps cli option

### v0.3.28 (2017-07-17)

* workspace level ci flow

### v0.3.27 (2017-07-16)

* cargo make ci-flow on travis now automatically runs code coverage and uploads to codecov

### v0.3.25 (2017-07-16)

* New --no-workspace cli arg

### v0.3.24 (2017-07-15)

* Workspace support

### v0.3.23 (2017-07-14)

* Added codecov task in default toml

### v0.3.20 (2017-07-14)

* Added coverage task in default toml

### v0.3.16 (2017-07-14)

* Added more environment variables based on target environment and rust compiler

### v0.3.15 (2017-07-13)

* Added common init and end tasks

### v0.3.13 (2017-07-10)

* cargo-make now defines rust version env vars

### v0.3.11 (2017-07-09)

* cargo-make now defines env vars based on project git repo information

### v0.3.10 (2017-07-06)

* cargo-make now defines env vars based on project Cargo.toml

### v0.3.6 (2017-07-05)

* Added --cwd cli arg to enable setting working directory

### v0.3.5 (2017-07-04)

* Added clippy task

### v0.3.4 (2017-07-03)

* Added --print-steps cli arg

### v0.3.1 (2017-07-02)

* Added CARGO_MAKE_TASK env var holding the main task name

### v0.3.0 (2017-07-02)

* Renamed few cli options

### v0.2.20 (2017-07-02)

* Added -v and --verbose cli arg

### v0.2.19 (2017-07-01)

* Added extend config level attribute

### v0.2.17 (2017-06-30)

* Added force task attribute

### v0.2.12 (2017-06-28)

* Published website

### v0.2.8 (2017-06-28)

* Platform specific task override

### v0.2.7 (2017-06-26)

* Platform specific alias

### v0.2.6 (2017-06-26)

* Enable task attributes override

### v0.2.3 (2017-06-25)

* Added disabled task attribute support

### v0.2.0 (2017-06-24)

* Internal fixes (renamed dependencies attribute)

### v0.1.2 (2017-06-24)

* Print build time, added internal docs, unit tests and coverage

### v0.1.1 (2017-06-24)

* Added support for env vars, task alias and crate installation

### v0.1.0 (2017-06-23)

* Initial release.
