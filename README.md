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


```


* ...


Please feel free to use a different markup language if you do not plan to run
<tt>rake doc:app</tt>.
