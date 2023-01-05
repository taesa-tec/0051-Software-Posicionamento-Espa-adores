# 0051-Software-Posicionamento-Espacadores

<p align="center">
  <img src="http://img.shields.io/static/v1?label=License&message=MIT&color=green&style=for-the-badge"/>
   <img src="http://img.shields.io/static/v1?label=STATUS&message=CONCLUIDO&color=GREEN&style=for-the-badge"/>
</p>

![0051_Divulgaçãov3](https://user-images.githubusercontent.com/42223882/210839516-3bb0d777-347a-4a5c-99e3-aeec5a4b4be2.jpg)



### Tópicos 

:small_blue_diamond: [Descrição do projeto](#descrição-do-projeto)

:small_blue_diamond: [Objetivo do Programa](#objetivo-do-programa)

:small_blue_diamond: [Sobre o Programa](#sobre-o-programa)

:small_blue_diamond: [Entrada de dados](#entrada-de-dados)

:small_blue_diamond: [Como rodar a aplicação](#como-rodar-a-aplicação-arrow_forward)

:small_blue_diamond: [Análise dos Resultados](#análise-dos-resultados)



## Descrição do projeto 

<p align="justify">
O Projeto "Sistema Suporte e Espaçador - Dispositivo de suporte e amortecimento mecânico para cabos condutores em linhas de transmissão sujeitas à sobrecarga de operação", realizado em 2021 no âmbito do Programa de PDI ANEEL, teve como finalidade o desenvolvimento de uma solução segura para aumentar a capacidade de transmissão de energia elétrica, visando garantir a expansão do sistema elétrico a partir de instalações já existentes.
A capacidade de corrente de uma linha de transmissão (LT) é determinada pela temperatura máxima do condutor que garante distâncias mínimas contidas no projeto original da LT. Correntes mais altas ou dissipação menor de calor reduzem essas distâncias, afetando a continuidade de transmissão da linha e pondo em risco a integridade de terceiros.
<br>
O uso de dados estatísticos que norteia o despacho de LTs e cria ampacidades sazonais aumenta o risco de falhas das linhas de transmissão devido à violação da distância mínima entre as partes energizadas e as partes aterradas. Nesse sentido, a solução proposta por este projeto se faz importante, uma vez que permite a ampliação da capacidade de linhas de transmissão existentes, sem que haja problemas de violação das distâncias de segurança pelos cabos condutores.  </p>

## Objetivo do Programa
<p align="justify">
O programa foi criado com a finalidade última de levantar o número de espaçadores e sua posição no vão analisado. Para atingir esse objetivo, foram introduzidas funcionalidades no programa “Spacer Position” para facilitar a rápida análise das diversas variáveis envolvidas. Toda a interface do programa foi desenvolvida de tal forma a facilitar a operação do programa pelo usuário.
<br>
O programa também demanda de um equipamento de pouca capacidade para a sua execução, portanto, a arquitetura e o algoritmo foram desenvolvidos para a rápida execução sem ocorrência de travamentos ou problemas correlatos.
</p>

## Sobre o Programa
<p align="justify">
O programa Spacer Position, foi programado utilizando a linguagem LabVIEW (acrônimo para Laboratory Virtual Instrument Engineering Workbench). O LabVIEW é uma linguagem de programação gráfica originária da National Instruments. A primeira versão surgiu em 1986 para o Macintosh e atualmente existem também ambientes de desenvolvimento integrados para os Sistemas Operacionais Windows, Linux e Solaris.
<br>
O painel frontal do LabVIEW é um meio confortável para construir programas com uma boa interface gráfica. O programador não necessita de escrever qualquer linha de código. A apresentação gráfica dos processos aumenta a facilidade de leitura e de utilização.
<br>
O programa desenvolvido na linguagem descrita deve calcular a posição dos espaçadores desenvolvidos no âmbito do projeto em um determinado vão definido pelo operador. Para que isso seja possível, o programa deve ser alimentado com um conjunto de parâmetros.
</p>

## Entrada de dados
<p align="justify">
Os seguintes dados devem ser preenchidos nos controles separados por cinco itens, são eles: condutor, suporte, vão, subvãos e projeto. Cada um dos itens mencionados contém:
</p>
<ul><li> Condutor 
<ul><li>	Peso unitário (N/m) – Pc (N/m);
<li>	Módulo de Young (N/m²) – Mod.Young (N/m²);
<li>	Coeficiente de Dilatação térmica linear (1/°C) – Dil.Term.c (1/°C);
<li>	Seção transversal (mm²) – Seção trans. (mm²);
<li>	Tração horizontal EDS (N).
</ul><br>
<li> Cabo Suporte 
<ul><li>	Peso unitário (N/m) – Ps (N/m);
<li>	Módulo de Young (N/m²) – Mod.Young (N/m²);
<li>	Coeficiente de Dilatação térmica linear (1/°C) – Dil.Term.c (1/°C);
<li>	Seção transversal (mm²) – Seção trans. (mm²);
<li>	Tração horizontal EDS (N).
</ul><br>
<li> Vão 
<ul><li>	Comprimento do vão (m);
<li>	Desnível (m).
</ul><br>
<li> Subvão
<ul><li>	Extensão limite (m)</ul>
<br>
<li> Projeto
<ul><li>	Temperatura EDS (°C);
<li>	Limite original (°C);
<li>	Limite estendido (°C);
<li>	N° de cabos por fase. - N° Cabo/Fase</ul></ul>
<br>

## Como rodar a aplicação :arrow_forward:
<p align="justify">
O primeiro arquivo a ser aberto: "Spacer Position.lvproj"
<br> O arquivo principal é o chamado "Spacer Position.vi", para rodá-lo basta clicar no menu/run ou CTRL+R para a tela inicial do programa.
<br>
Na tela inicial do programa existem quatro linhas divididas em cinco seções, a fim de facilitar o preenchimento de dados, são elas: condutor, suporte, vão e subvão e projeto. 
<br>
Assim que o programa é iniciado, a primeira linha fica habilitada, disponível para o preenchimento. Para se preencher a segunda linha de dados, logo abaixo, deve-se acionar a tecla “Próximo” e assim sucessivamente até a quarta e última linha de dados, chamada “Projeto”. 
<br>
Esse procedimento é realizado para maximizar o foco no preenchimento por itens de mesma natureza, o que minimizar a ocorrência de erros no processo de preenchimento dos dados entrada.
Cada campo é autoexplicativo, para que não haja dúvidas durante o preenchimento dos espaços, bastando apesar pousar a seta indicadora por um segundo que em seguida, um quadro com as dicas de preenchimento será apresentado ao usuário.
<br>
Ao final surge uma mensagem de confirmação a qual questiona o correto preenchimento dos dados por parte do usuário. Caso haja algum erro, o processo se inicia novamente, voltando a primeira na linha superior, e conforme é pressionada a tecla “Próximo”, as linhas são varridas novamente de cima para baixo. 
<br>
Ao final do processo, o operador é inquirido novamente sobre o preenchimento. Uma vez os dados aceitos, ao selecionar “sim”, o programa segue para a próxima tela. 
<br> Para o preenchimento dos dados dos cabos e do vão, com a tecla de atalho Page Down é possível passar para a linha seguinte de dados, além da opção de teclar “Próximo”.
<br>
Após o preenchimento dos dados na tela inicial e dado o aceite para os cálculos, eles são processados pelo programa. Os dados são apresentados graficamente e por três abas com indicadores.
O gráfico apresenta curvas em vermelho, uma curva em verde e pontos brancos, indicando, respectivamente, as catenárias formadas nos subvãos do cabo condutor, a catenária formada pelo cabo suporte e a posição dos espaçadores, conforme figura abaixo.


![0051-grafico](https://user-images.githubusercontent.com/42223882/210844976-223ad0d6-e85a-401a-a36b-96ddedaced3a.png)

Quanto as três orelhas das abas menores logo abaixo do gráfico, elas são acessadas através do posicionando do ponteiro sob a aba de interesse. Cada aba representa um conjunto de dados dos Espaçadores, Subvão (formado pelos espaçadores e cabos condutores) e Cabo Suporte.
<br>Os dados apresentados em cada aba citada são os seguintes:
<ul><li>Espaçadores:
<ul><li>	Número de espaçadores que compõe o vão analisado;
<li>	Vetor de dados referente a posição de cada espaçador no vão, em metros.
 </ul>
<li>	Subvão
<ul><li>	Extensão c/ 55% (m): comprimento dos vãos adjacentes aos suportes, equivalente a 55% do comprimento limite especificado pelo operador;
<li>	Flecha lim calc (m): flecha calculada da subcatenária; considerada a pior posição, no centro do vão, em metros;
<li>	Comp Calc (m): comprimento calculado do subvão médio, em metros;
<li>	Tração cond.(N): valor da tração horizontal média dos condutores que compõe os subvãos, em N.
</ul> 

<li>	Cabo Suporte
<ul><li>	Tração EDS (N): tração horizontal do cabo suporte, em N;
<li>	Tração Test (N): tração horizontal do cabo suporte à temperatura estendida, em N;
<li>	Flecha Test (N): flecha máxima da catenária formada pelo cabo suporte, em N.
</ul>
</ul>
Ao observar os valores e curvas apresentados, o operador tem duas opções: gravar, a partir do botão situado abaixo e no meio do gráfico (“Gravar”), ou clicando o botão “Próximo”.
<br>
Na opção “Gravar”, tecla de atalho F11, quando acionado este botão, aparece uma tela pedindo pelo nome do arquivo. Neste arquivo serão salvos todos os dados fornecidos pelo operador e calculado pelo programa.
<br>
Na opção “Próximo”, aparecem mais duas opções em relação a opção Novo Cálculo, “Sim e Não”. Se optar por “Sim”, o processo repete-se desde o início novamente, caso contrário o programa é finalizado, apresentando o último painel antes da interrupção.



</p>

<p align="center">

![0051-fluxo](https://user-images.githubusercontent.com/42223882/210844723-d25d9075-4577-4238-9c3c-07695192f246.png)

</p>

## Análise dos Resultados

A análise dos resultados pode ser feita através dos recursos apresentados na aba “Análise”, situada na parte superior esquerda do programa, que automaticamente é selecionada após o término do preenchimento da primeira tela. Ali podem ser encontrados um gráfico contendo duas curvas e os pontos de instalação dos espaçadores, outra três abas, contendo indicadores, que se encontram abaixo do gráfico, conforme descrito no item anterior.
<br> Quando se opta por gravar os dados, surge uma tela do Windows Explorer, no intuito de nomear o arquivo e destinar a pasta onde será salvo este arquivo. O conteúdo do arquivo é gravado com caracteres em ASCII e se apresenta da seguinte forma:
<ul><li>Dados do painel inicial introduzido pelo operador:
<ul><li>Condutor: Peso Unitário do condutor, Módulo de Young do cabo Condutor, Coeficiente de dilatação térmica linear do condutor, Seção transversal do condutor, Tração horizontal EDS condutor Tração horizontal do condutor nominal, Tração horizontal do condutor ampliada.
<li>	Suporte: Peso Unitário do cabo suporte, Módulo de Young do cabo Suporte, Coeficiente de dilatação termina linear do cabo suporte, Seção transversal do suporte, Tração horizontal suporte à temp. estendida.
<li>	Vão: Comprimento do vão, Desnível dos apoios, Flecha máxima na temperatura nominal de projeto.
<li>	Subvão: Comprimento do subvão calculado, Número de espaçadores calculado, Extensão do subvão calculada, Extensão do subvão calculada 55%, Comprimento do cabo do subvão.
</ul>
<li>Coordenadas x e y dos pontos da instalação dos espaçadores, em metros.
<li>Coordenadas x e y das curvas dos subvãos de condutores, em metros.
<li>Coordenadas x e y da curva do cabo suporte, em metros.
</ul>


## Special thanks

This is part of the RD&I project results obtained during the execution of PD-07130-0051/2020: "Support device and mechanical damping for conductor cables in transmission lines subject to operating overload”, executed by TAESA and LACTEC Institutes financed by the RDI Program of the Brazilian Electricity Sector Regulated by ANEEL (National Agency of Electric Energy).

![01](https://user-images.githubusercontent.com/42223882/210847845-3c9b80e0-5ed5-4a67-b4bc-9db25c0f2623.png)




## Licença 

The [MIT License]() (MIT)

Copyright :copyright: 2020 - Sistema Suporte e Espacador
