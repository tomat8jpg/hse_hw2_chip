# hse_hw2_chip
Ссылка на коллаб - https://colab.research.google.com/drive/1-OPFkVOliGIt7k0emYfyZ4Axu81LgpSa?usp=sharing  
Клеточная линия H1, гистоновая метка H3K4me3
# FastQC
Реплика 1 (ENCFF156FYC.fastq) и реплика 2 (ENCFF654NIP.fastq)
Было 	ENCFF156FYC.fastq:  
![image](https://user-images.githubusercontent.com/60805733/157036128-bf46f37f-1a4f-426c-97a8-f8d181fcf615.png)
![image](https://user-images.githubusercontent.com/60805733/157036154-e8cc8f69-3849-431b-b0ca-efef7849c04c.png)
![image](https://user-images.githubusercontent.com/60805733/157036170-88b512ff-57c6-4def-b599-f3b3c0f14717.png)
![image](https://user-images.githubusercontent.com/60805733/157036222-f12f3378-bf50-4b54-b3c8-4c7f7527030d.png)
![image](https://user-images.githubusercontent.com/60805733/157036245-461a797c-0927-408b-a1c9-e0eb94ccae1f.png)
Стало после подрезания	ENCFF156FYC.fastq:  
![image](https://user-images.githubusercontent.com/60805733/157036277-f040ef55-6800-4e53-a1cf-c7c5fc8a524c.png)
![image](https://user-images.githubusercontent.com/60805733/157036298-0315a3b8-b6d5-4770-b4c5-1774a56459f3.png)
![image](https://user-images.githubusercontent.com/60805733/157036315-482db460-c29e-4f00-8984-018814da9e07.png)
![image](https://user-images.githubusercontent.com/60805733/157036356-622b9a50-9f9e-433a-8f6b-029587f11418.png)
![image](https://user-images.githubusercontent.com/60805733/157036370-1ffa35c6-eecb-4380-81c9-f47a94e39cbc.png)

Было ENCFF654NIP.fastq (можно и не подрезать):  
![image](https://user-images.githubusercontent.com/60805733/157036497-9783cacf-3fb6-4345-a488-cf07d8792651.png)
![image](https://user-images.githubusercontent.com/60805733/157036537-3d6adbbd-6fba-4057-b928-053f5f5ef2e7.png)
![image](https://user-images.githubusercontent.com/60805733/157036548-86a1630b-7cd8-4a21-96ef-ba72490f3b18.png)
![image](https://user-images.githubusercontent.com/60805733/157036591-f7a965f0-0b28-43f7-9c78-bbede455ed89.png)

Контроль 	ENCFF191QXK.fastq (можно и не подрезать):  
![image](https://user-images.githubusercontent.com/60805733/157036822-55fe701a-f2f8-4f54-b326-4116925fb582.png)
![image](https://user-images.githubusercontent.com/60805733/157036866-90ca2ff5-aa01-4767-a976-b1077eaebc2c.png)
![image](https://user-images.githubusercontent.com/60805733/157036878-c8170142-b17a-4152-b414-5b02270a23f1.png)
![image](https://user-images.githubusercontent.com/60805733/157036908-bc388f23-db6d-47a9-80a9-3a116f6db59a.png)

# Выравнивание на хромосому. Сравнительная таблица  
![image](https://user-images.githubusercontent.com/60805733/157049103-b0f400cb-67aa-4c36-a335-cbba8dbc5556.png)
Мы видим очень низкий процент выравниваний, т.к. производилось выравнивание только на одну хромосому (а у нас 23 пары)  

# Сравнение результатов, диаграммы Венна  
Для реплики 1 (NA_peaks = ENCFF156FYC)
![image](https://user-images.githubusercontent.com/60805733/157046435-f58509c0-6dda-4895-8d84-0140bbee5dbb.png)
![image](https://user-images.githubusercontent.com/60805733/157046469-936ba5aa-8b98-4a64-bce7-c8446a3069f0.png)
Для реплики 2 (NA_peaks = ENCFF654NIP)
![image](https://user-images.githubusercontent.com/60805733/157046585-ccb28c76-5070-4a51-952e-00202a8031bf.png)
![image](https://user-images.githubusercontent.com/60805733/157046614-cf3fbac7-40f2-40c8-a4d1-48f4b9687f5a.png)
Диаграмма Венна показывает количество пересечений между нашими пиками и пиками в ENCODE. При этом при прямом и обратном сравнении количество пересечений неодинаково. Это связано с порядком анализа пиков: сначала считается число пиков в первом файле, которые имеются во втором. При изменении порядка изменится количество пересечений.
Количество пересечений небольшое, т.к. пиков изначально получилось не много из-за выравнивания на одну хромосому.
