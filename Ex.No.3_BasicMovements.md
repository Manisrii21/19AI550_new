# Ex.No: 3  Basic movements in Unity 
### DATE: 29-04-2026                                                                          
### REGISTER NUMBER : 212223110025
### AIM: 
 To learn the basic movements translation,scaling and rotation of game objects through code.
### Procedure:
1. Setup the Scene
2. Open Unity and create a 3D Scene.
3. Add three objects:Cube → Rename to Object1 (for movement),Sphere → Rename to Object2 (for rotation).Capsule → Rename to Object3 (for scaling).
4. Add the Script,Create a C# Script → Name it TransformOperations.cs.
5. Write the code for translation,scaling and rotation,save and close the script
6. Save the script
7. Select any empty GameObject (or create one: GameObject → Create Empty).
8. Attach the TransformOperations script to it.
9. In the Inspector, assign Object1 → Drag the Cube,Object2 → Drag the Sphere.Object3 → Drag the Capsule.
10. Run the Scene Press Play ▶️ in Unity
11. Stop the program.
### Program 
```
using UnityEngine;

public class TransformOperations : MonoBehaviour
{
    public Transform object1; // Move
    public Transform object2; // Rotate
    public Transform object3; // Scale

    void Update()
    {
        if (object1 != null)
        {
            object1.Translate(Vector3.right * 3f * Time.deltaTime);
        }

        if (object2 != null)
        {
            object2.Rotate(0, 100f * Time.deltaTime, 0);
        }

        if (object3 != null)
        {
            float scale = Mathf.PingPong(Time.time, 1f) + 1f;
            object3.localScale = new Vector3(scale, scale, scale);
        }
    }
}
```
### Output:

BEFORE MOVEMENTS 
<img width="1919" height="1024" alt="Screenshot 2026-04-30 114806" src="https://github.com/user-attachments/assets/f06e512f-88e5-471e-9a01-be88e03eb30c" />


AFTER MOVEMENTS
<img width="1918" height="993" alt="Screenshot 2026-04-30 141658" src="https://github.com/user-attachments/assets/726d828e-e28d-4e61-998c-30b78ca5d92f" />







### Result:
Thus the basic movement is learned through scripting


