## Bot Configuration

### Setup
One of the most important steps of getting a Discord bot is running the setup and properly configuring it, on LewdBot, you can start
the setup by using
```javascript
L!setup
```
This quick setup will ask you some simple questions, like `Do you want to enable NSFW?` or `Do you want to set up a music channel?`.
Simply answer these questions with either `Y`, `N` or a mention (`@role` or `#channel`).

---

### Permissions
Once the setup is complete, you can start to configure permissions for the bot, to do this, you will use the `L!perms` command.

#### Listing Permissions
```javascript
L!perms list
```
This command will list all available (and up-to-date) permissions, these are what we later call Permission Nodes in this guide.

#### Retrieving permissions
```javascript
L!perms get [role]
```
This command will list all permissions that are attached to the mentioned role (their names and values).

#### Setting a permission
```javascript
L!perms set [role] [node] [value]
```
This command will change the status of a permission for a role. The node argument takes a Permission Node (seen above on the list command) and the value
argument takes in a `true` or `false` parameter.

#### Resetting permissions for a role
```javascript
L!perms reset [role]
```
This command will reset the permissions for this role (aka clear them).

#### Resetting a specific permission for a role
Ok, we are getting too specific...
```javascript
L!perms clear [role] [node]
```
This command will remove the `node` permission from the `role`, like it was before you added it.

#### TIP: Changing permissions for everyone
You may have noticed this guide always talks about a role, but never everyone, so how come do we set default permissions?

Well, that's where the `@everyone` role comes in! To set default permissions for everyone, just use `everyone` instead of
a `@role`.

---

### Prefix
One important step of Bot configuration is knowing and customizing your prefix. Assuming you ran the setup we described
above, you will probably already have a custom prefix. If not however, feel free to use the following commands:

#### Current Prefix
```javascript
L!prefix
```
This will show your current prefix, along with help on the command.

#### Changing the Prefix
```javascript
L!prefix !
```
This will change your custom prefix to `!`, allowing you to use commands like `!help` instead of `L!help`.

#### TIP: Prefixes are non-replaceable.
That's right, your custom `$` prefix won't override `L!` or `@LewdBot`, that means you can always use those in case
you end up forgetting the custom prefix you set.
