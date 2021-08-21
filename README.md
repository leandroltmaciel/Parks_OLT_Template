# Parks_OLT_Template
Templates para zabbix e Dashboard para grafana de monitoramento de OLTs Parks Fiberlink 20008s, 30028 e 40016

Template Parks Fiberlink OLTs 20008s/30028/40016

Template Zabbix - Versão 1.0 - Agosto/2021
Template Grafana - Versão 1.0 - Agosto/2021

Desenvolvido por Leandro Maciel - Consultor ISP - (69) 99257-6048

Dúvidas, elogios ou sugestões de melhorias podem ser enviadas através do 
email: leandro@257consultoria.com.br
ou pelo 
Whatsapp: (69) 99257-6048


ESTE TEMPLATE FOI DISPOLIBILIZADO GRATUITAMENTE E LEVOU HORAS DE PESQUISA, DESENVOLVIMENTO E TRABALHO.
SE ELE FOI ÚTIL PARA VOCÊ, CONSIDERE FAZER UMA DOAÇÃO, ELA ME INCENTIVA A CONTINUAR CRIANDO NOVAS VERSÕES.

PIX - 69992576048 (Celular) 



Requisitos:
	- Zabbix 5.X ou superior
	- Grafana 8.1 ou superior
	- Capacidade do servidor de aproximadamente 2.2 novos valores por segundo para cada OLT monitorada


Instruções para instalação - Zabbix:
	1. Faça a importação dos templates para o Zabbix na sequencia numerada na pasta
	2. Verifique se os seguintes templates apareceram na relação do seu zabbix
		- Template Module Generic SNMP Parks		
		- Template SNMP Interfaces Parks
		- Template Module Generic SNMPv2
		- Template Module Interfaces SNMPv2
		- Template Parks Fiberlink 20008S
		- Template Parks Fiberlink 30028
		- Template Parks Fiberlink 40016
	3. Verifique se os seguintes grupos de host foram devidamente criados
		- Parks OLT FL 20008
		- Parks OLT FL 30028
		- Parks OLT FL 40016
	4. Crie seus hosts e associe o template so devido modelo de OLT
		- Não marque a opção "Usar requisições em lotes" <<< MUITO IMPORTANTE! 
		- Coloque o host criado no respectivo grupo de modelo da OLT
		- Crie a macro "{$SNMP_COMMUNITY}" e atribua ao seu valor a community criada na sua OLT

Instruções para instalação - Grafana:
	1. Importe as dashboard para o grafana com os arquivos .json de acordo com o modelo escolhido

Notas: 
	- As regras de descobertas para as OLTs serie 20008s acontecem a cada 4 horas e coletas a cada 30 minutos
	- As regras de descobertas para as OLTs serie 30028 e 40016 acontecem a cada 2 horas e coletas a cada 15 minutos
	- As Dashboard foram otimizadas para exibição em resolução FullHD 1920x1080
	




