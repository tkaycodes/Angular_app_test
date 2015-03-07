#README

# PROJECT WITH CHRIS ON REACT:

## started with running command:
```shell
rails new angular -T -d postgresql
```

##next generated a model and a controller:

```shell

rails g model Task
rails g controller tasks

```

##next inside the task.rb file add these lines so it looks like this:
```shell

class Task < ActiveRecord::Base
  respond to :html, :js, :json
end

##make some new folders inside the javascripts directory(its important for organization!):
 ```shell
app/assets/javascripts/directories
app/assets/javascripts/factories
app/assets/javascripts/services
app/assets/javascripts/templates

also make a new file(todo_list.js):

app/assets/javascripts/todo_list.js

this file will declare and include all of your dependencies!!

```

##inside that file, start off like this:


angular.module('todo', [


  ])




##


* ...


Please feel free to use a different markup language if you do not plan to run
<tt>rake doc:app</tt>.
