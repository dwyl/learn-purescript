# learn-purescript

## How

### Install

The first step is to install `PureScript` on your machine.
Make sure to have nodejs and npm already installed, then run `npm install -g purescript`.
This will install `PureScript` globally (ie: the option `-g`) on you computer.
The `purs` command line will be then available: `purs --version`:
![image](https://user-images.githubusercontent.com/6057298/54027146-50539480-4198-11e9-9506-c435b24df674.png)

`purs` is used for compiling PureScript programs and provides also some tools (e.g: create/publish documentation, repl).
However other build tools (e.g: `pulp`, `spago`) based on top of `purs` aim to to create a better user experience when using PureScript.


### Start a new project

#### Pulp and Bower

The common way to create a new PureScript project 
is to use [Pulp](https://github.com/purescript-contrib/pulp), a build tool for PureScript,
with [Bower](https://bower.io/) a package manager.

Run `npm install -g pulp bower` to install these two packages.

Then create a new folder and go to this new directory with: 
`mkdir my-app && cd my-app` (change `my-app` to the name of your project)

Then initialise a new `PureScript` project with `pulp init`. You should see something similar to:

![image](https://user-images.githubusercontent.com/6057298/53793305-7de4d780-3f25-11e9-8a05-6b3155f9f805.png)

You can then run the new created project with `pulp run`.
This command will first compile the project to javascript then it will run this compiled code with Nodejs.

![image](https://user-images.githubusercontent.com/6057298/53793648-3743ad00-3f26-11e9-82f5-a6121f1f5519.png)

#### Spago

[Bower's website](https://bower.io/) is now recommanding other tools for managing packages.
> ...psst! While Bower is maintained, we recommend using Yarn and Webpack or Parcel for front-end projects read how to migrate!

Bower can still be used to manage PureScript packages as it is still maintained. 
However [Spago](https://github.com/spacchetti/spago) is a recent project which provides 
a buiding tool for PureScript and a package manager (based on [Package-Sets](https://github.com/purescript/package-sets))
at the same time.

Run `npm install -g spago` to install Spago on your machine. Then create a folder and initialise a PureScript project:

`mkdir my-app && cd my-app` then `spago init`. This will create the structure of a new PureScript project.

You can then build the project with `spago build` or run the tests with `spago test`.


