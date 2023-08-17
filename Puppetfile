# 
# Puppetfile
#
# Manage modules and dependencies for Puppet runs
#
forge "https://forge.puppet.com"

# Modules from the Puppet Forge
# Versions should be updated to be the latest at the time you start
mod 'puppetlabs-mod1',                   '1.0.0'
mod 'puppetlabs-mod2',                   '1.0.0'

# Modules from Git
# Use specific tag references!
mod 'pg_mod2',
  :git => 'git@github.com:procter-gamble/.git',
  :branch   => 'master'

mod 'pg_mod1',
  :git => 'git@github.com:procter-gamble/.git',
  :tag => '0.1.0'