# Домашнее задание к занятию «ОС Windows (часть 1)»


В качестве результата пришлите ответы на следующие вопросы:
1. Какой процесс отображается в логе первым? Какой у него PID?
2. Какой "драйвер" загружается первым? Что это за драйвер (ответьте своими словами)?
3. Какой PID у родительского процесса для smss.exe (не у самого smss.exe, а у того, кто его создал)?
4. Какой процесс является родительским для процесса winlogon.exe? Где расположен файл winlogon.exe? 
5. Какой процесс является родительским для процесса lsass.exe?
6. Что будет если в таск менеджере (taskmgr.exe) завершить работу следующего процесса:

![](pic/taskmgr.png)

### Ответы:

1. В логе первым отображается процесс SYSTEM его PID 4

![1](https://user-images.githubusercontent.com/122460278/218973946-fdaa4ccc-ac2b-4d41-856e-2c17a2b6f5ef.png)


2. Первым загружается драйвер PROCMON24.SYS - этот драйвер устанавливает сам PROCESS MONITOR для мониторинга за состоянием системы


3. У родительского процесса для smss.exe PID 4

![6](https://user-images.githubusercontent.com/122460278/218982665-d4671e91-e3c3-42f3-be2d-413cabf4c9dd.png)


4. Родительским для процесса winlogon.exe является smss.exe так как его PID 484. winlogon.exe располагается по адресу C:\Windows\System32\winlogon.exe

![3](https://user-images.githubusercontent.com/122460278/218977182-93af804a-ece0-44a2-b92d-02c4aed0f666.png)


5. Для lsass.exe родительским является процесс c PID 492 - это wininit.exe

![4](https://user-images.githubusercontent.com/122460278/218980987-fc28e7d7-dcf2-4c52-a346-09256fc8af96.png)

![5](https://user-images.githubusercontent.com/122460278/218982027-c26452d5-34df-45fc-8839-fb341a1e118d.png)


6. В этом случае сессия текущего пользователя будет завершена и система предложит залогиниться заново


![VirtualBox_Windows10_15_02_2023_12_08_42](https://user-images.githubusercontent.com/122460278/218983586-3ed159d0-5c25-4d6f-8386-3834e488902b.png)






