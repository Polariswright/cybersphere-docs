<h1></h1>
<h1>CyberSphere Tecnologies</h1>
  <p></p>
  <ul><li></li></li>
  <b> </b>
<b>SOBRE A EMPRESA</b>
<p>A CyberSphere Technologies é uma empresa de TI voltada para a resolução de problemas e serviços de TI. A empresa foi criada e desenvolvida pela necessidade de gerenciamento e nossos principais serviços e produtos são:</p>
AutoTech (Automação Industrial), CustoCRM(CRM), ServerMax(Servidores),CloudBox(Cloud Computing), RouterPro(Roteadores.)  


Veja Gerenciamento para compreender melhor sobre nossos produtos e serviços.
<hr>

<b> COMO A INFRAESTRUTURA FOI CONSTRUÍDA
</b>
<li>Topologia Física</li>
<p>Foi planejada para a topologia física de rede da empresa no modelo estrela, onde os dispositivos da empresa estão conectados a uma única fonte de transmissão. Sendo cinco switches ao todo conectados ao servidor, um na sala de TI, um na sala de ADM, um na sala de RH, um na sala do financeiro e um na sala do servidor.

Além dos roteadores, onde temos um na sala do servidor que faz conexão com o que está  na recepção, que é para uso dos visitantes e sem fio. Mas que recebe a conexão direta do roteador na sala do servidor. 
 
1º Switch (SSVDR105) - Esse switch está na sala do servidor e faz conexão com o switch da sala de TI. Este por sua vez, conecta os outros três switches dos outros três departamentos restantes: RH, ADM e Financeiro. O switch da sala também é o responsável por conectar todos os oito computadores da própria sala.

2º Switch (SSTI104) - O switch da sala está recebendo a conexão do switch da sala do servidor e está distribuindo para os oito computadores da própria sala.

3º Switch (SSADM103) - Esse switch está recebendo a conexão do switch da sala 104 que está diretamente ligado ao servidor e está distribuindo para os oito computadores da própria sala.

4º Switch (SSRH102) - Esse switch está recebendo a conexão do switch da sala 104 que está diretamente ligado ao servidor e está distribuindo para os oito computadores da própria sala.

5º Switch (SSFNC101) - Esse switch está recebendo a conexão do switch da sala 104 que está diretamente ligado ao servidor e está distribuindo para os oito computadores da própria sala.

1º Roteador (RSVDR105) - Esse roteador está recebendo conexão do servidor e está repassando para o roteador sem fio da recepção.

2º Roteador (RRCP) - Esse roteador está recebendo a conexão do servidor e distribuindo via wireless.


</p>
<li>Topologia Lógica:</li>

<p>Foram analisados, tipos de topologias que melhor se encaixaria na empresa, foi escolhida a topologia estrela que melhor se adequaria com os planejamentos da empresa,
e com isso, foram organizados os computadores conforme as áreas de TI, Administração, RH e Financeiro. Além disso, foi colocado um roteador na área de lazer também para o público.
no esquema Lógico, foram criados além das máquinas, um servidor DHCP,  com a possibilidade de hosts totais de 246, com ip inicial de 10.142.68.10  e máscara de sub-redes de classe C (255.255.255.0), o servidor DHCP foi configurado dessa maneira, assim,
passando o endereço ip pelos switches dos diferentes setores.</p>
<li>As VMs:</li>
<p>Foram criadas três máquinas virtuais que consistem em dois clientes e um servidor, sendo que o servidor é um servidor DHCP. Os clientes usam o sistema operacional Debian, que foi instalado usando uma interface gráfica e configurado para usar a rede interna, recebendo um endereço IP do servidor DHCP. Por sua vez, o servidor foi instalado com o sistema operacional Debian em modo texto, permitindo melhor gerenciamento dos serviços distribuídos para os clientes da empresa (DHCP). O servidor possui duas placas de rede, sendo que uma foi configurada para a saída para a Internet (enp0s3) e a outra (enp0s8) foi configurada com um endereço IP estático para distribuir IPs aos clientes da empresa. As três máquinas virtuais se comunicam entre si e têm acesso remoto habilitado, com a instalação padrão do SSH em ambas as VMs.
</p>
</ul>
<hr>
<b> 
PERFIL DOS USUÁRIOS DA REDE(LAN)

