# ![EnScript](https://i.ibb.co/wYGHbkD/d9f6e998c492ad14f709d41ed1715b56.png)
>[NEW! Pages](https://github.com/TriSn0w/EnScript/wiki/EnScript-Pages) | [download](https://github.com/trisn0w/enscript/releases/latest)

## Welcome to EnScript!
This is a Easy-to-use Node.js superset (hence the name, "EnScript") that I made for Node beginners, and people that want a different type of Node.js. You can use normal Node with it aswell.

## `.en` VS `.en.native`
**Note**: This is for the v2.0 update. If you want this feature ASAP, then get the [release](https://github.com/TriSn0w/EnScript/releases)

Comparison between the two:
| File Extension | Pros | Cons |
|----------------|----------|------|
|`.en` | - More like a seperate language than a superset | May be confusing at first</br></br>Does not have backwards compatibility with `v1.1` |
|`.en.native` | - More like a superset </br>- Has better JavaScript support</br>- Most syntax is removed so you can use plain JavaScript along with EnScript |  Does not have backwards compatibility with `v1.1` |

## Installation/Usage
1. Download the runCode.js
2. Make a `script.en` file that looks something like this:
   ```js
   console.log['Hello World!'];
   ```
 <br>  
3. Go to the path of both files and run this code in the terminal

```sh
node runCode.js [name-Of-En-File]
```

## Syntax / Examples
Here is an example of console logging (the famous "Hello World!" one)
```js
console.log['Hello World!'];
```

Here is another example, with functions.
```js
function test() ~>
console.log['Wowie!'];
<~

test();      
```

Now, see how some lines have the character `;`? It helps the interpreter know it's the end of a line (so there are no errors).

Let's do one more example. A Discord bot!

```js
!! this code has been tested by us, and should work!
@variable Discord = import['discord.js'];
@variable client = new Discord.Client();

client.on['ready', () :: ~>
  console.log[`Ready as ${client.user.username}`];
<~];

client.on['message', (message) :: ~>
  if (message.content == "ping") ~>
    message.reply('Pong!');
  <~
<~];

client.login['YOUR_TOKEN_HERE'];
```
This code seems a little different than Node.js.

## More of the README is being worked on and is coming soon!
If you want, check out the [docs](https://github.com/TriSn0w/EnScript/wiki)
