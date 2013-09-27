Read first !
============

This is an experimental repository. If you're using OSX and have a card that support
most of what is binded here. Then chances are that it will just work for you.

Otherwise, this updated opengl binding is not likely to work on other platform 
unfortunately. It might compile fine but if extensions aren't loaded at runtime,
it will probably segfault as soon as you'll try to use some opengl 1.5+ features.

That said !
===========

I have no idea what I'm doing but these bindings are working for me. Since I have little
idea of what's going on, I might not be much of a help if something isn't working for you.

On the other side, if you have problem with it. You can create an issue and I might get it
resolved. I'm not planning to limit myself to OSX in the long run so chances are that
I might fix issues with other platforms as I discover them...Actually most problem are
fixed as I discover them.

Why updating a binding for opengl ?
===================================

The bindings in the chicken-egg repository are pretty old. If I'm right, they haven't been
updated for years. They only support opengl 1.4-. Anything related to shader is a no go.
For a school project, I dediced to use opengl and didn't want to restrain myself to Opengl1.4.
For that reason, I updated the egg with the `gl.h` header that comes with OSX.

As far as I understand, on OSX, extensions are already loaded or something like that. For that
reason, the use of extension loaders like `glee` and `glew` shouldn't be necessary for 
standard things. If you need some special extensions, then most probably loading them manually
might be necessary and that's out of the scope of what I'm doing.

Installing should be as easy as

    cd where_cloned
    chicken-install -location .

Why not posting updates to the chicken-egg repository?
======================================================

I have no idea of what I'm doing and it might just work or break everything.
