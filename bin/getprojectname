#!/usr/bin/env node
var location
if(process.argv[2]==undefined) location=process.cwd()
else location=process.argv[2]
var packageJSON = require('fs').readFileSync(location+'/package.json')
var pack = JSON.parse(packageJSON)
console.log(pack.name)