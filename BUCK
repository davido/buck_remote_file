# Replace Gerrit's home baked maven_jar() toolchain
# with native remote_file() rule

#maven_jar(
#  name = 'httpmime',
#  id = 'org.apache.httpcomponents:httpmime:4.3.4',
#  bin_sha1 = '54ffde537682aea984c22fbcf0106f21397c5f9b',
#  src_sha1 = '0651e21152b0963661068f948d84ed08c18094f8',
#  license = 'Apache2.0',
#)

prebuilt_jar(
  name = 'httpmime',
  binary_jar = ':httpmime-jar',
  source_jar = ':httpmime-src',
)

remote_file(
  name = 'httpmime-jar',
  sha1 = '54ffde537682aea984c22fbcf0106f21397c5f9b',
  url = 'mvn:org.apache.httpcomponents:httpmime:jar:4.3.4',
  out = 'httpmime.jar',
)

remote_file(
  name = 'httpmime-src',
  sha1 = '0651e21152b0963661068f948d84ed08c18094f8',
  url = 'mvn:org.apache.httpcomponents:httpmime:src:4.3.4',
  out = 'httpmime-src.jar',
)

