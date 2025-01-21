# Selene

My journey on learning how to build an interpreter (by writing a Lua interpreter).

# Plan

Since my plan is to learn Zig, Lua internals, and -mainly- how to build an interpreter, I will not worry about compatibility with existing Lua code at first. That means I will not use Lua C API.

The reason I won't use the Lua C API is that it already gives me the things I want to learn how to develop (tokenizer, lexer, virtual machine, etc), so, my plan is to develop a **simple** interpreter, with my own implementations of the base of an interpreter and a standard library. Then, once I have a good understanding of what if going on, I will use the Lua C API to ensure `Selene` can run existing Lua code, by using its standard library only (if that makes any sense).

I am planning `Selene` this way now because I want it to be a "batteries included" language as well. I think Lua is a great language and it would be awesome to use it as a more general purpose language, and not just a language for very small script (given the limitations of the current standard libraries) or embedding in other software (which is one of the reasons Lua is great, but I think it would be nice to use Lua in more places[^1]).

So considering my learning purposes, for now, the steps will be (very roughly written):
- Develop a basic Lua interpreter from scratch;
- Add a simple standard library by `Selene`, not necessarily compatible with [PUC Lua](https://www.lua.org/).
- Ensure compatibility (considering I will be able to use the Lua C API later to do that)


All my development and learning will be public, so, if you see anything weird and you know you can help, feel free to open a issue and/or send pull requests, but I politely ask you to do that didactically, so I (and maybe others reading following this) can improve based on your contributions. Thanks in advance for your kindness!


Fun fact: The project name was chosen`Selene` because it is another name given to our moon (Lua, in portuguese), related to the Greek mythology goddess. Checkout [wikipedia](https://en.wikipedia.org/wiki/Selene). That's why the study of the moon's "geography" is called [selenography](https://en.wikipedia.org/wiki/Selenography).

Another fun fact is that I still doubt if I should name this project [Jaci](https://pt.wikipedia.org/wiki/Jaci), due to the moon goddess of [Guarani mythology](https://pt.wikipedia.org/wiki/Mitologia_guarani), a native Brazilian mythology (just like Lua is native from [Brasil](https://www.youtube.com/watch?v=JMlHex-Ca0A)).

[^1]: Just like JavaScript went out of the browser.
