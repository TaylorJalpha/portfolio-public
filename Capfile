require "capistrano/setup"
#INclude default deployment tasks
require "Capistrano/deploy"











require "capistrano/scm/git"
install_plugin Capistrano::SCM::git













require "capistrano/rbenv"

require "capistrano/rails"

require "capistrano/passenger"

dir.glob(lib/capistrano/tasks/*.rake).each { |r| import }

set :rbenv_type, :user
set :rbenv_ruby, '2.3.3'
