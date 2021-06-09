<img src="/Capa.png">

# Projeto Terezinha

<p><i> Metodologia da Pesquisa Científico-tecnológica - Banco de Dados - FATEC São José dos Campos </i></p>
<p>Aluna: Isabella Rosa Peixoto Segundo</p>

# Resumo
<p> A tecnologia atual, apesar de extensa e muito bem desenvolvida, pode ser um problema para pessoas que apresentam uma idade mais avançada, tanto por questões de dificuldade no aprendizado quanto por não estarem adaptadas a todas essas grandes novidades que surgiram e que continuam evoluindo cada vez mais. Conforme essa necessidade – ou mesmo curiosidade – em aprender e interagir com a tecnologia é cada vez mais comum no meio dos idosos, este projeto visa apresentar a proposta de um aplicativo que auxilie e ensine de forma didática e eficiente a utilização dos websites, aplicativos e configurações mais comuns. </p>

# 1 – Introdução
<p> No século passado, a maioria das pessoas nem imaginava a grande evolução tecnológica que temos hoje em dia. Coisas simples como ligações telefônicas até outras como chamadas de vídeo em tempo real eram impensáveis há não muitos anos atrás, mas, enfim, fazem hoje parte da realidade e do cotidiano quase que como necessidades imprescindíveis em muitos casos. A própria evolução dos celulares foi um grande salto, considerando que em 1993 foi enviada a primeira mensagem de texto do mundo (SMS), algo que inclusive demorou para chegar ao Brasil pois as operadoras ainda estavam começando a instalar os telefones fixos [Tecmundo]. O <i>TouchScreen</i> nos celulares foi também uma grande novidade, assim como a Internet, as redes sociais, os aplicativos, inteligência artificial, entre outras incontáveis tecnologias que são mais novas e ao mesmo tempo estão sempre evoluindo. </p>

<p> No entanto, conforme as tecnologias avançam, existe um grupo de pessoas no qual muitas apresentam dificuldades: os idosos. É notável que com o passar dos anos há maior dificuldade em aprender e reter novas informações, assim como para relembrar informações já conhecidas. Uma parte da comunidade médica acredita que com o passar dos anos as conexões cerebrais vão sendo prejudicadas. Já outra parte, conforme a publicação científica <i>Journal of Topics in Cognitive Science</i> entende que o cérebro funciona como um disco rígido: quanto mais dados tem, mais demora para encontrar as informações necessárias [BBC]. De qualquer forma, as tecnologias são um grande desafio para quem nunca nem imaginou tudo o que temos na atualidade. </p>

<p> Em uma amostra de 320 pessoas idosas, 103 pessoas afirmaram já ter utilizado o computador, dentre estes 75,7% afirmaram ter dificuldades [Baptista]. Essa grande dificuldade pode ser encontrada também na utilização de Smartphones. 5,2 milhões de pessoas acima dos 60 anos têm acesso à internet no País – 21% da população na terceira idade [Instituto Locomotiva]. </p>

<p> Segundo uma pesquisa feita pela terapeuta ocupacional e professora da Universidade Federal do Paraná (UFPR) Taiuani Marquine Raymundo, 24% dos idosos declararam ter medo de utilizar novas tecnologias e 40% confessaram receio em danificar o aparelho. De acordo com uma pesquisa do <i>Pew Research Center</i>, entidade norte-americana, 50% dos idosos que utilizam a Internet melhoram o contato familiar, social, comercial (por meio da leitura de notícias) e até educacionais – para além do aprendizado da tecnologia, os idosos também passam a realizar pesquisas, a ver filmes e a fazer cursos on-line [Tena]. </p>

<p> Com isso, alguns aplicativos foram criados para auxiliar os idosos: configurar interfaces, salvar lembretes médicos ou mesmo ensinar a adicionar, deletar ou editar contatos na agenda [Zoom]. Porém, não existe um aplicativo mais completo ou mais intuitivo – apesar de serem simples, alguns idosos podem ainda apresentar dificuldades. É por este motivo que a proposta desse trabalho é a criação de um aplicativo que ensine, por meio de tutoriais interativos e didáticos, acessados por comando de voz (como assistente virtual), a facilitar a relação dos idosos com a tecnologia. </p>

# 2 – Fundamentação Teórica
<p> Esta seção visa apresentar os conceitos e tecnologias a serem utilizados no desenvolvimento da aplicação. </p>

## 2.1 – Comando de Voz
<p> O reconhecimento de voz segue alguns passos básicos, partindo da transformação das ondas sonoras em dados. A amostra de voz é comparada a padrões em uma base de dados. Havendo um <i>"match"</i> entre a amostra recolhida e as registradas, o comando é "entendido" pelo aparelho e, em seguida, executado. Os algoritmos que atuam no reconhecimento de voz usam complexos modelos como o <i>Hidden Markov Model</i> (HMM) – aplicado em reconhecimento de padrões. Eles combinam informações acústicas e determinam quais frequências estão presentes em qual instante de tempo para calcular qual a palavra mais provável que a pessoa está falando [Tilt UOL]. </p>

## 2.2 – Tecnologia Mobile
<p> A tecnologia Mobile é aquela que vai aonde o usuário estiver: smartphones, tablets, relógios, entre outros [IBM]. </p>

