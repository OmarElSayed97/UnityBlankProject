# UnityBlankProject



## Conventions & Rules

1. ALWAYS use descriptive Variables and Methods:
```C#
int i_PrimaryWeaponAmmo = 30;
int i_SecondaryWeaponAmmo = 40;

void Start()
{
    IntializeAmmunations();
}
```

2. Use PascalCase for Variables:
```C#
Transform t_PilotTransform;
GameObject go_PilotGameObject;
int i_PilotHP;
```

3. Use small letters abbreviations to describe Variables
..* go_ for GameObject <br />
..* t_ for Transform <br />
..* i_ for int <br />
..* Is for Bool <br />
..* f_ for float <br />
..* p_ for Pilot <br />
..* titan_ for Titan <br />
..* wep_ for Weapon <br /> 
..* ability_ for Weapon <br /> 
..* ui_ for anything related to UI <br />
..* anim_ for Animator <br />
..* audioSource_ for AudioSources <br />
..* audioClip_ for AudioClip <br />
..* l_ for any lists and arrays (l_go_ , l_p__) <br />
..* __-_ for any static Variable (__go_ , __p_) <br />

```C#
Transform t_PilotTransform;
GameObject go_PilotGameObject;
int i_PilotHP;
bool IsHit;
Weapon wep_PilotPrimaryWeapon
GameObject[] l_go_Enemies
Tranforms[] l_t_TitanPositions
static Pilot __p_MainPilot
```
4. Use PascalCase for Methods:
```C#
GetHit()
{
  Debug.Log("I'm HIT");
}

WallRide()
{

}
```

5. Use CamelCase for Methods Parameters:
```C#
GetHit(int index)
{
  Debug.Log("I'm HIT" + index);
}

WallRide(Transform targetWall)
{
    targetWall.position = null;
}
```
6. Use [SerializeField] instead of public to show Variables in inspector:

```C#
[SerializeField]
private Transform t_PilotTransform;

[SerializeField]
public int i_PilotHP;

```


7. Use regions to organise every block of your code:
```C#
#region Variables
int HP;
#endregion

```

8. There will be a Singleton in every script for the PlayerPilot, Use it carefully.

9. You will find your script containing regions, use them and make all your scripts similar to them, also feel free to add more regions.

10. You will find a SampleScript.cs that contains all of the required regions, you can copy it's if you are going to create a new script.

11. Everyone of us has his own Structured Sandbox (Scene) to create and test his tasks, Try sticking to the Scene Hierarichy.