</b>
<li>Tecnologia da Informação:
</li>
Comportamento: 
Os funcionários de TI tendem a utilizar mais recursos de manutenção e possuem cuidados extras com as máquinas do escritório por serem os mesmos a resolver os problemas, e utilizam a rede priorizando a segurança de si mesmos e dos outros funcionários da  empresa. 

Necessidades: 
Os profissionais especializados na manutenção da rede possuem a necessidade de acesso a todas funcionalidades disponíveis na LAN, para caso seja necessário alterações de segurança e backup das informações da rede;
Treinamento das políticas de segurança da empresa.

Permissões:
Acesso não restritivo a rede;
Acesso a senhas, logins, e-mails corporativos dos funcionários da empresa;
Acesso aos servidores;

<li>Administração:</li>
Comportamento: 
Diferente dos setor de informática, o setor administrativo tendem a usar a rede corporativa para utilizar as ferramentas administrativas da empresa, como por exemplo o Microsoft Excel para a criação de planilhas e acesso aos nossos softwares de organização, como o CustoCRM

Necessidades:
Treinamento das políticas de segurança da empresa;
Suporte técnico para a infraestrutura e rede,


Permissões:
Acesso somente a rede administrativa;
Acesso ao servidor de arquivo,web e e-mail; 
Acesso aos recursos do pacote Office;
Acesso às contas a pagar e receber, incluindo processar pagamentos e faturas.
Acesso ao Microsoft Teams;

<li>Recursos Humanos: 
</li>
Comportamento: 
O funcionário de RH possui acesso às informações cadastrais dos funcionários da empresa, portanto ele protege e utiliza as informações contidas nos servidores caso necessário, e sempre segue as políticas de segurança da rede em relação aos dados, evitando acessar a rede para questões pessoais e não autorizadas dentro das instalações  da empresa.

Necessidades:
Suporte Técnico para a rede e a infraestrutura;
Treinamento das políticas de segurança da rede da empresa;
Suporte para instalação e configuração de softwares específicos de RH para gerenciar processos de recrutamento, seleção e desempenho de funcionários.


Permissões:
Acesso às informações dos funcionários da empresa;
Gerenciamento dos e-mails e comunicações internas de funcionários e gerentes;
Acesso ao Pacote Office para gerenciamento de desempenho dos funcionários;
Acesso a internet com limitações;
Acesso ao servidor de arquivos, e-mails e web da empresa.

<li>Financeiro:</li>
Comportamento: 
O funcionário de RH possui acesso às informações cadastrais dos funcionários da empresa, portanto ele protege e utiliza as informações contidas nos servidores caso necessário, e sempre segue as políticas de segurança da rede em relação aos dados, evitando acessar a rede para questões pessoais e não autorizadas dentro das instalações  da empresa.

Necessidades:
Suporte Técnico para a rede e a infraestrutura;
Treinamento das políticas de segurança da rede da empresa;
Suporte para instalação e configuração de softwares específicos de RH para gerenciar processos de recrutamento, seleção e desempenho de funcionários.
Permissões:
Acesso às informações dos funcionários da empresa;
Gerenciamento dos e-mails e comunicações internas de funcionários e gerentes;
	Acesso ao Pacote Office para gerenciamento de desempenho dos funcionários;
Acesso a internet com limitações;
Acesso ao servidor de arquivos, e-mails e web da empresa.

<hr>
<b>CRESCIMENTO PROJETADO DA REDE</b>
<p>Equipamentos:


Cabos par trançado:
quantidade:27

Cabos par trançado cruzado:
quantidade:2
cabo de fibra ótica:
quantidade:1

Switches:
quantidade:5

Roteadores:
quantidade:2

Cloud:
quantidade:1

HOSTs: 
quantidade: 25

Servidores:
quantidade: 2


Instalações:
Dentro da empresa, já possuímos uma sala específica pensada para a expansão da rede e da quantidade nova de usuários que vem com ela. Nessa nova parte da instalação do nosso prédio principal será destinada a aumentar e incluir mais um novo servidor nas nossas instalações
</p>
<hr>

<b>POLÍTICA DE SEGURANÇA - FUNCIONÁRIOS</b>
<p>
Como a empresa Cyber Sphere, entendemos a importância de proteger as informações confidenciais da empresa e de nossos clientes. Por isso, desenvolvemos uma política de segurança da informação para garantir que todos os nossos funcionários estejam cientes das medidas de segurança que devem ser seguidas.

A seguir, apresentamos nossa política de segurança da informação:

