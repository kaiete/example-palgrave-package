# example-palgrave-package
Hello!

If you're reading this, you likely came from Instant Palgrave and want to make an add-on.

If so, you've come to the right place. Here's
### How to make a Palgrave add-on
First things first, fork this repo. Once you've done that, you'll want to give it a more original name. Then you can start editing.
#### ppc.json
This is your metadata file. Edit as you wish.
#### commands.json
This is where the action happens. Make sure enabled is "true".

First, try editing the pre-made command. It should look like this.
```json
"whoIsPalgrave": {
        "wakeWord": "who are you",
        "response": "Hello! My name is Palgrave.",
        "execute": "pass"
      }
```
Let's look at it. First off, there's a key called `whoIsPalgrave`. Its value is an object containing `wakeWord`, `response` and `execute`.

First off, `wakeWord`. This will have to be said for the command to trigger.

Then, there's `response` This is what palgrave will say in response.

Finally, `execute`. This is the command palgrave will run after replying. If you don't want to run anything, leave it as pass.

Each time you add a new command, add its code name (in this case `whoIsPalgrave`) to the `list` array.

## That's it!
