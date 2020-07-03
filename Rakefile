namespace :greeting do

  desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end

desc 'outputs hola to the terminal'
task :hola do
  puts "hola de Rake!"
end

end

desc 'console'
task :console do
end

namespace :db do

  task :environment do
    require_relative './config/environment'
  end

  desc 'invokes the environment task as a dependency'
  task :migrate => :environment do
    Student.create_table
  end

  desc 'seeds the database with dummy data from a seed fil'
  task :seed => :environment do
    require_relative './db/seeds.rb'
  end

end



