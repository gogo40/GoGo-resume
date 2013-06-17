Marcelo Aires Caetano
========================
:Email: marcelo@fiveti.com
:Localização: São Paulo/SP, Brasil
:Idade: 29

Experiência relevante
---------------------
*Para mais detalhes relativos a experiência entre em contato por e-mail*

Sobre
~~~~~

Sou um profissional com larga experiência em resolução de problemas complexos de alta tecnologia, dimensionamento de soluções, *realtime*, missão crítica, sistemas distribuídos, etc.

Apaixonado por tecnologia, sempre me sinto motivado em meio a desafios e na exploração de novas técnicas, procuro em todos os projetos nos quais trabalho, desenvolver arquiteturas de solução que a médio e longo prazo sejam de barata manutenção.

Conto com uma experiência de 14 anos em pesquisa e desenvolvimento de tecnologia.

.. . [1] Neste Currículo, pretendo demonstrar apenas as experiências que eu achar mais relevantes e apenas de no máximo 4 anos de carreira. para maiores informações, entre em contato por email e/ou acesse minha página no github (esta página tem apenas projetos públicos feitos por mim de 1 ano pra cá).

_______



Algumas experiências relevantes
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


Sistema embarcado em RasperberryPI
____________________________________________________

Baseado em RaspBMC, criei media center interativo com suporte a eventos de IO por usuários, reconhecimento de faces (OpenVC), com suporte a apis de twitter e rss para exibição de informações ao usuário,
bem como client de torrent (baseado no Transmission) com servidor privado para distribuição de mídia,

desenvolvimento de drivers usb com OpenUSB


.. _2502:

Biblioteca para monitoramento de arquivos em windows
____________________________________________________

Utilizando WaitForMultipleObjects e IO Completion Port (WFMO e IOCP) fiz projeto de monitoramento de arquivos em python, utilizando apenas ctypes e win32api pura para notificação de eventos em sistemas de arquivos no windows.



Biblioteca de eventos multiplataforma baseada em Glib
_____________________________________________________

Pygel é uma biblioteca que gerencia de maneira multiplataforma eventos de todas as fontes (sistemas de arquivos, sockets, keyboard, etc), e contem suporte a timers e threading nativos para cada uma de suas plataformas


2502
____
  *Framework para Computação distribuída em topologia de Estrela*

  Arquitetura, Planejamento e Desenvolvimento

  Desenvolvido em meu tempo livre, o 2502, consiste numa plataforma de computação distribuída que provê uma rede em topologia de estrela, escalado em multi-estrela e anel, na qual todos os computadores nela conectados, podem enviar RPCs, Chamadas Remotas de funções, consultar documentação de função remotas, chamadas de funções em broadcast e multicast, utiliza técnicas de sendfile para menor latência, funcionamento multiplataforma, inclusive em Android, suporte a escalamento de rede por meio de hubs e framework web wsgi compatível com suporte a templates, roteamento, etc.  que permite acessar a rede diretamente Framework através de uma webapp, se necessário.

  Ferramentas utilizadas: Python, pygel, openssl.


Client de rede que dá informações em tempo real sobre o mercado de capitais
___________________________________________________________________________

  Em parceiria com um amigo, foi feita engenharia reversa e sniffing em um *client* de uma rede que disponibilizava informações de mercado financeiro para windows por DDE. Foi desenvolvido apartir daí, um client em C++ multiplataforma.

  Ferramentas utilizadas: Python, Aida-PRO, wireshark

______


