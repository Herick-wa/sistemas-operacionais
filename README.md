# sistemas-operacionais
 questao (1)
 Pronto: o processo foi criado e está pronto para entrar na fila de execução.
- Pronto → Executando: o escalonador escolhe esse processo para usar a CPU.
- Executando → Bloqueado: o processo precisa esperar por algo (como leitura de arquivo).
- Bloqueado → Pronto: o evento esperado aconteceu (ex: terminou a leitura), então ele volta à fila.
- Executando → Pronto: o tempo de CPU acabou, e ele volta para a fila.
- Executando → Finalizado: o processo terminou sua tarefa.
- questao (2)
- Process Control Block (PCB) é como a “ficha técnica” de um processo no sistema operacional. Ele guarda todas as informações que o sistema precisa para controlar e gerenciar esse processo.
- questao(3)
- Quando um processo termina, o sistema operacional realiza uma limpeza completa para liberar todos os recursos que estavam sendo usados por ele
- questao(4)
- fork() é como fotocopiar um funcionário com todas as suas tarefas. Já exec() é como trocar o funcionário por outro com uma função completamente diferente, mas mantendo o mesmo crachá.
- questao(5)
- No UNIX, a hierarquia de processos funciona como uma árvore genealógica digital — cada processo pode gerar outros processos, criando uma estrutura de pai e filho.
- questao(6)
- - Memória compartilhada: rápida, mas exige controle de concorrência e é difícil de escalar.
- Troca de mensagens: mais segura e organizada, ideal para sistemas distribuídos, porém com mais overhead.

Cada uma tem seu uso ideal dependendo do contexto e da complexidade do sistema.
questao(7)
- Memória compartilhada: shmget(), shmat(), shmdt()
- Mensagens: msgget(), msgsnd(), msgrcv()
- Semáforos: semget(), semop()
- Sockets: socket(), send(), recv()
- Pipes: pipe(), read(), write()
- questao(8)
- No UNIX, a hierarquia de processos funciona como uma árvore genealógica digital — cada processo pode gerar outros processos, criando uma estrutura de pai e filho.
- questao (9)
- O gerenciamento de processos é uma das funções mais cruciais de um sistema operacional
- questao(10)
- processos independentes como pessoas lendo livros em silêncio numa biblioteca. Cada uma está focada no seu próprio conteúdo.  
Já processos cooperativos são como pessoas jogando futebol: precisam se comunicar, passar a bola, e trabalhar em equipe para alcançar o objetivo.

questao (11)
Um processo zumbi em sistemas UNIX/Linux é como um fantasma no sistema: ele já morreu, mas ainda aparece na tabela de processos

questao(12)
processo espera até que a operação termine.  
É como quando você liga para alguém e fica esperando ele atender. Você só continua depois que ele responde.

questao(13)
Um processo é um programa em execução. Ele tem seu próprio espaço de memória, arquivos abertos, variáveis e recursos. É como uma casa separada: cada processo vive em seu próprio ambiente.

questao(14)
É um sistema onde vários processos ficam na memória ao mesmo tempo, e o sistema operacional alterna entre eles para usar melhor a CPU. Isso permite que, enquanto um processo está esperando (por exemplo, por leitura de disco), outro possa usar o processador.

questao(15)
A comunicação via memória compartilhada é uma técnica bastante utilizada em sistemas operacionais e programação concorrente para permitir que múltiplos processos ou threads troquem informações de forma eficiente