Acesso à informação: todos os funcionários devem ter acesso apenas às informações necessárias para realizar suas funções. É proibido acessar informações confidenciais sem autorização prévia.

Senhas fortes: todas as senhas devem ter pelo menos oito caracteres e incluir letras maiúsculas, minúsculas, números e caracteres especiais. As senhas devem ser alteradas a cada três meses.

Dispositivos móveis: todos os dispositivos móveis devem ter senha de acesso e criptografia de dados. É proibido armazenar informações confidenciais em dispositivos móveis, a menos que seja absolutamente necessário.

Backup de dados: todos os dados críticos da empresa devem ser regularmente salvos em locais seguros e devem ser realizados testes regulares de restauração de dados.

Segurança física: todos os funcionários devem seguir as políticas de segurança física da empresa, como o uso de cartões de acesso e a proibição de entrada de pessoas não autorizadas em áreas restritas.

Treinamentos de segurança: todos os funcionários devem passar por treinamentos regulares de segurança da informação para garantir que estejam cientes das políticas de segurança da empresa e saibam como proteger as informações confidenciais.

Incidentes de segurança: todos os incidentes de segurança devem ser relatados imediatamente ao responsável pela segurança da informação da empresa.

A política de segurança da informação da Cyber Sphere é uma parte fundamental de nossos processos de negócios. Todos os funcionários devem seguir essas políticas rigorosamente e quaisquer violações serão tratadas com seriedade e de acordo com as políticas de disciplina da empresa.




</p>

<b>POLÍTICA DE SEGURANÇA - VISITANTES</b>
<p>A seguir, apresentamos nossa política de segurança da informação para visitantes:

Acesso restrito: os visitantes devem ser acompanhados por um funcionário autorizado durante sua visita à empresa. O acesso a áreas restritas é proibido, a menos que seja estritamente necessário e autorizado previamente.

Identificação: todos os visitantes devem fornecer uma forma de identificação, como um documento com foto, para serem registrados na empresa. O visitante deve estar ciente de que suas informações de identificação serão mantidas em segurança e de acordo com as leis de proteção de dados.

Senhas Wi-Fi: os visitantes podem ser autorizados a usar a rede Wi-Fi da empresa com uma senha específica fornecida pelo funcionário autorizado. Eles devem ser informados de que a rede Wi-Fi da empresa é protegida e que não devem acessar sites suspeitos ou baixar arquivos suspeitos.

Informações confidenciais: os visitantes não devem ter acesso a informações confidenciais da empresa ou de nossos clientes, a menos que seja absolutamente necessário e autorizado previamente.

Segurança física: os visitantes devem seguir as políticas de segurança física da empresa, como o uso de crachás de identificação, o acompanhamento de um funcionário autorizado e a proibição de entrada em áreas restritas.

Incidentes de segurança: se um visitante notar qualquer atividade suspeita ou incidente de segurança durante sua visita, ele deve relatar imediatamente ao funcionário responsável pela segurança da informação da empresa.

A política de segurança da informação da Cyber Sphere é uma parte fundamental de nossos processos de negócios, e esperamos que nossos visitantes a sigam rigorosamente. Qualquer violação será tratada com seriedade e de acordo com as políticas de disciplina da empresa.
</p>
<hr>
<b> GERENCIAMENTO
</b>

<p>
Esta parte da documentação apresenta os sete métodos de gerenciamento utilizados para melhorar a gestão de TI da empresa. Os métodos incluem Gerenciamento do Catálogo de Serviço, Gerenciamento de Nível de Serviço, Gerenciamento da Capacidade, Gerenciamento da Disponibilidade, Gerenciamento da Continuidade do Serviço de TI, Gerenciamento da Segurança da Informação e Gerenciamento de Fornecedor. O objetivo desta documentação é fornecer informações detalhadas sobre cada um desses métodos e como eles foram implementados para melhorar a eficiência e eficácia dos serviços de TI da empresa.

Gerenciamento do Catálogo de Serviço - Como equipe, implementamos um processo da ITIL (Information Technology Infrastructure Library) para manter um registro centralizado e atualizado de todos os serviços de TI oferecidos por nossa organização. Isso envolve:

Registro de serviços: mantemos um registro centralizado de todos os serviços de TI oferecidos, incluindo informações sobre preços, acordos de nível de serviço (SLAs) e relacionamentos com outros serviços.

