# learn-purescript

## How

### Install

The first step is to install `PureScript` on your machine.
The easiest way require to have nodejs and npm already installed and to run `npm install -g purescript`.
This will install `PureScript` globally (because of the option `-g`) on you computer.

You need to also install:
- `pulp` the build tool for `PureScript` (it helps to create and manage your project)
- `Bower` the package manager used by `PureScript` (used to install other packages in projects)

Run `npm install -g pulp bower` to install these two packages.

### Start a new project

Create a new folder and go to this new directory with: 
`mkdir my-app && cd my-app` (change `my-app` to the name of your project)

Then initialise a new `PureScript` project with `pulp init`. You should see something similar to:

![image](https://user-images.githubusercontent.com/6057298/53793305-7de4d780-3f25-11e9-8a05-6b3155f9f805.png)

You can then run the new created project with `pulp run`.
This command will first compile the project to javascript then it will this compiled code with Nodejs.

![image](https://user-images.githubusercontent.com/6057298/53793648-3743ad00-3f26-11e9-82f5-a6121f1f5519.png)

