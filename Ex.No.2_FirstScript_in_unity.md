# Ex.No: 2  Welcome Script in Unity
### DATE: 28-04-2026                                                                        
### REGISTER NUMBER : 212223110025
### AIM: 
 To learn the basic scripting in Unity and print welcome message in Console window. 
### Procedure:
1. Start the program
2. Open the Unity hub and Create a new 3D project
3. In Assets window, create the new folder and name it as Scripts
4. Create a new script with file name as FirstScript
5. Open the Script and print message "Welcome to Unity" inside the start function
6. Save the script
7. Create a new 3D game object in Hierarchy window and name it as 3DObject.
8. Add the component Firstscript in inspector window of 3Dobject.
9. Run the program
10. Stop the program.
### Program 
```
using UnityEngine;

public class firstscript : MonoBehaviour
{
    // Start is called once before the first execution of Update after the MonoBehaviour is created
    public Transform object1;
    public float speed ;
    void Start()
    {
        //print("Welcome to Unity!");
    }

    // Update is called once per frame
    void Update()
    {
        //print("Welcome to Unity!");
        //this.transform.Translate(0.02f, 0, 0);
        //transform.position += new Vector3(0.02f, 0, 0);
        if(Input.GetKeyDown(KeyCode.Space))
        {
            object1.position += new Vector3(0, 0, speed);
        }
    }
}
```
### Output:

<img width="1918" height="1025" alt="image" src="https://github.com/user-attachments/assets/0ce6f2ec-4d49-4fc9-b43f-9317d7085f8d" />



### Result:
Thus the welcome script was printed on Console Window  sucessfully.

