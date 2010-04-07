require 'rubygems'
require 'rake'

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gem|
    gem.name = "jonbell-awesome_print"
    gem.rubyforge_project = "awesome_print"
    gem.summary = %Q{Pretty print Ruby objects with proper indentation and colors.}
    gem.description = %Q{Great Ruby dubugging companion: pretty print Ruby objects to visualize their structure. Supports MongoMapper objects via included mixin.}
    gem.email = "jonbell@spamcop.net"
    gem.homepage = "http://github.com/jonbell/awesome_print"
    gem.authors = ["Michael Dvorkin", "Jonathan Bell"]
    gem.add_development_dependency "rspec", ">= 1.2.9"
    gem.files = FileList["[A-Z]*", "lib/**/*.rb", "rails/*.rb", "spec/*", "init.rb"]
    gem.has_rdoc = false
    # gem is a Gem::Specification... see http://www.rubygems.org/read/chapter/20 for additional settings
  end
  Jeweler::GemcutterTasks.new
rescue LoadError
  puts "Jeweler (or a dependency) not available. Install it with: gem install jeweler"
end

require 'rake/rdoctask'
Rake::RDocTask.new do |rdoc|
  version = File.exist?('VERSION') ? File.read('VERSION') : ""

 rdoc.rdoc_dir = 'rdoc'
 rdoc.title = "ap #{version}"
 rdoc.rdoc_files.include('README*')
 rdoc.rdoc_files.include('lib/**/*.rb')
end
