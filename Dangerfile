# Check links
require 'json'
results = File.read 'ab-results-README.md-markdown-table.json'
j = JSON.parse results
if j['error']==true
  m = j['title']
  m << ', a project collaborator will take care of these, thanks :)'
  warn m
  markdown j['message']
end