Arquiteto de Software Senior, Titans Group, *2012* - Atualmente
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Titans Sync
_______________________________________
 Primeiro sistema de cloud Files (como o dropbox) produzido no brasil

 Neste projeto sou responsável por arquitetura de client desktop multiplataforma em python (para núcleo) e c++ para backend/frontend, bem como, líder técnico.

 Entre as atividades, estão: engine python, para tratamento de regras de negócio, e alta concorrência para sincronização de repositórios.
 Client em C++ que embarca a engine Python C++,
 o Client C++ é responsável por backend com os sistemas operacionais, tal como comservers, acesso a internet, shadowcopy, file system monitoring, spooling, e front end (traybar, e plugins para nautilus, finder, windows explorer com suporte a menus de contexto para estado de arquivos e sincronização, bem como ícones anexados aos seus arquivos representado estado de sincronização de arquivos)

 No Client é usado recursos de Eventos (WFMO, IOCP, para windows, IOCP, KQUEUE para linux e bsd-osx), memory pool, threadpools, semáforos, barriers, e mutexes, protocolo de IPC para comunicação nativa com COMSERVERS apartir de namedpipe e unix domain socket em sistemas baseados em unix (linux, osx)

 na engine é usado recursos de barrier de fluxos, grafos ponderados,

 é embarcado todo o python (salvo python.dll) dentro do binário sendo seus módulos importados dinamicamente, inclusive outras dlls



Arquiteto de Soluções/Engenheiro de Software, Grupo Markplan , *2012*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Mídia em Tablets
_______________________________________

 Arquitetura, desenvolvimento

 O Projeto visa uma maneira eficiente de distribuir mídias para tablets android utilizando tecnologia de `transferência de arquivos`_ em junção ao 2502 previamente desenvolvidos por mim, porém portada para funcionar no android.

 Coordenei o desenvolvimento de um launcher java para lançar um webview e mediaview no tablet para acesso ao frontend previamente desenvolvido(html5) e backend(2502).

 Ferramentas utilizadas para o backend: 2502, SL4A, Python

.. _Player:

Player de Vídeo Baseado em libvlc
_________________________________
 Desenvolvimento de Player de vídeo em Qt, baseado na libvlc.

 O Player *standalone* suporta scripting em Javascript, configuração de interface gráfica por css, além de herdar todos os recursos avançados do vlc. No scripting foi dado suporte a controle multiplataforma à porta paralela (sem necessidade de root), além de funções de JSON e manuseamento de arquivos.

 Ferramentas utilizadas: C++, Qt, libvlc, MOC, qmake, QtScript

Desenvolvimento de Totem de Mídia Interativa
____________________________________________
 Utilizando o `Player`_ acima construído, foi criado um circuito eletrônico paraacender conjuntos de 18 leds em cada pino da porta paralela, para isto, foram utilizados Relês e Transistors BC475.
 O Objetivo do projeto, é prover uma Mídia interativa, que, quando um determinado personagem no vídeo apontasse para caixas de acrílico, estas acendecem.
 Para garantir sincronismo, foi especificado um arquivo um tanto similar com os arquivos .srt, porém em formato JSON, que lidos pelo scripting em Javascript, acendem, ou apagam, os leds no tempo determinado.

 Ferramentas utilizads: C++, Qt, `Player`_, lpdev, javascript

.. _Mídia em elevadores:
Plugin de Browser
__________________________________________
 Desenvolvimento de Plugin para Firefox e Internet Explorer e Desenvolvimento de Microbrowser

 O Plugin utiliza `player`_ e fornece à aplicação web suporte a player, captura de vídeo, legendas, e eventos suportados por javascript.

 O Plugin também Funciona em um Microbrowser por mim desenvolvido.

 Ferramentas utilizadas: C++, Qt, `player`_ , WebKit, MOC, qmake

Bafômetro
_________
 Arquitetura e desenvolvimento de Bafômetro de baixo custo.

 Utilizando uma placa de som, um sensor MQ-3, e alguns resistores, Desenvolvi um bafômetro com uma precisão razoável, reduzindo o custo de produção da solução anterior.

 Ferramentas utilizadas: C++ com STL, alsa, pthreads, winthreads e WSApi, na segunda implementação, foram usadas as bibliotecas portaudio e portmixer.

Totems de Celulares
___________________
 Arquitetura e desenvolvimento de circuito e software para monitoramento de carga de celulares.

 Consiste em um totem para carregadores de celulares. O circuito eletrônico, permite que através da porta paralela do computador, soubesse-se quando um celular estava sendo carregado e utilizando o equipamento. Os Dados são enviados de forma segura para webservice com a proteção de uma assinatura HMAC. possibilitando-se assim, monitorar-se em tempo real o uso dos totems.

 Ferramentas utilizadas: C++, libevent, lpdev.

