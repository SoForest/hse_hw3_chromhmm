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

Номер | Название | Характерная эпигенетическая метка | Другие свойства | Картинка
--- | --- | --- | --- | --- 
1 | Active Promoter | H3K27me3 | Часто находится на ядерной ламине, то есть попадает на участки репрессированного хроматина, попадает как на интроны, так и на экзоны | ![Screenshot_20240324_122501](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/03a53e92-113c-403b-a091-310db1bd7baa)
2 | Weak Promoter | В выдаче ChromHMM не указаны | Часто находится на ядерной ламине, то есть попадает на участки репрессированного хроматина, попадает в основном на интроны | ![Screenshot_20240324_122704](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/943a7195-40a0-4d19-9dd3-4fba60311e0a)
3 | Inactive/poised_Promoter | H3K9me3 | Часто находится на ядерной ламине, то есть попадает на участки репрессированного хроматина | ![Screenshot_20240324_123327](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/735eaf1c-346a-4c6c-8921-502591aec561)
4 | Strong_enhancer | H3K36me3 | Часто попадает на экзоны, на RefSeq TES | ![Screenshot_20240324_124940](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/5a3e2469-c43f-40e2-8833-2e9638a09709)
5 | Strong_enhancer | H3K79me2, H3K36me3 | Попадает на экзоны или интроны, на RefSeq TES | ![Screenshot_20240324_125610](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/4a482235-0a03-470f-a1ab-3de5fc86cde0)
6 | Weak/poised_enhancer | H3K79me2 | Попадает на экзоны или интроны | ![Screenshot_20240324_125856](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/e15a1325-8018-4327-9b9e-ec99c3e66631)
7 | Weak/poised_enhancer | H3K79me2, H3K4me1, H3K4me2, H3K36me3 | Попадает на экзоны или интроны, на RefSeq TES | ![Screenshot_20240324_130020](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/c923cf71-17c9-4132-a666-d4a87ff7dd64)
8 | Insulator | H3K27ac, H3K9ac, H3K4me3, H3K4me2, H3K4me1, H3K79me2 | Попадает на CpG-островки, часто на экзоны, на RefSeq TES, RefSeq TSS | ![Screenshot_20240324_130210](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/254a05c7-17c0-4dfc-80ad-c923740ed69e)
9 | Transcriptional_transition | H3K27ac, H3K9ac, H2AFZ, H3K4me3, H3K4me2, H3K4me1, H3K79me2 | Попадает на CpG-островки, часто на экзоны, на RefSeq TES, RefSeq TSS | ![Screenshot_20240324_132434](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/d1a07a63-ccc5-43b4-9f90-b58228e6a600)
10 | Transcriptional_elongation | H3K27ac, H3K9ac, H3K4me1 | Попадает на RefSeq TES, на ядерную ламину | ![Screenshot_20240324_132721](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/c6cf834a-02b2-49a2-8456-1656eeddae9b)
11 | Weak_transcribed | H3K4me1, H3K27ac | Может попадать на ядерную ламину, на RefSeq TES | ![Screenshot_20240324_125158](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/ee090e3c-3ea5-4d7e-b0df-8592b082ba61)
12 | Polycomb-repressed | H3K4me2, H3K4me1 | Попадает как на интроны, так и на экзоны. Может попадать на CpG-островки, на RefSeq TES и RefSeq TSS | ![Screenshot_20240324_124705](https://github.com/SoForest/hse_hw3_chromhmm/assets/145841508/d0ebc7cf-1a6c-440f-899e-dc236a528abd)

### Бонусное задание:
```bash
from google.colab import files
import os

states = ['Active_Promoter',
          'Weak_Promoter',
          'Inactive/poised_Promoter',
          'Strong_enhancer',
          'Strong_enhancer',
          'Weak/poised_enhancer',
          'Weak/poised_enhancer',
          'Insulator',
          'Transcriptional_transition',
          'Transcriptional_elongation',
          'Weak_transcribed',
          'Polycomb-repressed']

with open('Dnd41_12_dense.bed', 'r') as f:
  with open('Dnd41_12_dense_new.bed', 'a') as new_f:
    lines = f.readlines()
    new_f.write(lines[0])
    for line in lines[1:]:
        l = line.split('\t')
        l[3] = l[3] + '_' + states[int(l[3]) - 1]
        new_f.write('\t'.join(l))
```


