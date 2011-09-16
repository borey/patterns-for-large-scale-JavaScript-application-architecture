This project is an attempt to build a JavaScript application structure based on the article "Patterns For Large-Scale JavaScript Application Architecture", written by: Addy Osmani on http://addyosmani.com/largescalejavascript/

The Proposed Architecture 

	The solution to the architecture we seek to define is a combination of three well-known design patterns: the module, facade and mediator.

	Rather than the traditional model of modules directly communicating with each other, in this decoupled architecture, they'll instead only publish events of interest (ideally, without a knowledge of other modules in the system). The mediator pattern will be used to both subscribe to messages from these modules and handle what the appropriate response to notifications should be. The facade pattern will be used to enforce module permissions.
