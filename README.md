# MixTestUmbrella

##How the project was created
###Created umbrella app
`mix new mix_test_umbrella --umbrella`

###Created 2 phoenix apps under the umbrella
`cd mix_test_umbrella/apps`

`mix phoenix.new api --no-html --no-brunch`

`mix phoenix.new web --no-html --no-brunch`


##How to make it fail
###Run mix test from the parent
`git clone https://github.com/chrisfishwood/mix_test_umbrella.git`

`cd mix_test_umbrella`

`mix test`

The api application will pass, the web application will fail with "database "web\_test" does not exist".
