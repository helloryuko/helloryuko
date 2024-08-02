выыфшщы

привет lhepmz
<div align='right'>
<img src="https://github.com/user-attachments/assets/88a532c4-60f9-4352-9fa0-f8f97dc0d24a" width=320>
</div>

# Почему так мало сейчас говорят о правах простых мужчин? 😑 Вообще-то мальчик имеет право...
Спиздить знак 🛑
![1711300627972](https://github.com/user-attachments/assets/0c47351b-909c-4e29-9528-f49c210723f6)

Zeemo, [7/27/2024 5:02 PM]
чёрный еблан

Zeemo, [7/27/2024 5:02 PM]
негр

Zeemo, [7/27/2024 5:02 PM]
mocny gaz

Zeemo, [7/27/2024 5:03 PM]
nie lubie mocnego gazu

Zeemo, [7/27/2024 5:03 PM]
uuuuuu

Zeemo, [7/27/2024 5:03 PM]
gengsta

Zeemo, [7/27/2024 5:03 PM]
haha

Zeemo, [7/27/2024 5:03 PM]
most niggas

Zeemo, [7/27/2024 5:04 PM]
pierogi z babki

Zeemo, [7/27/2024 5:04 PM]
i sos z dziadka

Zeemo, [7/27/2024 5:04 PM]
тоже круто  
![image](https://github.com/user-attachments/assets/464f67b4-ba98-43e9-a2f6-23a7605846f0)

bool (*CanShoot)(void* weapon);struct WeaponCmd { 
 bool ToFire; bool ToAim; 
 bool ToReload; bool ToAction; 
 bool ToInspect;}; 
void (*UpdateCommands)(void*); 
void (*BaseExecuteCommands)(void* weapon, WeaponCmd commands, float duration, float time, void* method); 
void (*old_ExecuteCommands)(void* weapon, WeaponCmd commands, float duration, float time, void* method);void ExecuteCommands(void* weapon, WeaponCmd commands, float duration, float time, void* method) { 
 if (silentaim) {  void* player = *(void**)((uint64_t) weapon + 0x18); 
  if (player) {   void* camholder = *(void**)((uint64_t) player + 0x20); 
   if (camholder) {    void* cam = get_transform(camholder); 
    if (cam) {     void* aimingdata = *(void **) ((uint64_t)*(void **)((uint64_t) player + 0x60) + 0x90); 
     if (aimingdata) {      Vector3 oldangles = get_eulerAngles(cam); 
           bool aimed = false; 
      bool wantaim = false;      
      if (silentaim && aimeds && commands.ToFire) {       BaseExecuteCommands(weapon, commands, duration, time, method); 
       UpdateCommands(weapon);       ihook( 
        (void*[]) {         (void*)getRealOffset(0x1CE1298), 
        },        (void*[]) { 
         (void*)set_angles_call, 
        },        1 
       );       wantaim = true; 
              if (CanShoot(weapon)) { 
        Vector3 shootpos = get_position(cam);        Vector3 aimangles = (Quaternion::LookRotation(aimedPlayerHeadPos - shootpos).euler() - 180).normalizedEuler(); 
        aimangles.z = 0;         
        set_eulerAngles(cam, aimangles);        set_eulerAngles(get_transform(get_camera()), aimangles); 
                ihook( 
         (void*[]) {          (void*)getRealOffset(0x38C402C), 
          (void*)getRealOffset(0x38C4150),          (void*)getRealOffset(0x38C4068), 
          (void*)getRealOffset(0x38C418C),          (void*)getRealOffset(0x1CE403C), 
          (void*)getRealOffset(0x1CE1298),         }, 
         (void*[]) {          (void*)set_angles_call, 
          (void*)set_angles_call, 
          (void*)set_angles_call,          (void*)set_angles_call, 
          (void*)recoil_call,          (void*)set_angles_call, 
         },         6 
        );        aimed = true; 
       } 
      }      
      old_ExecuteCommands(weapon, commands, duration, time, method);       
      if (wantaim) {       ihook( 
        (void*[]) {          
        },        (void*[]) { 
          
        },        0 
       ); 
      }      if (aimed) { 
       set_eulerAngles(cam, oldangles);       set_eulerAngles(get_transform(get_camera()), oldangles); 
      }     } 
    }   } 
  } } 
 else {  old_ExecuteCommands(weapon, commands, duration, time, method); 
 }}
