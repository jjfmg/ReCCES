# Joshua Gonzales
# jgonzales6@ucmerced.edu

desc 'Compiles SASS into style.css'
task :sass do
  require 'sass'
  engine = Sass::Engine.for_file('./sass/style.scss', syntax: :scss)
  File.open('./style.css', 'w') {
    |f| f.write(engine.render)
  }
end

task default: :sass
