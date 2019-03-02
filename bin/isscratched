#!/usr/bin/env node
var scratchName
if(process.argv[2]==undefined){
  var packageJSON = require('fs').readFileSync(process.cwd()+'/package.json')
  var pack = JSON.parse(packageJSON)
  scratchName=pack.name
}else scratchName=process.argv[2]
var orgsJSON = require('child_process').execSync('sfdx force:org:list --json')
var orgs = JSON.parse(orgsJSON).result
orgs.scratchOrgs.forEach(org => {
  if(org.alias==scratchName) process.exit()
});
process.exit(1)