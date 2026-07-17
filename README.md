
# Sistema Automatizado para Demonstração Experimental da Queda Livre 

> Projeto vinculado ao SINAES – Soluções Inclusivas para Necessidades de Aprendizagem Específicas.

## Apresentação

O estudo do Movimento Retilíneo Uniformemente Variado (MRUV) e da Queda Livre na física mecânica frequentemente esbarra na barreira da abstração teórica, pois a velocidade com que os corpos caem impede medições manuais precisas, gerando erros gigantescos por causa do tempo de reação humana com cronômetros comuns. Essa limitação frustra os estudantes e os afasta da investigação científica real, forçando-os à memorização passiva de fórmulas. Como resposta a esse problema, propõe-se o desenvolvimento de uma Torre Vertical de Queda Livre Automatizada que combina um eletroímã, múltiplos sensores ópticos de barreira de luz ao longo do percurso com um sensor de fim de curso na base de impacto, conectados a um display LCD TFT posicionado ao lado da estrutura. Gerenciado por um microcontrolador ESP32, o sistema registra com precisão de microssegundos o instante em que o objeto rompe os feixes e o momento do choque final, processando esses dados instantaneamente para esboçar os gráficos de posição e velocidade em tempo real diretamente na tela. Essa solução é altamente relevante pois alia a engenharia à prática pedagógica inclusiva e ao Desenho Universal para a Aprendizagem (DUA), permitindo que estudantes com diferentes capacidades motoras participem de forma autônoma e visualizem o tempo físico invisível se transformar imediatamente em curvas e parábolas dinâmicas na bancada.

## Objetivo geral e objetivos específicos

### Objetivo geral

Capacitar estudantes a validarem as leis da gravidade autonomamente por meio de uma torre automatizada que transforma a queda livre em gráficos

### Objetivos específicos

Para alcançar esses objetivos, o projeto prevê o desenvolvimento do firmware no ESP32 focado na leitura das barreiras ópticas via interrupções de hardware e na renderização dos gráficos no display LCD TFT, em paralelo ao design e fabricação da estrutura física da torre por meio de impressão 3D e corte CNC para assegurar o alinhamento perfeito dos sensores e do fim de curso. O protótipo será validado inicialmente em bancada através da comparação entre a aceleração medida pelo sistema e o valor real da gravidade ($g \approx 9,8\text{ m/s}^2$) para fins de calibração. Por fim, sua avaliação prática e documentação definitiva ocorrerão durante a feira de inovação **IFTech**, onde a interação direta de estudantes e visitantes com o dispositivo servirá como teste real de usabilidade da interface gráfica, robustez do hardware e eficácia pedagógica da automação.

## Público-alvo e possibilidades de aplicação

- **Público-alvo:** alunos do ensino médio e superior.
- **Áreas ou componentes curriculares:** Física.
- **Conteúdos favorecidos:** física, Lei da Gravidade, MRUV, Leis de Newton e queda livre.
- **Possibilidades de aplicação:** Aulas, eventos e laboratórios.

## Resultados esperados

Espera-se desenvolver um protótipo funcional de uma Torre Vertical de Queda Livre Automatizada, construída com peças modulares em impressão 3D e corte CNC, integrada a um microcontrolador ESP32 com sensores de barreira de luz, um sensor de fim de curso na base, um eletroímã no topo para liberação controlada e sem impulso da esfera metálica, e um display LCD TFT acoplado. Esse dispositivo favorecerá a aprendizagem ao eliminar totalmente o erro humano de medição e de disparo manual, permitindo que os estudantes visualizem os gráficos e parábolas do MRUV sendo esboçados em tempo real na tela ao lado da estrutura, consolidando a transição do conceito abstrato da gravidade para dados empíricos visuais de forma multissensorial. Além disso, após sua validação e apresentação pública na IFTech, o projeto possui alto potencial de replicação e compartilhamento, pois todo o código-fonte, esquemáticos eletrônicos e arquivos de modelagem digital serão disponibilizados de forma open-source, funcionando como um kit didático de baixo custo que pode ser facilmente adaptado ou reproduzido por outros laboratórios de ensino e estudantes.

## Fundamentação e integração de conhecimentos

### Conhecimentos curriculares relacionados ao projeto

