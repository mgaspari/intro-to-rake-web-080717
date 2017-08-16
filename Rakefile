namespace :greeting do
desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end
desc 'outputs hola in the terminal'
task :hola do
  puts "hola de Rake!"
end
end

namespace :db do
  desc "environment setup"
  task :environment do
    require_relative './config/environment'
  end

  desc 'migrate the database'
  task :migrate => :environment do
    Student.create_table
  end
  desc "seed the database so that it has values"
  task :seed do
      require_relative "./db/seeds.rb"
  end
end
