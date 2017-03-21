# Sometimes it's a README fix, or something like that - which isn't relevant for
# including in a project's CHANGELOG for example
new_migration = git.added_files.include? 'db/migrate/*.rb'

if new_migration && git.modified_files != ['db/schema.rb']
  fail "Please open an separate PR with only the migrations!"
end