Velocidade, aceleração da gravidade, Movimento Retilíneo Uniformemente Variado (MRUV) e equações da Cinemática, temporização em microcontroladores, computação gráfica para renderização de curvas em displays TFT.

### Conhecimentos pedagógicos e metodológicos

- **O estudante poderá:** observar, testar, ouvir.
- **O material ajuda a compreender:** as funções horárias da posição e da velocidade no MRUV, o conceito de aceleração constante da gravidade e a tradução geométrica de uma aceleração em uma parábola gráfica.
- **A dificuldade que procura reduzir é:** a barreira de abstração e imprecisão gerada pelo tempo de reação humano ao usar cronômetros manuais, o erro experimental em medições dinâmicas de queda livre.
- **O conteúdo será apresentado por meio de:** objetos físicos tridimensionais, cores contrastantes no display LCD TFT, dados numéricos de tempo com precisão de microssegundos e o estímulo auditivo do impacto na base.
- **O estudante poderá demonstrar o que aprendeu por meio de:** testes práticos repetíveis na bancada, explicações baseadas nos coeficientes das parábolas geradas na tela e cálculos comparativos da aceleração local da gravidade.

### Conhecimentos técnicos mobilizados

- **Programação:** Desenvolvimento do firmware no ESP32 com interrupções de hardware para cronometragem em microssegundos e renderização dos gráficos de MRUV em tempo real no display TFT.
- **Eletrônica:** Circuitos de potência com transistor para acionamento do eletroímã.
- **Automação:** Desligando o eletroímã para soltar a esfera e encerrando a coleta de dados no instante do impacto mecânico na base.
- **Modelagem:** Empregada no design (CAD) de todas as partes do protótipo, como os suportes modulares das barreiras ópticas, o encaixe do eletroímã no topo e o gabinete do display TFT.
- **Impressão 3D:** Para realizar a manufatura das peças previamente modeladas (CAD), garantindo fixação, suportes de sensores sob medida e uma estrutura modular leve e alinhada.
- **Corte CNC:** Usinagem precisa da base de impacto e das réguas de sustentação vertical da torre em MDF


### Integração dos conhecimentos na solução

A transformação da barreira de abstração da gravidade em uma solução concreta ocorreu pela articulação direta entre a física, a pedagogia e a engenharia. Os **conhecimentos curriculares** de cinemática (MRUV) definiram os requisitos matemáticos que o sistema precisava processar, enquanto os **conhecimentos pedagógicos** baseados no DUA (Desenho Universal para a Aprendizagem) guiaram a criação de uma experiência multissensorial que elimina a frustração dos cronômetros manuais por meio de estímulos visuais e auditivos. Viabilizando essa proposta, os **conhecimentos técnicos** materializaram o hardware e o software: a **modelagem CAD** e o **corte CNC** estruturaram a torre, a **impressão 3D** fabricou os suportes modulares para os sensores ópticos da **eletrônica**, e a **programação** no ESP32 unificou tudo via **automação**, gerenciando o disparo do eletroímã, capturando o tempo em microssegundos até o impacto no fim de curso e plotando instantaneamente as parábolas no display TFT para que os estudantes comprovem as leis da física sem a interferência do erro humano.

### Diferentes formas de aprendizagem

- **Formas de representação:** A aceleração da gravidade deixa de ser uma teoria invisível e assume características multissensoriais. Visualmente, o display LCD TFT ao lado da torre esboça as curvas e parábolas do MRUV em tempo real utilizando cores contrastantes para diferenciar os gráficos de posição e velocidade, enquanto objetos físicos reais — a esfera metálica em queda livre e os sensores dispostos verticalmente — materializam o espaço percorrido; e auditivamente, o estalo mecânico do impacto da esfera contra o fim de curso na base fornece um feedback imediato do encerramento da contagem de tempo.
- **Formas de participação e interação:** O estudante atua como protagonista e investigador ativo do próprio aprendizado através do manuseio livre do dispositivo. Ele interage diretamente com o experimento ao posicionar a esfera no eletroímã do topo e iniciar o disparo automatizado via microcontrolador.
- **Formas de ação e expressão:** A validação do conhecimento ocorre de maneira flexível e prática, rompendo com os modelos de avaliações escritas tradicionais e equações decoradas. O aluno demonstra o que compreendeu ao operar com autonomia o sistema de controle, ao calibrar o protótipo comparando os dados da tela com a aceleração real da gravidade, ou ao explicar os fenômenos físicos e mecânicos observados por meio de apresentações orais e discussões baseadas nos coeficientes das funções plotadas diretamente no display TFT.

