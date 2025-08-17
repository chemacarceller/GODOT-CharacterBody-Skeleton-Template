# GODOT-CharacterBody-Skeleton-Template

This utility consists of a template for creating a character inheriting from...

Specifically, you want to obtain a CharacterBody3D object, and its mesh will be stored in a Skeleton3D.

The template includes a CollisionShape3D with a capsule-type shape prepared for a 1.80m high skeletal mesh.

This utility also contains an AnimationPlayer node and an AnimationTree node.

The script associated with this utility allows you to assign a Skeleton3D and an Animationplayer, both stored in PackedScenes.

When importing a character from mixamo, it is relatively easy to extract both the Skeleton3D and the Animationplayer and assign them to the character created from this template. 

This utility also has an additional Vector3 parameter to scale the Skeleton3D so that its height matches the 1.80 m height for which the CollisionShape3D is designed.

If you need a character of a different size than 1.80m or need a different collision mesh than the capsule, you can delete the default shape in your character and assign a custom one.

Finally, the template associates the Animationplayer assigned to the Animationtree node, but does not provide any root element of that node, in your character you will be responsible for assigning a value to that parameter

Feel free to extend the functionality of this template by adding components such as motion components, camera controller components, or adding multiple CollisionShape3Ds to make complex collision meshes (Note that only those meshes that hang directly from the character root node will be part of the global character collision mesh, collision meshes of nodes attached to the character root node will be ignored).
