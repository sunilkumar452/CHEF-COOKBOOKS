# 0.6.0

- Fixed some foodcritic rules
- Set Jenkins to the latest LTS version
- Node monitors can be configured
- Added Chef Solo support
- Basic authentication header must not be disabled

# 0.5.5

- Fixes "undefined method `[]' for nil:NilClass" error introduced in 0.5.4

# 0.5.4

- Added jenkins_script "configure crowd permissions" for Jenkins authentication with a JIRA account
- Added documentation about the ssh_identity recipe

# 0.5.3

- Made executed resource after admin user creation configurable
- Added security strategy with "generate" as default instead of "chef-vault"

# 0.5.2

- Implemented alternative plugin configuration with a template. This fixes the flapping locale plugin configuration on jenkins restart.
- Set mailer defaults to use the local system mail by default
- Set ProjectMatrixAuthorizationStrategy instead of GlobalMatrixAuthorizationStrategy
- Added ssh_identity recipe to generate a SSH identity with Ruby in the Jenkins home folder

# 0.5.1

- Fixes: Jenkins is not restarted after installing plugins for the first time
- Added type.chef_environment so that environment is not empty in production
- Set Nginx default_site_enabled to false
- Added chef-vault dependency

# 0.5.0

- BC break: SSH slaves are found with a search on a node attribute instead of a data bag. The creation of a
  data bag item from a recipe requires admin permissions which is not desirable.

# 0.4.0

- Added support for SSH slaves

# 0.3.2

- Added an attribute to configure global properties in Jenkins
- Fixes bug: Nginx server block for Jenkins is not default

# 0.3.1

- Updated changelog

# 0.3.0

- Added Nginx
- Added composer
- Added composer vendor install for jenkins-php packages
- Added jobs recipe
- Added user settings recipe that fixes missing home folder files and shell 
- Added more Jenkins settings

# 0.2.0

- Added configurable plugins
- Added configurable Jenkins settings
- Added Java, Ant and Git package

# 0.1.1

- Documentation improvements
- Better attribute defaults

# 0.1.0

Initial release of jenkins-server