### Referências consultadas

HALLIDAY, David; RESNICK, Robert; WALKER, Jearl. Fundamentos de Física, Volume 1: Mecânica. 10. ed. Rio de Janeiro: LTC, 2016.

ESPRESSIF SYSTEMS. ESP32 Technical Reference Manual. Versão 4.6. Espressif Systems, 2023.

## Percurso metodológico do projeto SINAES

Os projetos vinculados ao SINAES adotam como referência o Processo de Desenvolvimento de Protótipos Acadêmicos, metodologia sistematizada pela proponente a partir da experiência acumulada na orientação e no acompanhamento de projetos acadêmicos voltados à criação de materiais didáticos e protótipos tecnológicos. A metodologia foi construída com base em práticas aplicadas, observadas e progressivamente aperfeiçoadas em projetos anteriores. Sua finalidade é oferecer aos estudantes um percurso acessível para organizar a identificação do problema, o planejamento técnico, a construção, os testes e a documentação das soluções. Embora dialogue com princípios do Processo de Desenvolvimento de Produtos apresentado por Rozenfeld et al. (2006), o percurso adotado pelo SINAES possui finalidade e organização próprias, adequadas ao contexto educacional e ao desenvolvimento de protótipos acadêmicos. 

O Processo de Desenvolvimento de Protótipos Acadêmicos está organizado em quatro etapas: 
1. **Geração do Conceito:** compreender o problema ou desafio de aprendizagem, identificar o público e definir a ideia inicial, a finalidade e as características gerais da solução.
2. **Planejamento e Especificação:** organizar o desenvolvimento do projeto, definir responsabilidades, identificar capacitações necessárias e selecionar materiais, tecnologias, ferramentas e recursos, considerando requisitos, cronograma e orçamento.
3. **Desenvolvimento Incremental:** construir a solução em partes, módulos ou versões sucessivas, realizando testes durante o processo e registrando dificuldades, decisões e modificações.
4. **Validação e Aperfeiçoamento:** verificar o funcionamento técnico e a contribuição da solução para a aprendizagem, analisar sua utilização por diferentes públicos, incorporar melhorias e organizar a documentação necessária ao compartilhamento e à replicação.

Essas etapas constituem uma orientação geral, e não uma sequência rígida. Conforme as características e necessidades de cada projeto, poderão ocorrer simultaneamente, ser retomadas ou receber procedimentos complementares. As adaptações realizadas deverão ser justificadas e registradas pelas equipes, com o acompanhamento dos professores responsáveis. 

A adoção desse percurso comum busca: 
- auxiliar os estudantes na organização do desenvolvimento;
- facilitar o acompanhamento dos projetos;
- registrar decisões, dificuldades e alterações;
- favorecer a integração entre conhecimentos curriculares e técnicos;
- orientar os testes e o aperfeiçoamento das soluções;
- padronizar a documentação sem eliminar a autonomia das equipes;
- facilitar o compartilhamento e a replicação dos resultados.

## Cronograma das etapas do desenvolvimento

| Etapa do PDP | Período planejado | Período realizado | Atividades desenvolvidas | Alterações, retornos ou sobreposições |
|---|---|---|---|---|
| Geração do conceito | novembro/2025 | novembro/2025 | Conversa com professor de física | definir a ideia inicial |
| Planejamento e especificação | maio/2026 | junho/2026 | desenvolvimento de esboços e reuniões com a equipe que está realizando o projeto | Mudança de sensores ultrassônicos para sensores ópticos |
| Desenvolvimento incremental | segundo semestre 2026 |  | montagem do protótipo |  |
| Validação e aperfeiçoamento | segundo semestre 2026 |  | aperfeiçoamento do protótipo |  |

## Capacitações, tecnologias, materiais e orçamento

| Capacitação | Finalidade no projeto | Período | Situação |
|---|---|---|---|
| Aulas ESP-IDF | Introduzir e ensinar os alunos a programar o ESP32 por meio do VS Code usando a ESP-IDF | abril,maio/2026 | Concluída |
| Aula soldagem eletrônica | Ensinar a base da soldagem em componentes eletrônicos e placas de prototipação | junho/2026 | Concluída |
| Aula Impressão 3D | Ensinar fatiamento e comandos básicos com impressora 3D | junho/2026 | Concluída |
| Aula CNC | Ensinar a comandar e operar CNC | agosto/2026 | Prevista |

