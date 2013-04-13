{spawn} = require 'child_process'
fs = require 'fs'

# Until GitHub has proper Literate CoffeeScript highlighting support

turnToReadme = (src, target) ->
  source = fs.readFileSync(src).toString()
  source = source.replace /\n\n    ([\s\S]*?)\n\n(?!    )/mg, (match, code) ->
    "\n```coffeescript\n#{code.replace(/^    /mg, '')}\n```\n"
  fs.writeFileSync target, source

task "readme", "rebuild the readme file", ->
  turnToReadme 'article/promise-en.coffee.md', "README-en.md"
  turnToReadme 'article/promise-fr.coffee.md', "README.md"