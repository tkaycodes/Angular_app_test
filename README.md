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

##make some new folders and a todo_list.js file(this file will include all our dependencies) inside the javascripts directory(this is important for organization!):

 ```shell
app/assets/javascripts/directories
app/assets/javascripts/factories
app/assets/javascripts/services
app/assets/javascripts/templates
app/assets/javascripts/todo_list.js

```

##inside the todo_list.js file, make it look like this:

```shell

angular.module('todo', [], function(){


  });

```


##then go ahead to : https://angularjs.org/ and download the angularJS library:

place it inside the vendors folder we create (we will put external libraries, like the one we just downloaded in here - external stuff go here - typically neve modify these files!)


* ...

## so it should look like this:

```shell
app/assets/javascrips/vendor/angular.js

the angular.js file is the one we downloaded from the site
```


##even though, we dont HAVE to, we will be explicitally requriing everythig inside the application.js file. So far, it should look like this:



##great! now lets setup our routes

```shell

  root 'tasks#index'


```

##lastly, inside our views folder, create a tasks subfolder, and inside that subfolder, create an index.html.erb file. Inside that views/tasks/index.html.erb file, it should look like this:
```shell

<div ng-ap="todo">

</div>

```

#ANGULAR IS NOW SETUP AND READY TO GO!!

Please feel free to use a different markup language if you do not plan to run
<tt>rake doc:app</tt>.
