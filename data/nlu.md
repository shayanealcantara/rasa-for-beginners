## intent:dor_de_cabeca <!--- The label of the intent -->
  - Estou com dor de cabeça
  - Tô com dor de cabeça
  - Dor de cabeça
  - Enxaqueca
  - Estou com enxaqueca
  - Cefaleia
  - dor de cabeça e [enjoo](other_symptoms)
  - dor de cabeça e [vomito](other_symptoms)

## intent:dor_torax
  - dor no peito
  - dor no petio
  - Estou com dor no peito
  - dor torácica
  - peso no peito
  - dor no peto
  - peso no peto

## intent:dor_abdomen
  - dor na barriga
  - dor de barriga
  - irritação na barriga
  - dor no pé da barriga
  - dor no estômago
  - cólica
  - cólica intestinal
  - cólica menstrual
  - dor no bucho
  - dor de lado
  - dor desviada
  - dor no lado direito da barriga
  - dor no lado esquerdo da barriga
  - dor na barriga e [cansaço](other_symptoms)
  - dor no umbigo
  - Estou com dor na barriga
  - Estou com dor de barriga
  - To com dor na barriga
  - To com a barriga irritada

## intent:sintomas_gripais
  - tosse
  - Tosse
  - Tosse e dor de garganta
  - Estou com resfriado
  - Estou gripado
  - Estou com dor de garganta
  - Estou tossindo muito
  - Estou com muita dor de garganta
  - Estou com febre e dor de garganta
  - Estou tossindo sem conseguir respirar
  - Estou tossindo e com dor no corpo
  - Estou com tosse e cansaço
  - Estou tossindo e com fraqueza
  - Estou com tosse e dor nos músculos
  - Estou com calafrios e tosse
  - Estou gripada
  - Estou resfriado
  - Estou resfriada
  - gripe
  - resfriado
  - Tosse e nariz escorrendo

## intent:outros_sintomas <!--- The label of the intent -->
  - nausea
  - Naúsea
  - Enjoo
  - Ânsia
  - Ansia
  - dor no pescoço
  - estou enjoado
  - estou com tontura
  - estou enjoada
  - dor na nuca
  - suor
  - suor frio
  - suando frio
  - irradiação
  - cansaço
  - diarreia
  - diarréia
  - vômito
  - Estou me sentindo [cansado](other_symptoms:cansaço)
  - Estou me sentindo [cansada](other_symptoms:cansaço)
  - Estou me sentindo [prostrado](other_symptoms:cansaço)
  - Estou me sentindo [prostrada](other_symptoms:cansaço)
  - Tô [cansada](other_symptoms:cansaço)
  - Estou [vomitando](other_symptoms:vômito)
  - Estou com [diarreia](other_symptoms:diarreia)
  - inchaço na barriga
  - Estou me sentindo [inchado](other_symptoms:inchaço)

## intent: sim
  - sim
  - isso
  - positivo

## intent:negativo
  - não
  - nada
  - nadinha
  - de forma alguma
  - nenhum
  - nenhuma

## regex:vital
  - ([0-9]{2}.[0-9])

## regex:height
  - ([0-1].[0-9]{2})

## intent:dados
  - estes são meus sinais vitais {(data)}
  - estes são meus sinais vitais {'temperature': [vital], 'blood_oxygen_level': [vital]}
  - estes são meus sinais vitais {'temperature': 38.0, 'blood_oxygen_level': 95.0}
  - estes são meus sinais vitais {'temperature': 36.0, 'blood_oxygen_level': 92.0}
  - estes são meus sinais vitais {'temperature': 36.5, 'blood_oxygen_level': 93.0}
  - estes são meus sinais vitais {'temperature': 40.0, 'blood_oxygen_level': 90.0}
  - estes são meus sinais vitais {'temperature': 39.5, 'blood_oxygen_level': 91.0}
  - estes são meus sinais vitais {'temperature': 37.5, 'blood_oxygen_level': 97.0}
  - estes são meus sinais vitais {'temperature': 35.0, 'blood_oxygen_level': 89.0}
  - estes são meus sinais vitais {'height':[height], 'body_mass': 53}
  - estes são meus sinais vitais {'height': 1.70, 'body_mass': 100}
  - estes são meus sinais vitais {'height': 1.48, 'body_mass': 60}
  - estes são meus sinais vitais {'height': 1.58, 'body_mass': 53}
  - estes são meus sinais vitais {'height': 1.80, 'body_mass': 80}
  - estes são meus sinais vitais {'height': 1.65, 'body_mass': 67}
  - estes são meus sinais vitais {'height': 1.58, 'body_mass': 53}
  - estes são meus sinais vitais {'blood_pressure': "\[\"120\", \"81\"\]"}
  - estes são meus sinais vitais {'blood_pressure': "\[\"170\", \"81\"\]"}

