## What is Mixin?
Mixin is a tool used by modders to modify or add code to the Vanilla game (or other mods) in an easy, and safe manner. This is not to say that Mixin is totally safe to use, nor does this mean it's not prone to user error, but it is safer than the alternatives.

## Alternatives to Mixin
There are alternatives to Mixin, such as ObjectWeb ASM and Jarmodding.
<br><br>
ObjectWeb ASM, or ASM for short, is the tool that Mixin is built off of. Like Mixin, it is a method of altering Java Bytecode at runtime. However, unlike Mixin, it is much more difficult to not just learn, but to write safely, due to being so different from typical Java code.
<br><br>
Jarmodding, on the other hand, has the ease of learning strength that comes with Mixin, however it results in a mod that can not work with other mods, unless they are compiled together. While great for single mods, or modloaders, it is not suitable for collections of mods, or modpacks.

## Mixin Misconceptions
1. _"Mixin causes mods to be highly incompatible with one another!"_
   <br><br>
   This is, in the kindest way possible, a flat-out lie.
   <br><br>
   Mixin is a powerful tool, yes, and it can be mishandled and create massive incompatibilities, but it is far safer than its alternatives given the amount of power it grants a modder over the code they're working with.
   <br><br>
2. _"Mixin is all-powerful."_
   <br><br>
   Unfortunately, Mixin has limitations (which will be spoken about in [Limitations of Mixin](https://github.com/CammiePone/Mixin-Crash-Course/blob/master/src/main/java/dev/cammiescorner/mcc/p1_intro_to_mixin/p1_2_limitations_of_mixin/limitations_of_mixin.md)). For all the power it grants to modders, it has some things that hold it back.
   <br><br>
3. _"Mixin can fully replace a modding API."_
   <br><br>
   This is another misconception that I wish was true, but is far from the truth.
   <br><br>
   While Mixin can replace many things, including events (premade injection sites to make it easier for modders to add additional functionality to a given "event" that occurs in game, such as an item being dropped), it cannot replace everything.
   <br><br>
4. _"Mixins are 100% safe, so long as you don't use `@Overwrite`."_
   <br><br>
   This is very much untrue. There are two other "unsafe" operations that I will get into in [Safe vs. Unsafe Operations](https://github.com/CammiePone/Mixin-Crash-Course/blob/master/src/main/java/dev/cammiescorner/mcc/p1_intro_to_mixin/p1_3_safe_vs_unsafe_operations/safe_vs_unsafe_operations.md).