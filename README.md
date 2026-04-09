> **MEMORANDUM**
> Should the reader of this document experience difficulty in comprehending the informal style of presentation, said individual is directed to refer to the [READMESIR.md](READMESIR.md) file for further information.

<a title='j++' href='https://github.com/jppteam'>
  <picture>
    <source media='(prefers-color-scheme: dark)' srcset='https://i.ibb.co/PsQRJskM/Logo.png' alt='работник ж++ (белый) (не расизм)' width='200px'/>
    <img src='https://i.ibb.co/R4cVvd4N/Logo-1.png' alt='работник ж++ (черный) (не расизм)' width='200px'/>
  </picture>
</a>
<img width="1379" height="166" alt="MS Paint _ Microsoft Paint Online(7)" src="https://github.com/user-attachments/assets/2800fa99-5e3c-489c-a583-e8b4e1df85d4" />

![Untitled](https://github.com/user-attachments/assets/c91fe845-b355-4353-90bd-5877bef31a42)
выыфшщы
<img src="https://github.com/user-attachments/assets/78ef06c4-9ee2-4093-a36a-562353862a7e" width=100>



привет lhepmz
<div align='right'>
<img src="https://github.com/user-attachments/assets/88a532c4-60f9-4352-9fa0-f8f97dc0d24a" width=320>
</div>

<img width="594" height="534" alt="image" src="https://github.com/user-attachments/assets/5a3a2c81-f9e4-4b0e-a843-8713e214026d" />

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

<a href="https://ibb.co/j9SSTJwf"><img src="https://i.ibb.co/wZffRcQg/IMG-20260206-161401-489.jpg" alt="IMG-20260206-161401-489" border="0"></a>

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
![image](https://github.com/user-attachments/assets/ae7bc18b-6db6-46c2-89d7-35634baf8daf)

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
<img src="https://github.com/user-attachments/assets/40bafc75-0c34-442d-818e-557b0eb34f74" width=600>
<img src="https://github.com/user-attachments/assets/178c97c2-2f8b-4b69-b22d-24b2aec6dad4" width=600>

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
— Крым | Севастополь (украинсикй)
— Курган   
— Курск   (КНР)

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
![image](https://github.com/user-attachments/assets/580b6eab-770b-4d47-b690-d5b364dc8e66)
</h1>

Изначально утвердим твое положение в данном разговоре. Ты же ебучий lame без Rick Owens Geobasket, Rick Owens Cargobasket. Ты хочешь взять мою фишку. 1) Ты без скита (uid 1337 можешь пмнуть ну давай-давай-давай пмни меня уебан), без турбера, без ровера, без свэгги. У тебя джуганная swagga парень. Кстати о джуганном, дж = g знаешь где эта буква встречается? Правильно это же мои кросовки Rick Owens Geobasket которых у тебя никогда не будет, у тебя нету раста в стиме он стоит 1200 рублей Rick Owens Geobasket стоят 1400 евро о каких деньгах может идти речь если ты нищий, нищий кста напомню чего у тебя еще нету это : айдишки скита риковенс геобаскет риковенс каргобаскет у тебя нету коннекта с шайни коннекта с аглистефаном по краней мере хотя бы с Melon Gang, если ты думаешь что у тебя есть нелегит Rick Owens Рамоны (XDDDDDDDDDDDDDD) и ты можешь настроить со мной какую либо коммуникацию то я тебя разочарую с такими ебаными broуками как ты я даже разговаривать не стану. Знай свое место обдроченный салом петухъ который обязан сейчас понимать что человек (то есть я) который имеет 1) Rick Owens Geobasket
(2 пары)
2) Rick Owens Cargobasket (2 пары)
3) Айдишку (@vampire, @king, @rickowens, кста гетни се хоть что то уже аууу xD)
4) Турбер
5) Ровер
6) Парсер
https://github.com/user-attachments/assets/c8d1055d-0401-46b3-99a4-aaeb028a6cbb

![IMG_7278](https://github.com/user-attachments/assets/0e7429f7-ed90-4748-858b-0350f4fac03e)

<img width="739" height="985" alt="image" src="https://github.com/user-attachments/assets/628b32d3-3108-487e-9874-22d4dc048854" />

7) Свеггу ( у тебя она конкретно джуганная + хэшанная + не легит риковенс + ты нищий + без айди + без скита + без турбера + без ровера + без парсера + без денег + без айдишки + без братишки)
8) Парсер (8к евро)
9) 4 ляма евро на балансе
И ты реально думаешь что после того что я тебе в данный момент времени и пространства пишу ты можешь мне хоть что то сделать человеку который настолько богат что может каждый день себе покупать по заводу по производству кроссовок отличного качества "Rick Owens"?
Я задам тебе простой вопрос: - когда ты меня уже сможешь пмнуть в ските ало безскитовое уебище ебанно

![image](https://github.com/user-attachments/assets/56b8bd61-d28d-45d8-9a06-0edfcc2d0d2d)



![PXL_20251022_010955803](https://github.com/user-attachments/assets/e1eb1eb0-bb8e-404e-aa25-2a17f046adac)
(я в юбочке миленькая :з бабло кстати тоже моё а между ножек мой мальчик миленький хехехехеее)
