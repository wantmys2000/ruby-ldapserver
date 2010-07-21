require 'rubygems'
require 'hoe'
require File.join(File.dirname(__FILE__), 'lib', 'ldap', 'server', 'version')

RDOC_OPTS = ['--quiet', '--title', "ruby-ldapserver",
    "--opname", "index.html",
    "--line-numbers", 
    "--main", "README",
    "--inline-source"]

# Generate all the Rake tasks
hoe = Hoe.new('ruby-ldapserver', ENV['VERSION'] || LDAP::Server::VERSION::STRING) do |p|
  p.rubyforge_name = 'ruby-ldapserver'
  p.summary = "A pure-Ruby framework for building LDAP servers"
  p.description = "ruby-ldapserver is a lightweight, pure-Ruby skeleton for implementing LDAP
  server applications."
  p.author = 'Brian Candler'
  p.email = 'B.Candler@pobox.com'
  p.url = 'http://rubyforge.org/projects/ruby-ldapserver'
  p.test_globs = ["test/**/*_test.rb"]
  p.changes = p.paragraphs_of('ChangeLog', 0..1).join("\n\n")
end
