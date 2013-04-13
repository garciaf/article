{spawn} = require 'child_process'
fs = require 'fs'

# Until GitHub has proper Literate CoffeeScript highlighting support

task "readme", "rebuild the readme file", ->
  source = fs.readFileSync('promise/promise-fr.coffee.md').toString()
  source = source.replace /\n\n    ([\s\S]*?)\n\n(?!    )/mg, (match, code) ->
    "\n```coffeescript\n#{code.replace(/^    /mg, '')}\n```\n"
  fs.writeFileSync 'README.md', source