### Tecnologias, ferramentas e equipamentos

| Tecnologia, ferramenta ou equipamento | Finalidade no projeto | Forma de acesso |
|---|---|---|
| Impressora 3D | Impressão de partes do projeto | Disponível no campus |
| Fusion360 | Modelar as peças para impressão 3D ou corte CNC | Disponível no campus |
| CNC | Corte da base em MDF | Disponível no campus |
| VS Code | Programar usando a ESP-IDF por meio dele | Disponível sem custo |

### Materiais e orçamento


| Material ou componente | Quantidade | Finalidade | Disponibilidade | Valor estimado |
|---|---:|---|---|---:|
| ESP32 | 1 | Calculo de tempo e dos valores desejados para fazer o gráfico | Adquirido na 1ª edição do projeto | |
| inserts de latão | 6 | possibilitar utilização de parafusos | Adquirido na 1ª edição do projeto |  |
| parafusos | 6 | prender a estrutura a base | Adquirido na 1ª edição do projeto |  |
| Eletroímã | 1 | segurar a esfera metálica e soltar no tempo preciso | Adquirido na 1ª edição do projeto |  |
| Sensores ópticos | 5 | fornecer dados sobre a queda | Adquirido na 1ª edição do projeto |  |
| Chapa de MDF | 3 | para a base e suportes verticais | Adquirido na 1ª edição do projeto |  |
| Filamento PLA | 300g | suportes para sensores, display e eletroímã | Adquirido na 1ª edição do projeto |  |
| **Total estimado** |  |  |  |  |

## Artefatos do projeto


| Artefato | Descrição | Formato ou localização | Situação |
|---|---|---|---|
| Apresentação do projeto | Experimento (torre) de queda livre e MRUV | [`apresentacao/`](apresentacao/) | Disponível |
| Código-fonte | Calculo de tempo e dos valores desejados para fazer o gráfico | [`codigos/`](codigos/) | Em elaboração |
| Modelo 3D | Modelos 3Ds das diversas partes da torre | [`modelos-3d/`](modelos-3d/) | Em elaboração |
| Imagens | Fotos da torre e dos gráficos | [`imagens/`](imagens/) | Previsto |
| Resultados | Exposição no IX IFTECH | [`resultados/`](resultados/) | Previsto |

> [!NOTE]
> **Possibilidades de replicação:** Ao término do projeto todos os materiais, modelos e códigos serão disponibilizados gratuitamente para replicação mediante a devida creditação, sem necessidade de licença ou autorização.

> **Créditos:** Informe a autoria dos arquivos, modelos, códigos, imagens e materiais externos utilizados.


## Produções e participação em eventos

- Inscrição na XIV IFTECH Campus Paranavaí, em outubro de 2026.
 
# Equipe

| Categoria | Nome | Curso, setor ou instituição | Participação no projeto |
|---|---|---|---|
| Estudante | Arthur Barbiratto Costa | Mecatrônica | Bolsista, estudante mentor do projeto |
| Estudante | Augusto Germano Ramos Meyer | Mecatrônica | Voluntário, estudante mentor do projeto |
| Estudante | Jheniffer de Brito Mariano | Mecatrônica | Desenvolvedor |
| Estudante | Rafael da Silva Santos  | Mecatrônica | Desenvolvedor |
| Estudante | Luzia Beatriz de Souza Pereira | Mecatrônica | Desenvolvedor |
| Estudante | Beatriz Aiko Hogaha | Mecatrônica | Desenvolvedor |
| Servidor | Eduardo Augusto Castelli Astrath | Docente E.B.T.T. – Núcleo da Base Nacional Comum/Física | Orientador/Demandante |
| Servidor | Daniela Eloise Flôr  | Docente E.B.T.T. – Informação e Comunicação/Informática | Coordenadora |



## Instituição

**Instituto Federal do Paraná – Campus Paranavaí**

**Projeto SINAES – Soluções Inclusivas para Necessidades de Aprendizagem Específicas**

---

*Este repositório está em desenvolvimento. Os conteúdos serão atualizados conforme o andamento das atividades.*
