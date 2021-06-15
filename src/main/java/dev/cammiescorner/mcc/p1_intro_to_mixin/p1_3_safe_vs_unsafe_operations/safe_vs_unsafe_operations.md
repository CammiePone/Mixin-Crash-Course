## Safe vs. Unsafe Operations
Firstly, I should define what I mean by "safe" and "unsafe" operations, as there are no standardised terms for these groupings.
<br><br>
When I refer to a "safe" operation, I mean an operation that will - if done properly - work with other mods that do the same operation in the same place. These would be your `@Inject`, `@ModifyVariable`, and `@Accessor`/`@Invoker` annotations.
<br><br>
When I refer to an "unsafe" operation, I mean an operation that will always break with another mod that does the same operation in the same location. These are your `@Overwrite`, `@Redirect`, and `@ModifyConstant` operations.

## When to Use Safe Operations
Safe operations are the ones you want to use the most whenever doing anything regarding Mixins. So long as you do them right, there is no reason to not use them if you need them, however there are some exceptions.
<br><br>
For instance, if the modding API you are using - whether it be Forge, Fabric, Quilt, or some other API - has its own event for what you are trying to do, in most situations it may be easier, or better for compatibility, to use that event instead of your own Mixin.

## When to Use Unsafe Operations
Unsafe operations should be used as sparingly as possible. While they are easier, and often more direct, than using one of the safe operations to achieve the functionality you want, they're usually not necessary.
<br><br>
That being said, there are two major instances in which it is acceptable to use an unsafe operation. They are:

1. You are making a library or API for other modders to use, and what you are doing cannot be achieved without the use of an unsafe operation, and
   <br><br>
2. You are making a mod that is almost entirely impossible to make without unsafe operations.

An example of the first one would be Somnus API, a mod that allows other mods to use and mess with the sleeping feature of Minecraft.
<br><br>
An example of the second one would be Sodium, a mod that replaces Minecraft's rendering engine with its own.