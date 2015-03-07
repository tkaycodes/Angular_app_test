#My first Angular App (Thanks to Chris):
#below is a step by step walk-through of how we got started:


###Start with running command:
```shell
rails new angular -T -d postgresql
```

###Next, generate a model and a controller for "tasks" which is what our app will be about:

```shell
rails g model Task
rails g controller tasks
```

###Next, inside the task.rb file add the lines below so it looks like:
```shell
class Task < ActiveRecord::Base
  respond to :html, :js, :json
end
```

###Now, make some new folders and a todo_list.js file(this file will include all of our dependencies) inside the javascripts directory(this is important for organization!) Your setup should look like this:

 ```shell
app/assets/javascripts/directories
app/assets/javascripts/factories
app/assets/javascripts/services
app/assets/javascripts/templates
app/assets/javascripts/vendors
app/assets/javascripts/todo_list.js
```

###Inside the todo_list.js file we just created, make it look like this:

```shell
angular.module('todo', [], function(){
  });
```
###Now, we can go ahead to : https://angularjs.org/ and download the angularJS library:
(Place it inside the vendors folder we created above (In this folder, we will put external libraries, like the one we just downloaded - we typically never modify these files!)

* ...

##After downloading, your setup should look like this:

```shell
app/assets/javascrips/vendor/angular.js
(The angular.js file being the one we downloaded from the angular link above)
```

###Even though we dont need to, we will be explicitally 'requiring' everything inside the application.js manifest file. It should look like this:

```shell
//= require jquery
//= require jquery_ujs
//= require turbolinks
//= require_tree ./vendor
//= require_tree .
//= todo_list.js
```



###Great! Now lets setup our routes as follows:!

```shell
  root 'tasks#index'
```

###Lastly, inside our views folder, create a tasks subfolder, and inside that subfolder, create an index.html.erb file. So, inside the views/tasks/index.html.erb file, it should look like this:
```shell
<div ng-ap="todo">
</div>
```

#ANGULAR IS NOW SETUP AND READY TO GO!!:)

