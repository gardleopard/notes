#configuration
* git config --global branch.autosetuprebase always
* git config --global color.ui auto
* git config --global sslVerify false
* git config --global push.default current


#commands
* rev-parse
* show
* rebase
* fetch
* reflog
* bisect
* daemon
* bundle
* sub-tree


#plumbing
* echo "Long text line" | git hash-object -w --stdin
* git update-index --add --cacheinfo 100644 5575c52f5b68eb2f38080c11e524d0d2b2e83c85 test.txt
* git write-tree
* git commit-tree 17e20bb99b8c57b7d57a1bffadd57e60ac365106 -m "my message"
* git checkout 791b46c
* git checkout -b master

#bisect
* git bisect start
* git bisect bad HEAD
* git bisect good 93870
* git bisect run mvn test


#filter-branch
* git filter-branch


#hooks
```ruby
#!/usr/bin/env ruby
if File.read(ARGV[0]).strip.include?("monkey") then
  exit 0
else
  puts "No monkey"
  exit 1
end
``` 

#fun
* git cat-file -p d670460b4b4aece5915caf5c68d12f560a9fe3e4

#gh-pages
* https://help.github.com/articles/creating-project-pages-manually

#daemon
* git-daemon --base-path=.
* touch git-daemon
* better to run with ssh imho


#forking -- keep your fork up2date
* git remote add upsream https://------ #master repo
* git pull upstream master

#submodules
##vis status på submoduler:
* git ls-tree 7032145


##database
* pull request på dbmigrering
** shipper for seg selv
** koden kommer etterpå

#pretty log
* git log --all --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --

