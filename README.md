# Restart Windows

Um script simples em Batch (.bat) para reiniciar o Windows através do Agendador de Tarefas.

## Como usar

1. Crie uma tarefa no **Agendador de Tarefas** do Windows apontando para o arquivo `restart.bat`.
2. Para agendar rapidamente via linha de comando (executando o CMD como Administrador) para rodar uma única vez às 3h da manhã:
   ```cmd
   schtasks /create /tn "Restart_Unico_3AM" /tr "C:\Caminho\Para\O\Arquivo\restart.bat" /sc once /st 03:00 /rl highest
   ```
