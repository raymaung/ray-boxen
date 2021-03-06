# This file manages Puppet module dependencies.
#
# It works a lot like Bundler. We provide some core modules by
# default. This ensures at least the ability to construct a basic
# environment.

def github(name, version, options = nil)
  options ||= {}
  options[:repo] ||= "boxen/puppet-#{name}"
  mod name, version, :github_tarball => options[:repo]
end

# Includes many of our custom types and providers, as well as global
# config. Required.

github "boxen", "2.1.0"

# Core modules for a basic development environment. You can replace
# some/most of these if you want, but it's not recommended.

github "dnsmasq",    "1.0.0"
github "gcc",        "1.0.0"
github "git",        "1.2.2"
github "homebrew",   "1.1.2"
github "hub",        "1.0.0"
github "inifile",    "0.9.0", :repo => "cprice-puppet/puppetlabs-inifile"
github "nginx",      "1.4.0"
github "nodejs",     "2.2.0"
github "repository", "2.0.2"
github "ruby",       "4.1.0"
github "stdlib",     "4.0.2", :repo => "puppetlabs/puppetlabs-stdlib"
github "sudo",       "1.0.0"
github "sysctl",     "1.0.0" 
github "postgresql",  "1.0.0", :repo => 'boxen/puppet-postgresql'

github 'property_list_key', '0.1.0', :repo => 'boxen/puppet-property_list_key'

# requires property_list_key
github 'osx',               '1.0.0', :repo => 'boxen/puppet-osx'

# requires: osx
github 'zsh', '1.0.0', :repo => 'boxen/puppet-zsh'

github 'vlc',            '1.0.1', :repo => 'boxen/puppet-vlc'
github 'dropbox',        '1.1.0', :repo => 'boxen/puppet-dropbox'
github 'handbrake',      '1.0.0', :repo => 'boxen/puppet-handbrake'
github 'sublime_text_2', '1.1.1', :repo => 'boxen/puppet-sublime_text_2'
github 'virtualbox',     '1.0.3', :repo => 'boxen/puppet-virtualbox'
github 'chrome',         '1.1.0', :repo => 'boxen/puppet-chrome'
github 'skype',          '1.0.2', :repo => 'boxen/puppet-skype'
github 'cyberduck',      '1.0.0', :repo => 'boxen/puppet-cyberduck'


# Optional/custom modules. There are tons available at
# https://github.com/boxen.
