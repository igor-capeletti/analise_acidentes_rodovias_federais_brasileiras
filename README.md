# Análise de dados dos acidentes de trânsito ocorridos nas rodovias federais do Rio Grande do Sul


No presente trabalho serão analisados os dados e respondidas questões sobre os acidentes acontecidos no Estado do Rio Grande do Sul nos anos de 2007 até 2020.


## Aquisição dos dados
Os conjuntos de dados correspondem ao período de 2007 a 2020 e foram disponibilizados através da [plataforma Kaggle](https://www.kaggle.com/mcamera/brazil-highway-traffic-accidents). Estes foram extraídos diretamente do [website da PRF](https://www.gov.br/prf/pt-br/acesso-a-informacao/dados-abertos/dados-abertos-acidentes).

Esses dados são divididos em arquivos .CSV anuais e o ultimo arquivo (ano atual) é atualizado mensalmente.

Os dados são disponibilizados em 3 grupos:

1. Agrupados por ocorrencia - (arquivos como datatranANO.csv)
2. Agrupados por pessoa - (arquivos como acidentesANO.csv)
3. Agrupados por pessoa - Todas as causas e tipos de acidentes (a partir de 2017) - (arquivos como acidentesANO\_todascausas\_tipos)

**Para o presente trabalho, utilizaremos os dois primeiros conjuntos de dados.**

Os dados são provenientes dos sistemas BR-Brasil e Boletim de Acidente de Trânsito (BAT), com as seguintes considerações:
* O sistema BR-Brasil foi usado em nivel nacional entre 2007 a 2016. Os acidentes foram armazenados usando o sistema BR-Brasil. Nesse sistema o policial responsável pela ocorrencia insere os dados relacionados aos involvidos, localização, veículos e a dinâmica do acidente.


## Download dos arquivos:
* [Arquivos de execução em formato Jupyter Notebook(.ipynb)](https://github.com/igor-capeletti/analise_acidentes_rodovias_federais_brasileiras)
* [Arquivos para as análises(.csv)](https://drive.google.com/file/d/1pBDrDMnYS9oeQ-o14GWVmBsCNlYverG5/view?usp=sharing)


## Instalação do Python, Pip e Jupyter Notebook:
### Windows:
  * [Python3](https://python.org.br/instalacao-windows)
  * Você poderá instalar somente o [Jupyter Notebook](https://jupyter.org/install) ou o pacote completo [Anaconda](https://www.anaconda.com/)

### Linux:
  * As versões Linux mais atuais já possuem o Python3 instalado, mas você pode baixar e instalar nas versões anteriores utilizando os os seguintes comandos:
  ```
  sudo apt-get install python3
  ```
  e também:
  ```
  sudo apt-get install python3-pip
  ```
  * Pode seguir o tutorial do [Jupyter Notebook](https://jupyter.org/install) ou executar:
  ```
  sudo pip install notebook
  ```
### Mac:
  * [Python3](https://www.python.org/downloads/macos)
  * Você poderá instalar somente o [Jupyter Notebook](https://jupyter.org/install) ou o pacote completo [Anaconda](https://www.anaconda.com/)

## Instalação de Bibliotecas:
  * Pandas e Numpy para tratamento dos dados;
  * Seaborn, Matplotlib e Folium para geração dos gráficos;
  ```
  sudo pip3 install -r requirements.txt
  ```

## Execução dos experimentos:
1. Você precisa extrair o arquivo [arquive](https://drive.google.com/file/d/1pBDrDMnYS9oeQ-o14GWVmBsCNlYverG5/view?usp=sharing) zipado e colocar na mesma pasta dos arquivos **.ipynb**.

2. Abrir o Jupyter Notebook ou o Anaconda e acessar os arquivos **.ipynb**.

3. Você poderá executar somente o arquivo **acidentes_br.ipynb** para visualizar as análises. Os arquivos **data_cleaning_ocorrencia.ipynb** e **data_cleaning_pessoas.ipynb** são referentes à limpeza e normalização dos dados originais.  

## Alguns gráficos gerados:
<img src="https://github.com/igor-capeletti/analise_acidentes_rodovias_federais_brasileiras/blob/main/img/mapa_calor_acidentes_nas_rodovias.png"/>

---

<img src="https://github.com/igor-capeletti/analise_acidentes_rodovias_federais_brasileiras/blob/main/img/download.png"/>

---

<img src="https://github.com/igor-capeletti/analise_acidentes_rodovias_federais_brasileiras/blob/main/img/dias_da_semana_com_acidentes_por_ano.png"/>

---

<img src="https://github.com/igor-capeletti/analise_acidentes_rodovias_federais_brasileiras/blob/main/img/acidentes_por_horario_do_dia.png"/>

---

<img src="https://github.com/igor-capeletti/analise_acidentes_rodovias_federais_brasileiras/blob/main/img/acidentes_por_hora_e_dia.png"/>

---

<img src="https://github.com/igor-capeletti/analise_acidentes_rodovias_federais_brasileiras/blob/main/img/motivos_que_levaram_aos_acidentes.png"/>

---

<img src="https://github.com/igor-capeletti/analise_acidentes_rodovias_federais_brasileiras/blob/main/img/acidentes_por_faixa_etaria_dos_motoristas.png"/>
