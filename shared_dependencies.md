Without having access to the actual content of the files in the repository, it's impossible to provide a precise list of shared dependencies, data schemas, id names of DOM elements, message names, and function names. However, based on the typical structure of a Node.js application, we can make some educated guesses:

1. Dependencies: These would be listed in the "package.json" file and might be shared across multiple files. Common dependencies for a SaaS application might include "express" for server setup, "mongoose" for database interaction, "passport" for authentication, and "cors" for handling Cross-Origin Resource Sharing.

2. Exported Variables: These could be shared across multiple files. For example, "server.js" might export the initialized server, which could be used in "bin/www". Similarly, "app.js" might export an Express application instance.

3. Data Schemas: If the application uses a database, data schemas might be defined in one file and used in others. For example, a User schema might be defined in "users.js" and used in "routes/users.js".

4. ID Names of DOM Elements: These would be defined in the Jade view files and used in "public/javascripts/app.js". For example, a form might have an id of "signupForm" in "views/index.jade", and "app.js" might use this id to attach event listeners.

5. Message Names: These could be used for communication between the client and server. For example, "app.js" might emit a "signup" message when a user submits a form, and "server.js" might listen for this message to create a new user.

6. Function Names: These could be shared across multiple files. For example, "routes/index.js" and "routes/users.js" might both use a function called "authenticate" defined in "server.js".

Again, these are just educated guesses based on typical Node.js application structure. The actual shared elements would depend on the specific code in the repository.