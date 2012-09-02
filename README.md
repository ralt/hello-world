hello-world
===

Introduction
---

It is a simple module. It doesn't do anything but displaying a text on the console.

This module shows how to make a simple module according to node.js. This module
could then be shared on npm or be kept private.

Instructions
---

If you just want to run this module, do the following:

    npm install hello-world

And see the `example.js` file for a usage example.

Here are the instructions to see how to run this module and also how to develop
your modules:

- Run `git clone https://github.com/Ralt/mymodule.git`.
- Go to the `mymodule` folder, and run `sudo npm link`. This will create a global link
of the current module.
- Create a folder named `test`. Go to it, and run `npm link mymodule`. You'll see a
symbolic link of the module in your `test/node_modules/` folder.
- Create a file in the `test` folder, name it `file.js`. Write the following in it:
`require( 'mymodule' )();`.
- Run the file with `node file.js`. See, mymodule is working!
- Now, try to change the `index.js` file in the `mymodule` directory. Rerun `file.js`, and see
that the change immediately happened. Because `npm link` just *creates a link*, not a copy.
- Finally, look at the `package.json` file to understand how this works. More information
can be found on [npmjs.org](https://npmjs.org/doc/json.html).

