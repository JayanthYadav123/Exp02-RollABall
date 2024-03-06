# Exp02-RollABall
## Aim :
To develop a 3D application for RollABall in unity.
## Algorithm:
### Step1 :
Create a new project.

### Step 2 :
Click Heirarchy -> 3D object -> Select the plane -> 3DObject -> Sphere.

### Step 3 :
Define the physics properties of the surface (Rigidbody).

### Step 4 :
Assets -> Create -> # Script

### Step 5 :
Create a folder name Coding and create a C# file to add the coding in it.

### Step 6 :
To add our C# Script file to our selected object, click on the C# Script file and drag it to our selected objects in the Hierarchy window nad run the application.

### Step 7 :
Stop.

## Program:
```
 Developed by :G.Jayanth
 Register Number:212221230030.
```
```python
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class roll : MonoBehaviour
{
    public float xForce = 5.0f;
    public float zForce = 5.0f;
    public float yForce = 200.0f;
    void Update()
    {
        float x = 0.0f;
        if (Input.GetKey(KeyCode.A))
        {
            x = x - xForce;
        }
        if (Input.GetKey(KeyCode.D))
        {
            x = x + xForce;
        }
        float z = 0.0f;
        if (Input.GetKey(KeyCode.S))
        {
            z = z - zForce;
        }
        if (Input.GetKey(KeyCode.W))
        {
            z = z + zForce;
        }
        float y = 0.0f;
        if (Input.GetKeyDown(KeyCode.Space))
        {
            y = y - yForce;
        }
        GetComponent<Rigidbody>().AddForce(x, y, z);
    }
}
```
## Output:
<img width="960" alt="image" src="https://github.com/JayanthYadav123/Exp02-RollABall/assets/94836154/5114e558-a899-4fce-b025-e24a7e076920">

## Result:
Thus a 3D application for RollABall objects in unity is developed successfully.



