## Release notes

- Update java crate test for latest stevedore


### java-0.5.1

- Add scm to enable release of module

- Set JAVA_HOME when installing java

- Fix java crate for non x86 arch on rh derivatives

- Update Java crate to work with fedora
  Redhat 5.5 based distros will now do a rebuild of the jpackage source rpm
  for sun-java-compat.


### pallet-crates-0.5.0


### pallet-crates-0.4.4

- Update for repository management in separate namespaces


### pallet-crates-0.4.3

- Update centos java install
  Explicitly set mode of rpm autoinstaller, and enable jpackage for compat
  package installation

- Update java, maven and tomcat to use pallet 0.4.15

- Update java, tomcat, and maven to use jpackage-utils-compat
  Update java based crates to use the updated jpackage functions in 
  pallet.resource.package, based on the jpackage-utils-compat rpm

- Update java and tomcat crates for jpackage repos disabled by default

- Update for 0.5.0-SNAPSHOT
  Change pallet.resource.\* to pallet.action.\*. Change stevedore calls to
  script functions to use unquote and the pallet.script.lib namespace. 
  Change request to session.  Change build-resources to build-actions.


### pallet-crates-0.4.2


### pallet-crates-0.4.1


### pallet-crates-0.4.0

- Add java-home and jdk-home to java crate


### pallet-crates-0.4.0-beta-1

- Use live-test/\*images\* in java live tests

- Add install of user supplied oracle rpm on CentOS.
  On CentOS, you will can download the Oracle rpm.bin file, get it on the
  node with remote-file, and point the java install at it.  The crate will
  install the rpm.

      (remote-file "some-path" ...)
     (java :sun :rpm-bin "some-path")

- Add support for sun java on debian

- Fix circular project dependency

- Add live test for java crate

- Fix java test for partner repo

- Correct partner repository name

- Fix whitespace and tests

- Added ubuntu-specific update to ensure the 'partner' repository is
  available for installing the Sun JDK using the java.clj crate.

- working node-list compute service

- Fix tomcat and java crates for centos (and hopefully amazon-linux)

- basic package operations with pacman now working

- remove defresource usage from crate/java

- Updated to use template as a map, and for new Hardware in jclouds nodes

- Fixes for functional style.  Added :no-packages target for testing. Added
  brew as default packager on mac.

- Refactoring to a more functional implementation

- Made converge run phase by phase, instead of node by node.  Added
  pre-phase. Removed :reload-all from tests to avoid deftype problems.

- Fixed java crate for target bindings

- add test that provokes failure of java crate

- Added target/\*all-nodes\* and target/\*target-nodes\*.  Made target vars
  uninitialised. Tidied mock.

- Harmonised do-script, cmd-join, et al.  Added defvar, defn, and println to
  stevedore. minor documentation fixes.

- change pallet.target's \*target-template\* and \*target-tag\* to \*target-node\*
  and \*target-node-type\*

- clojure 1.1 / 1.2 compatibility modifications

- clojure 1.1 / 1.2 compatibility modifications

- Updated tomcat and hudson configuration

- added installation of JCE policy files, mostly implemented by hugod

- Added defnode, lift and configuration phases. Adds declaritive
  configuration definiton.

- java install fix

- added basic yum support

- fixed automated install of sun java

- cleanup of line endings and tests

- Fixed package manager add-scope, tests still need update

- Added new resources, crates and configure-resources

