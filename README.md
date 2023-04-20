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
