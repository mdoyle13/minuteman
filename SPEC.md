```ruby
# Track an event
minuteman_user = Minuteman.track("login:successfull")
minuteman_user.promote(user.id)

# Trigger an event in the pipeline
Minuteman.trigger("event:name")

# Gets an event analyzer
analyzer = Minuteman.analyze("event:name")
# Counts unique users in that given time
analyze.day(Time.now.utc)

Minuteman("event:name").day | Minuteman("event2:name).day
```

Caching:
Cache ids in events:

Minuteman::Operation:50:AND:20, Minuteman::Operation:50:OR:20
Minuteman::Operation:(50:AND:20):AND:14
