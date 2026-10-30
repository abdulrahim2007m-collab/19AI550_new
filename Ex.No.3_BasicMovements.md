# Ex.No: 3  Basic movements in Unity 
### DATE:            26-10-2026                                                                
### REGISTER NUMBER : 212225040007
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
    public Transform object1; // Object for translation
    public Transform object2; // Object for rotation
    public Transform object3; // Object for scaling

    public float moveSpeed = 2f;
    public float rotateSpeed = 50f;
    public float scaleSpeed = 0.5f;

    void Update()
    {
        // Translation along X-axis
        if (object1 != null)
        {
            object1.Translate(0.02f, 0f, 0f);
        }

        // Rotation around Y-axis
        if (object2 != null)
        {
            object2.Rotate(0f, 0.02f, 0f);
        }

        // Scaling along X and Y axes
        if (object3 != null)
        {
            object3.localScale += new Vector3(0.02f, 0.02f, 0f);
        }
    }
}

```
### Output:


<img width="1380" height="625" alt="image" src="https://github.com/user-attachments/assets/27d26bc1-7e60-43a8-810a-849975f52d8b" />


<img width="1394" height="609" alt="image" src="https://github.com/user-attachments/assets/d08dd349-e49f-4750-8bf2-5801d645f1c3" />


<img width="769" height="450" alt="image" src="https://github.com/user-attachments/assets/c8ea6827-03ca-48b9-8506-26977807bfc2" />




### Result:
Thus the basic movement is learned through scripting


