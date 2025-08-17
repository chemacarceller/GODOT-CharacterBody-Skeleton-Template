# GODOT-CharacterBody-Skeleton-Template

This utility consists of a template for creating a character inheriting from:

Specifically, you want to obtain a CharacterBody3D object, and its mesh will be stored in a Skeleton3D.

The template includes a CollisionShape3D with a capsule-type shape prepared for a 1.80m high skeletal mesh.

This utility also contains an AnimationPlayer node and an AnimationTree node.

The script associated with this utility allows you to assign a skeleton3D and an animationplayer, both stored in packedscene.

When importing a character from mixamo, it is relatively easy to extract both the skeleton3D and the animationplayer and assign them to the character created from this template. This utility also has an additional Vector3 parameter to scale the skeleton3D so that its height matches the 1.80 m height for which the CollisionShape3D is designed.

If you need a character of a different size than 1.80m or need a different collision mesh than the capsule, you can delete the default shape in your character and assign a custom one.

Finally, the template associates the animationplayer assigned to the animationtree node, but does not provide any root of that node, in your character you will be responsible for assigning a value to that parameter
