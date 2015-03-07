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




##then go ahead to : https://angularjs.org/ and download it:

place it inside the vendors folder we create (we will put external libraries, like the one we just downloaded in here - external stuff go here - typically neve modify these files!)


* ...

## so it should look like this:

```shell
app/assets/javascrips/vendor/angular.min.js

the angular.min.js file is the one we downloaded from the site
```


##even though, we dont HAVE to, we will be explicitally requriing everythig inside the application.js file. So far, it should look like this:

```shell

// This is a manifest file that'll be compiled into application.js, which will include all the files
// listed below.
//
// Any JavaScript/Coffee file within this directory, lib/assets/javascripts, vendor/assets/javascripts,
// or any plugin's vendor/assets/javascripts directory can be referenced here using a relative path.
//
// It's not advisable to add code directly here, but if you do, it'll appear at the bottom of the
// compiled file.
//
// Read Sprockets README (https://github.com/sstephenson/sprockets#sprockets-directives) for details
// about supported directives.
//
//= require jquery
//= require jquery_ujs
//= require turbolinks
//= require_tree .
//=require_tree ./vendor
//= todo_list.js 

```

Please feel free to use a different markup language if you do not plan to run
<tt>rake doc:app</tt>.