BluFIT
______
   Arquitetura, gestão de equipe e desenvolvimento

   Este projeto visa fornecer, através de heurística (e futuramente por algoritmos genéticos), o treino ideal para o usuário de academias, ou pessoa que queira exercitar-se por conta própria.

   Ferramentas utilizadas: Python, Flask, SQLalchemy

Arquiteto de Software, Lightcomm Tecnologia e Serviços , *2010 - 2012*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
- Arquitetura de plataforma Web e Mobile
- Desenvolvimento de Solução

Arquiteto de Soluções/Engenheiro de Software, RogerSoftware, *2008 - 2011*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
SICOTAG
_______
   Desenvolvimento de Solução de Monitoramento de Transeuntes

   O Projeto através de sensores de infravermelho monitora a quantidade de visitantes em eventos.

Auto Atendimento TouchScreen
____________________________
  Utilizando apenas o Cairo e tecnicas de programação gráfica (*como Gaussian Emboss*), foram feitos diversos widgets, afim de dar ao usuário de auto atendimento, uma simples, porém agradável experiência.

  Ferramentas Utilizadas: Python, PIL, Cairo


SigaNET
_______
- Ambiente de software multiplataforma de computação distribuída.

  Desenvolvimento de Toda a solução.

  Drivers multiplataforma para impressoras térmicas, portas paralelas, mouses seriais e interfaces USB.

  Widgets com GDI+ para toolkit criado para suporte a win98, com comportamento bastante similar ao GTK+.

  DLLs em C para gerenciamento de processos com NTApi (WinApi), serviços para Windows e daemons para Linux.

  Extensões de Python em C, C++ e Cython para otimizar a plataforma.

  _`Transferência de Arquivos`

  Sistema de sincronização de arquivos inspirado na tecnologia rsync, com suporte a correção automática de corrupções de arquivos, canais de entrega, slots de transmissão, fila de espera e controle de banda.

  Servidores para streaming de IPTV.

  Ferramentas Utilizadas: Python, GTK+, C, C++,  Alsa, winsound, libspeex, libvlc, GStreamer, 2502, etc

===============

Idiomas
-------
- Português (*Idioma nativo*): compreende bem, fala bem, lê bem, escreve bem
- Inglês: compreende razoavelmente, fala razoavelmente, lê bem, escreve bem

Habilidades
-----------
Eletrônica
~~~~~~~~~~
- Desenvolvimento de circuitos eletrônicos

Desenvolvimento de Software
~~~~~~~~~~~~~~~~~~~~~~~~~~~
- Nível *expert* em desenvolvimento em Python
- Nível avançado em desenvolvimento em C e C++
- Nível avançado em Multiprogramação (threads, mutexes, semaphores, condition variable, sistemas de eventos, barriers)
- Nível *expert* em sistemas distribuídos
- Programação em: Python, C, C++, Javascript, PHP, Lua, etc.
- Ferramentas: Hg, Git, Fossil, Apache, QMake, CMake, Subversion, MySQL, SQLite3, etc.
- Metodologia: Ágil (Scrum, XP)
- Plataformas: FreeBSD, Linux (Debian, Ubuntu), OSX, Windows (98, 2000, XP, 7).
- Bibliotecas: STL, Qt, GTK, Glib, Cairo, WxWidgets, Readline, WinAPI, Zlib, etc.
- Solidos conhecimentos em TCP/IP, UDP, IP, IPv6, Sistemas de Rotas
- Experiência com Blutooth, PPP
- Conhecimentos avançados em Posix
- Conhecimentos em Linux Kernel

Maiores Influcências
~~~~~~~~~~~~~~~~~~~~
Andrew S. Tanenbaum, Djisktra, Donald Knuth, Leslie Lamport, D. Richard Hipp, Fabrice Bellard, Et. Al.
boa

Projetos, e Links
------------------------------
- `github`_ - Minha página pessoal do github contendo projetos que mantenho e que desenvolvo
- Este `Currículo`_: `Repositório`_ (atualizada em 16 de junho de 2013)

.. _`github`: https://github.com/caetanus
.. _`Currículo`: https://github.com/caetanus/resume/resume-pt_br.rst
.. _`Repositório`: https://github.com/caetanus/resume/
