java_binary(
  name = 'plugin',
  main_class = 'org.ostrovsky.buck.Main',
  manifest_file = 'resources/MANIFEST.MF',
  deps = [':plugin-lib'],
)

java_library(
  name = 'plugin-lib',
  srcs = glob(['java/**/*.java']),
  deps = [':commons-io'],
)

prebuilt_jar(
  name = 'commons-io',
  binary_jar = ':commons-io-jar',
  source_jar = ':commons-io-src',
)

remote_file(
  name = 'commons-io-jar',
  sha1 = 'a8762d07e76cfde2395257a5da47ba7c1dbd3dce',
  url = 'mvn:commons-io:commons-io:jar:1.4',
  out = 'httpmime.jar',
)

remote_file(
  name = 'commons-io-src',
  sha1 = '48753e43ff29409fbbeadfb36186cbe27e41b179',
  url = 'mvn:commons-io:commons-io:src:1.4',
  out = 'httpmime-src.jar',
)
