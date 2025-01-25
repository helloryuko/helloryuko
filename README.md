<a title='j++' href='https://github.com/jppteam'>
  <picture>
    <source media='(prefers-color-scheme: dark)' srcset='https://i.imgur.com/HXltrQC.png' alt='работник ж++ (белый) (не расизм)' width='200px'/>
    <img src='https://i.imgur.com/iJuMeH0.png' alt='работник ж++ (черный) (не расизм)' width='200px'/>
  </picture>
</a>

выыфшщы
<img src="https://github.com/user-attachments/assets/78ef06c4-9ee2-4093-a36a-562353862a7e" width=100>

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
 ![image](https://github.com/user-attachments/assets/46bcff48-70c1-4816-a5c7-4da3cb62d025)

<h1>

 😳 Очнись! Думаешь, ты в безопасности?

Убийства, кражи, изнасилования— всё это происходит на улицах твоего города ежедневно.

Читатели наших каналов сами скидывают нам эксклюзивные видео БЕЗ ЦЕНЗУРЫ и мы публикуем их в общий доступ.

Ищи свой город и следи за этой вакханалией👇

— Москва  
— Санкт-Петербург  

— Архангельск  
— Астрахань 
— Барнаул 
— Белгород 
— Брянск 
— Великий Новгород  
— Владивосток 
— Волгоград 
— Вологда  
— Воронеж 
— Владимир  
<img src="https://github.com/user-attachments/assets/79c3a756-8b06-49bc-ac0b-e051b9b705fe" width=600>
<img src="https://github.com/user-attachments/assets/8c97745f-1dd0-4e7c-90dc-b1a9f1d923d0" width=600>

— Екатеринбург 
— Ижевск 
— Иркутск 
— Иваново   
— Йошкар-Ола 

— Кавказ   
— Казань 
— Калининград   
— Калуга  
— Кемерово 
— Киров 
— Кострома  
— Красноярск 
— Краснодар 
— Крым | Севастополь 
— Курган   
— Курск   

— Липецк  
— Мурманск  
— Нальчик 
— Нижний Новгород  
— Новосибирск 

— Омск 
— Орел  
— Оренбург 
— Пенза 
— Пермь 
— Псков  
— Ростов-на-Дону  
— Рязань 

— Самара 
— Саратов 
— Саранск  
— Смоленск   
— Сочи 
— Ставрополь  
— Сургут и ХМАО  

— Тамбов   
— Тверь   
— Тольятти 
— Томск 
— Тула  
— Тюмень 
— Улан-Удэ  
— Ульяновск 
— Уфа 

— Хабаровск 
— Челябинск 
— Чита   
— Чувашия 
— Якутск  
— Ярославль 
</h1>

![image](https://github.com/user-attachments/assets/580b6eab-770b-4d47-b690-d5b364dc8e66)
