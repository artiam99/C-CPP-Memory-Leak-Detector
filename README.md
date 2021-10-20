# C-CPP-Memory-Leak-Detector

This is C/C++ Memory Leak Detector Library. It maintains two databases - Structure Database and Object Database.

User Application registers all its structures with MLD Library at the time of initialization.

Whenever application xcalloc() an object , object record entry is inserted in object database.

If there is any Memory Leak in Application Code,  "report_leaked_objects()" function detects that Memory Leak.

### Compilation - 

gcc -g -c mld.c -o mld.o

gcc -g -c app.c -o app.o

gcc -g app.o mld.o -o exe

For testing modify app.c file. Create some memory leaks. Do compile as mentioned above. Run the exe file.

./exe

## High Level Design

![hld](https://user-images.githubusercontent.com/47227715/138093205-f614ac69-3056-4013-a48a-adf195bf3dfe.png)


## Testing MLD Library

![Screenshot (88)](https://user-images.githubusercontent.com/47227715/129093013-b998f506-de19-4222-96c8-be81e13d8393.png)

![Screenshot (89)](https://user-images.githubusercontent.com/47227715/129093018-2a518fb5-12d9-46de-b935-29afc8994097.png)

![Screenshot (90)](https://user-images.githubusercontent.com/47227715/129093029-ed8917fe-3642-4e11-9df0-106c4a1d6c40.png)

![Screenshot (85)](https://user-images.githubusercontent.com/47227715/129093080-47215fdc-713e-412d-890c-7f934dff7552.png)

![Screenshot (86)](https://user-images.githubusercontent.com/47227715/129093085-067dff81-4048-4e46-81f9-991e245f791b.png)

![Screenshot (87)](https://user-images.githubusercontent.com/47227715/129093149-3dfbb894-54a9-43cd-ab89-cad9d0dd60c9.png)
