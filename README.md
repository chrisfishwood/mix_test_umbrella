# MixTestUmbrella

How the project was created....

###Create umbrella app
`mix new mix_test_umbrella --umbrella`

###Create 2 phoenix apps under the umbrella
`cd mix_test_umbrella/apps`
`mix phoenix.new api --no-html --no-brunch`
`mix phoenix.new web --no-html --no-brunch`

###Run mix test from the parent
`cd ..`
`mix test`

The api project will pass, the web project will fail with "database "web\_test" does not exist"
