# hse_hw3_chromhmm

## Ссылка на Google Colab: https://colab.research.google.com/drive/1Oj6mYW7BlaLcW-BULgdeeQC3jRHOgDQ2?usp=sharing
Если ссылка не будет работать, то на всякий случай код привожу в файлах "hse_hw3_chromhmm.py" и "hse_hw3_chromhmm.ipynb" в директории src.

Я выбрала клетки Dnd41.
### Гистоновые метки:
Метка | Файл
--- | ---
H2AFZ | wgEncodeBroadHistoneDnd41H2azAlnRep2.bam 
H3K27ac | wgEncodeBroadHistoneDnd41H3k27acAlnRep1.bam   
H3K27me3 | wgEncodeBroadHistoneDnd41H3k27me3AlnRep1.bam
H3K36me3 | wgEncodeBroadHistoneDnd41H3k36me3AlnRep1.bam
H3K4me1 | wgEncodeBroadHistoneDnd41H3k04me1AlnRep1.bam 
H3K4me2 | wgEncodeBroadHistoneDnd41H3k04me2AlnRep1.bam
H3K4me3 | wgEncodeBroadHistoneDnd41H3k04me3AlnRep1.bam
H3K79me2 | wgEncodeBroadHistoneDnd41H3k79me2AlnRep1.bam
H3K9ac | wgEncodeBroadHistoneDnd41H3k09acAlnRep1.bam
H3K9me3 | wgEncodeBroadHistoneDnd41H3k09me3AlnRep1.bam

Файл с контрольным экспериментом: wgEncodeBroadHistoneDnd41ControlStdAlnRep1.bam

### Картинки из выдачи ChromHMM:
![emissions_12](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/8b85341c-831f-4ae4-80b9-9ee64a3d38bc)
![Dnd41_12_overlap](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/a10fb599-58b4-4da5-babd-3d0be5871c35)
![Dnd41_12_RefSeqTSS_neighborhood](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/b24887db-088f-48d3-a060-d006a5502523)
![Dnd41_12_RefSeqTES_neighborhood](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/68db1c6b-e1d0-42fc-8279-0ee518f99986)
![transitions_12](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/989adcab-4839-437a-aa2d-d90bbaad2a69)

Далее я выполнила бонусное задание и получившийся новый файл *_dense.bed загрузила в UCSC Genome Browser.
### Выбрала нужный тип клеток и гистоновые метки:
![Screenshot_20240324_112933](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/01e16917-e837-4b49-8461-c2f36222f580)
![Screenshot_20240324_113010](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/16bc169d-2b2e-4128-a776-86006ca4bfcf)

### Эпигенетические типы

Номер | Название | Характерная эпигенетическая метка | Другие свойства
--- | --- | --- | ---
1 | Active Promoter | 