Atualização constante: mantemos o registro atualizado com informações precisas e relevantes sobre cada serviço de TI oferecido.

Comunicação clara: comunicamos regularmente as informações do registro de serviços para as partes interessadas relevantes, como os usuários de TI e as equipes de gerenciamento de serviços.

Aperfeiçoamento contínuo: revisamos regularmente o registro de serviços e os SLAs para identificar áreas que possam ser aprimoradas e implementar mudanças necessárias para melhorar a eficiência e eficácia de nossos serviços de TI.

Gerenciamento de Nível de Serviço - Como equipe, adotamos a prática de gestão de serviços para garantir que nossos serviços atendam aos requisitos e expectativas dos clientes, de acordo com os SLAs. Algumas das formas como fazemos isso incluem:

Identificar e definir os SLAs: trabalhamos com nossos clientes para identificar seus requisitos e expectativas, e definimos acordos de nível de serviço claros e mensuráveis.

Monitorar o desempenho: monitoramos continuamente o desempenho de nossos serviços em relação aos SLAs e identificamos quaisquer desvios.

Implementar ações corretivas: implementamos ações corretivas imediatas para abordar quaisquer desvios e garantir que nossos serviços atendam aos SLAs.

Melhorar continuamente: buscamos constantemente oportunidades de melhoria em nossos serviços para atender às necessidades e expectativas em constante mudança de nossos clientes.

Gerenciamento de Capacidade - Como equipe, praticamos o gerenciamento da capacidade para garantir que os recursos da organização (servidores, redes, armazenamento, etc.) sejam dimensionados e gerenciados adequadamente para atender às necessidades do negócio.


Gerenciamento de Disponibilidade -  Como equipe, consideramos o Gerenciamento da Disponibilidade como um dos processos-chave da estratégia de serviço. É nossa responsabilidade garantir que os serviços de TI atendam às necessidades e expectativas dos usuários e clientes em relação à disponibilidade.

Gerenciamento de Continuidade do Serviço de TI - Nós somos responsáveis por garantir que nossa organização de TI possa continuar a fornecer serviços de TI essenciais, mesmo em caso de interrupções ou desastres.

Por exemplo, podemos criar backups regularmente e armazená-los em locais seguros para garantir a disponibilidade dos dados em caso de falhas no sistema. Além disso, podemos implementar planos de contingência para lidar com eventos imprevistos, como um desastre natural ou uma falha de energia, e garantir que nossos serviços continuem a funcionar sem interrupção para nossos usuários.

Gerenciamento da Segurança da Informação - Nós garantimos a confidencialidade, integridade e disponibilidade das informações da nossa organização. Para isso, implementamos medidas de segurança da informação que nos permitem gerenciar de forma adequada os riscos relacionados a ela. Assim, asseguramos que nossos dados e informações estejam protegidos contra acessos não autorizados, perdas, alterações ou indisponibilidades que possam comprometer o funcionamento da empresa. A segurança da informação é uma responsabilidade de todos nós e trabalhamos constantemente para mantê-la atualizada e eficiente.

Gerenciamento de Fornecedor - Nosso foco é a gestão do relacionamento com fornecedores externos para garantir:

Fornecimento de serviços e produtos necessários para suportar nossos serviços de TI;

Manutenção da qualidade e eficiência de nossos sistemas e processos;

Estabelecimento de parceria de confiança com fornecedores para trabalharmos juntos na resolução de problemas e na identificação de oportunidades de melhoria contínua;

Continuidade de nossos serviços e satisfação dos clientes internos e externos.




Gerenciamento de Melhoria Continuada - Podemos utilizar o Ciclo PDCA para gerenciar a melhoria contínua e garantir que nossos produtos e serviços atendam às necessidades dos clientes. Para isso, identificamos as áreas que precisam ser melhoradas, estabelecemos metas claras, implementamos mudanças e avaliamos os resultados para agir e melhorar constantemente nossos processos internos.

Gerenciamento de Incidentes - Como equipe, é importante que tenhamos prazos claros para cada etapa do processo de gerenciamento de incidentes de TI. Aqui estão alguns exemplos de prazos que podemos utilizar:

Identificação do incidente: o incidente deve ser registrado dentro de 15 minutos após sua ocorrência.

Classificação e priorização do incidente: devem ser feitas dentro de 30 minutos após sua identificação.

Investigação e diagnóstico do incidente: devem ser realizados dentro de 1 hora após sua classificação e priorização.

