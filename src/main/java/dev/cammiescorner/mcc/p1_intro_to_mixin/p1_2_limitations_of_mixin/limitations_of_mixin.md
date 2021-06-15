## Limitations Of Mixin
This is far from an exhaustive list, but despite the sheer power Mixin grants to modders, it does have some limitations. To my knowledge, the majority of these are arbitrary limitations and have no technical reason behind them.
<br><br>
If I am made aware of other limitations at some point in the future, this file will be updated to include them, so check the GitHub repository linked in the description.

1. You cannot modify or add to default methods in interfaces.
   <br><br>
2. On Fabric, you cannot modify or add to Light-Weight Java Game Library (LWJGL) or other library classes that Minecraft uses. There is an exception, but by default, you can not.
   <br><br>
3. You cannot modify or add to if statements, switch statements, for loops, or while loops. You can modify the code contained within them, but you cannot modify the checks within these statements or loops. There are exceptions, but are beyond the scope of this crash course.
   <br><br>
4. You can only use `@Inject` to add code to the `TAIL` or `RETURN` of constructors.