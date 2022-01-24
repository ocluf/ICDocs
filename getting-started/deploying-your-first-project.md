# deploying your first project

Now that the SDK is installed run the following command in a terminal to create a new project directory:

```
dfx new hello --no-frontend
```

Open the freshly created `hello` directory  in your favourite editor or `cd` into it from your current terminal with `cd hello`.&#x20;

From this directory run the following command to start a local node (called a replica) of the Internet Computer.

```
dfx start --background
```

Now that we have a local replica running let's deploy your first canister!  Run the following command:

```
dfx deploy
```

\
5\. Lets take a look at what we just deployed. When you open `src/hello/main.mo` you'll find the source code of your canister, which looks like this:

```
actor {
    public func greet(name : Text) : async Text {
        return "Hello, " # name # "!";
    };
};
```

This is a source file written in Motoko, a language custom made for the Internet Computer. We see that our code has a public function called `greet` which takes a Text input called `name`.\
\
The function takes the `name` parameter and returns a new Text value by putting `Hello,` in front of it and `!` behind it.&#x20;



\
\
\
\
\
\