## 2.3 – Heurísticas de Nielsen
<p> Organizar bem a UI (<i>User Interface</i>) está interligado a oferecer uma boa experiência para o usuário, que deixe as funcionalidades bem claras e que o sistema possa ser utilizado de forma simples e intuitiva – basicamente, sem necessitar de um “manual de instruções”. Para isso, Jakob Nielsen, cientista da computação, propôs dez heurísticas que auxiliam na criação de boas interfaces, melhorando a <i>User Experience</i> (UX), por conseguinte. </p>

## 2.4 – React Native
<p> Com o lema “aprenda uma vez, escreva em qualquer lugar”, o React Native combina as melhores partes do desenvolvimento nativo com React, uma biblioteca JavaScript para construção de interfaces. Pode ser utilizado tanto no Android quanto no iOS ou pode-se criar um aplicativo do zero. Atualmente é utilizado em aplicativos como Facebook, Instagram, Discord, Skype, Pinterest, Shopify, Uber Eats, Salesforce, Oculus, entre outros [ReactNative]. </p>

# 3 – Metodologia e Métodos
<p> Nesta seção serão apresentados os métodos utilizados e a metodologia aplicada para o desenvolvimento da aplicação. </p>

## 3.1 – Descrição do Funcionamento
<p> O usuário irá dizer “Terezinha” (nome do aplicativo/assistente) para ativá-lo por <b>comando de voz</b> e em seguida poderá dizer qual função deseja aprender a utilizar: configuração de algo no celular, ligações, como ver algum vídeo na internet, onde acessar para ler o jornal, como criar um e-mail, como acessar alguma rede social e seu funcionamento, como enviar mensagens, entre outros. Essas informações ficarão armazenadas no sistema por meio de <b>tutoriais</b> interativos que exibam o passo a passo de forma detalhada. Comandos de <b>ação direta</b> como “abrir internet”, “abrir agenda”, “fechar tal aplicativo” também serão reconhecidos para facilitar o acesso às aplicações. Não será necessário login para acessar, mas é importante possuir conectividade com a Internet. </p>

## 3.2 – Diagrama Explicativo
<img src="/Diagrama.png">

# 4 – Conclusão
<p> Conclui-se que, com o grande avanço da tecnologia, os idosos precisam de certa ajuda para se adaptarem – e o sistema proposto irá realizar estar função, auxiliando-os no cotidiano, ensinando desde o mais básico a funções específicas das aplicações mais utilizadas e agregando novos conhecimentos e integração ao mundo atual. A divulgação do aplicativo pode auxiliar até mesmo as famílias que porventura precisam se comunicar com os idosos, mas não conseguem ensiná-los de forma eficaz, e para que os idosos se sintam mais confiantes na utilização de algo que para eles é tão novo, mas ao mesmo tempo tão diferente e desafiador. </p>

# 5 – Referências
<p>JORDÃO, Fábio. História: a evolução do celular. Tecmundo, 2009. Disponível em: https://www.tecmundo.com.br/celular/2140-historia-a-evolucao-do-celular.htm </p>
<p> CÉREBRO DE IDOSOS é mais lento por excesso de informação, diz pesquisa. BBC News Brasil, 2014. Disponível em: https://www.bbc.com/portuguese/noticias/2014/01/140121_cerebro_lentidao_velhos_lgb </p>
<p>PRINCIPAIS OBSTÁCULOS da inclusão digital na terceira idade: uma revisão sistemática. Editora Realize, 2019. Disponível em: https://editorarealize.com.br/editora/anais/cieh/2019/TRABALHO_EV125_MD1_SA9_ID1712_27052019125015.pdf </p>
<p>BAPTISTA, Hélio Honorato Oliveira et al. A informática social: inclusão na terceira idade, 2014. Tese de Doutorado. </p>
<p>SCAFFUTO, Arthur. Tecnologia: os desafios encontrados na terceira idade. Jornal Daqui BH, 2017. Disponível em: https://www.daquibh.com.br/tecnologia-os-desafios-encontrados-na-terceira-idade/ </p>
<p>IDOSOS E A TECNOLOGIA: benefícios e dificuldades. Tena, 2016. Disponível em: https://www.tena.com.br/sobre-a-incontinencia/cuidadores/idosos-e-a-tecnologia-beneficios-e-dificuldades </p>
<p>BERGHER, Ricardo. Conheça 6 apps que facilitam o uso do smartphone para idosos. Zoom, 2020. Disponível em: https://www.zoom.com.br/celular/deumzoom/apps-smartphone-para-idosos </p>
<p>WHAT IS mobile technology?. IBM. Disponível em: https://www.ibm.com/topics/mobile-technology </p>
<p>LARA, Rodrigo. Fale e eu te escuto: como funciona o reconhecimento por voz. Tilt UOL, 2020. Disponível em: https://www.uol.com.br/tilt/noticias/redacao/2020/03/12/fale-e-eu-te-escuto-como-funciona-o-reconhecimento-por-voz.htm </p>
<p>MACEDO, Gabriel. 10 heurísticas de Nielsen para o design de interface. UX Collective, 2017. Disponível em: https://brasil.uxdesign.cc/10-heur%C3%ADsticas-de-nielsen-para-o-design-de-interface-58d782821840 </p>
<p>REACT NATIVE. Disponível em: https://reactnative.dev/
