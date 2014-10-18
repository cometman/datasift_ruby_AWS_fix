Hot Fix For Datasift, Rails 4 and AWS
=====================

Using datasift-ruby 3+, with Rails 4 on AWS does not work.  Datasift ruby requires multi_json 1.8+ which does not work on AWS with Rails 4.  

Error message: MultiJson::AdapterError: Did not recognize your adapter specification (cannot load such file -- json/ext/parser).

Fix Overview: Downgraded multi_json in Gemspec to 1.7.8


Run options: --seed 26534


Installation:

gem "datasift", :github => "cometman/datasift_ruby_AWS_fix"

Tested:
# Running:

.........................

Finished in 0.832526s, 30.0291 runs/s, 31.2303 assertions/s.

25 runs, 26 assertions, 0 failures, 0 errors, 0 skips
