# Mosima

Mosima is a **Mo**dern **Si**mplified **M**ake **A**lternative.

Know some Javascript? You already know Mosima. Using is as simple as:

```bash
mosima init
```

```javascript
// .mosima/main.js

export default {
    subTask: function() {
        console.log('Example subtask');
    },
    example: function() {
        console.log('Example task');
        this.subTask();
    }
}
```

```bash
mosima example
```

## What?

Make was originally intended as a build tool for low-level programming 
languages, but turned out to be useful for lots of other uses. 

Mosima is designed as a general purpose tool to tackle tasks encountered 
by developers today. As an example, a web developer today might have to 
use virtualisation tools like docker or vagrant, package managers like
npm or composer, build tools like grunt, gulp, webpack or make. 

## Why another?

Why not use [rake](https://ruby.github.io/rake/), [jake](http://jakejs.com/)
 or others (search, there's loads) ? These tend to be tailored to building 
ruby or JS projects, and require learning a DSL on top of the 
language itself. 

Mosima tasks are plain JS, no DSL, and its aim is to be as little as 
possible, with next to no setup.

## Setup

Just download [this bash script](./mosima), give it execute permissions
(`chmod +x mosima`) and move to a directory in your path 
(e.g. `mv mosima /usr/local/bin/mosima`)