Resolução do incidente: deve ser feita dentro de um prazo definido, de acordo com a gravidade e complexidade do incidente.

Encerramento do incidente: deve ser feito dentro de um prazo definido após a resolução do incidente.

Análise pós-incidente: deve ser realizada dentro de 24 horas após a resolução do incidente.

Cumprir esses prazos é essencial para garantir que os incidentes sejam resolvidos rapidamente e que os usuários sejam afetados o mínimo possível.
<hr>
	
<b>CÁTALOGO DE INCIDENTES</b>
	<p>Produção em Baixa Escala e Qualidade

Em uma linha de produção manual, é possível que haja variações no processo produtivo devido à interferência humana, o que pode levar a erros, retrabalhos e desperdício de materiais.

Solução

Ao implementar a Automação Industrial, a empresa pode utilizar sistemas robóticos e computadorizados para executar tarefas repetitivas e precisas com maior eficiência, reduzindo o tempo de produção e aumentando a qualidade do produto final. Além também de proporcionar uma maior flexibilidade e escalabilidade para a empresa, permitindo que ela se adapte às mudanças na demanda do mercado de forma mais rápida e eficiente.

Falta de Visibilidade e Coordenação

Muitas empresas enfrentam dificuldades para manter um registro completo e atualizado das interações com seus clientes, o que pode levar a uma falta de compreensão sobre as necessidades e preferências dos clientes, bem como uma falta de comunicação e colaboração entre diferentes departamentos da empresa.

Solução

Ao implementar um sistema de CRM, a empresa pode centralizar e gerenciar de forma mais eficiente todas as informações sobre seus clientes, como histórico de compras, interações anteriores, preferências e necessidades. Isso permite que a empresa personalize a experiência do cliente, oferecendo sugestões de produtos ou serviços que possam ser relevantes para ele e resolvendo problemas de forma mais rápida e eficiente.

Instabilidade e Falta de Segurança 

Muitas empresas dependem de servidores para executar aplicativos e armazenar dados críticos. No entanto, sem uma infraestrutura adequada em administração de servidores, esses servidores podem ficar vulneráveis a falhas de segurança, perda de dados e quedas inesperadas, o que pode prejudicar a produtividade da empresa e gerar custos elevados para sua recuperação.







Solução

Ao implementar uma infraestrutura de administração de servidores, a empresa pode ter maior controle sobre seus sistemas de TI, garantindo sua disponibilidade, estabilidade e segurança. Por meio de uma monitoração constante, a equipe responsável pode identificar e solucionar problemas antes que eles causem maiores danos, além de prevenir falhas de segurança e garantir a integridade dos dados.




Limitação de Espaço de Armazenamento

Com a crescente quantidade de informações produzidas pelas empresas, pode ser difícil manter todos os dados e arquivos importantes armazenados localmente em discos rígidos ou servidores próprios, o que pode levar a uma falta de espaço de armazenamento e dificuldade de acesso aos arquivos quando necessário.

Solução

Ao implementar uma solução de armazenamento na nuvem, a empresa pode liberar espaço em seus dispositivos locais e armazenar dados e arquivos em servidores remotos. Isso permite o acesso aos arquivos de qualquer lugar, a qualquer momento, e em qualquer dispositivo, desde que haja acesso à internet.


Falta de Conexão e Rede de Baixa Qualidade

Em muitas empresas, a conexão com a internet é crucial para o desempenho das operações e das equipes de trabalho. No entanto, a falta de uma rede confiável e de qualidade pode prejudicar a produtividade da empresa, tornando difícil a realização de tarefas e a comunicação entre funcionários.


Solução

Ao instalar roteadores em pontos estratégicos da empresa, é possível criar uma rede de internet sem fio (Wi-Fi) estável e confiável para os funcionários, permitindo que eles trabalhem de forma mais eficiente e se comuniquem de maneira mais eficaz.

Segurança da Rede

Com o aumento do número de dispositivos conectados à rede, é fundamental garantir a segurança da rede da empresa contra ameaças externas, como hackers, malware e vírus.




Solução

Ao configurar adequadamente os roteadores da empresa, é possível implementar medidas de segurança avançadas, como firewalls, criptografia de dados, controle de acesso e monitoramento de tráfego de rede. Isso ajudará a proteger a rede da empresa contra ataques externos e garantir que as informações confidenciais da empresa permaneçam seguras.




















</p>














</p>
