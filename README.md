# MixTestUmbrella

##How the project was created
###Create umbrella app
`mix new mix_test_umbrella --umbrella`

###Create 2 phoenix apps under the umbrella
`cd mix_test_umbrella/apps`
`mix phoenix.new api --no-html --no-brunch`
`mix phoenix.new web --no-html --no-brunch`


##How to make it fail
###Run mix test from the parent
`git clone https://github.com/chrisfishwood/mix_test_umbrella.git`
`cd mix_test_umbrella`
`mix test`

The api project will pass, the web project will fail with "database "web\_test" does not exist". Mix debugging is turned on.
