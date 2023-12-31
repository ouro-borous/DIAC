# Database In A Can (DIAC)

DIAC is a proof-of-concept cyber deception tool. Using wordlists of names and login credentials, DIAC outputs a randomly generated list of "sensitive information" (actually junk credentials) in MySQL format. This tool is intended to be used in a high interaction MySQL honeypot that provides false information.

>PLANNED: The user can select a minimum password length. 

>PLANNED: The user can provide a list of company usernames that they want included. This is so if an attacker performs a lookup in the database with an existing username, they are found.

>PLANNED: The user can provide a regex expression to DIAC that correspond to a naming convention. When generating usernames, DIAC follows this convention for more consistent, realistic results.

>EXAMPLE: My name is Marko Morrison and my company username is markom2. This means that I want first name + last initial + no. if repeating. With these conventions, if DIAC were to generate four names for Kathy Smith, the last username would be ksmith4.

>PLANNED: The user can choose for a single complex credential from the database to be stored in a seperate file. If this credential is found anywhere else on the network, it will be known that the database list was sprayed.

>PLANNED: Some passwords are more common than others - it's probably unusual to see perfectly unique passwords in a company. Therefore, assign different weight to passwords based on repetition (no need to make it too complicated)