## intent:escala_de_dor
  - [dez](pain_scale:10)
  - [nove](pain_scale:9)
  - [oito](pain_scale:8)
  - [sete](pain_scale:7)
  - [seis](pain_scale:6)
  - [cinco](pain_scale:5)
  - [quatro](pain_scale:4)
  - [três](pain_scale:3)
  - [tres](pain_scale:3)
  - [dois](pain_scale:2)
  - [um](pain_scale:1)

## intent:persistencia_dor
  - [constante](pain_persistance:constant)
  - [insistente](pain_persistance:constant)
  - [grande](pain_persistance:constant)
  - [muita](pain_persistance:constant)
  - [súbito](pain_persistance:not_constant)
  - [vai e volta](pain_persistance:not_constant)
  - [toda hora](pain_persistance:constant)
  - [progressiva](pain_persistance:not_constant)
  - [de repente](pain_persistance:not_constant)
  - a dor é [constante](pain_persistance:constant)
  - a dor [não vai embora](pain_persistance:constant)
  - a dor [não para](pain_persistance:constant)
  - [vai e vem](pain_persistance:not_constant)
  - a dor [vai e vem](pain_persistance:not_constant)
  - some as [vezes](pain_persistance:not_constant)

## intent:intoxicacao
  - eu tomei (substancia)
  - eu engoli (substancia)
  - tomei (substancia)
  - engoli (substancia)
  - tomei uma caixa de (substancia)
  - eu tomei veneno
  - tomei mais comprimidos do que deveria
  - tomei muito comprimido
  - tomei a dosagem errada do meu remédio
  - tomei a dosagem errada
  - eu confundi o remédio
  - confundi o remédio
  - confundi meu remédio
  - inalei produto de limpeza
  - respirei muito produto de limpeza
  - inalei (substancia)
  - respirei (substancia)

## regex:age_number
- ([0-9]{3})

## intent:idade
 - Qual é a sua idade? [1](age)
 - Qual é a sua idade? [3](age)
 - Qual é a sua idade? [14](age)
 - Qual é a sua idade? [60](age)
 - Qual é a sua idade? [8](age)
 - Qual é a sua idade? [99](age)
 - Qual é a sua idade? [23](age)
 - Qual é a sua idade? [85](age)
 - Qual é a sua idade? [45](age)
 - Qual é a sua idade? [32](age)
 - Qual é a sua idade? [age_number](age)
 - Qual é a sua idade? Minha idade é [age_number](age)
 - Qual é a sua idade? Tenho [age_number](age) anos
 - Qual é a sua idade? Tenho [age_number](age)

 ## regex:medication_name
 - ([a-z]{50})

 ## intent:dor_torax
   - dor no peito
   - Estou com dor no peito
   - dor torácica
   - peso no peito

 ## intent:dados_recebidos
   - dados iniciais recebidos
   - dados recebidos
   - Os dados foram salvos na aplicação da estação da triagem.

## regex:alergie_name
 - ([a-z]{60})

##intent:alergias
- Você possui alergia a alguma medicação? Se sim, cite a quais. [Não](alergies:False) tenho alergia
- Você possui alergia a alguma medicação? Se sim, cite a quais. [não](alergies:False) tenho alergia
- Você possui alergia a alguma medicação? Se sim, cite a quais. [Não](alergies:False)
- Você possui alergia a alguma medicação? Se sim, cite a quais. [Não](alergies:False) tenho
- Você possui alergia a alguma medicação? Se sim, cite a quais. [buspirona](alergies)
- Você possui alergia a alguma medicação? Se sim, cite a quais. [galvus](alergies)
- Você possui alergia a alguma medicação? Se sim, cite a quais. [adenpas](alergies)
- Você possui alergia a alguma medicação? Se sim, cite a quais. [aloxidil](alergies)
- Você possui alergia a alguma medicação? Se sim, cite a quais. [sinvastatina](alergies)
- Você possui alergia a alguma medicação? Se sim, cite a quais. [reducofem](alergies)
- Você possui alergia a alguma medicação? Se sim, cite a quais. [amoxilina](alergies)
- Você possui alergia a alguma medicação? Se sim, cite a quais. [amoxicilina](alergies)
- Você possui alergia a alguma medicação? Se sim, cite a quais. [sertralina](alergies)
- Você possui alergia a alguma medicação? Se sim, cite a quais. [ziprazidona](alergies)
- Você possui alergia a alguma medicação? Se sim, cite a quais. [alergie_name](alergies)
- Você possui alergia a alguma medicação? Se sim, cite a quais. Tenho alergia a [remedio](alergies)
- Você possui alergia a alguma medicação? Se sim, cite a quais. Tenho alergia a [remédio](alergies)
- Você possui alergia a alguma medicação? Se sim, cite a quais. Tenho alergia a [alergie_name](alergies)
- Você possui alergia a alguma medicação? Se sim, cite a quais. Tenho alergia a [alergie_name](alergies)
