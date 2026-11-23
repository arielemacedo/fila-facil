# Publicação e conferência pública - 23/11/2026

Estado: implementação, publicação e verificação automatizada concluídas; revisão humana e revisão cruzada pendentes. Conferência realizada pelo agente Codex (GPT-6), sem se apresentar como colega revisor.

Repositório: https://github.com/arielemacedo/fila-facil

Aplicação: https://arielemacedo.github.io/fila-facil/

Testes: https://arielemacedo.github.io/fila-facil/tests/index.html

Issue: https://github.com/arielemacedo/fila-facil/issues/1

Commit conferido: ff4c4647b822d73df3029071bba51ed8c3115979. Deploy: https://github.com/arielemacedo/fila-facil/actions/runs/45106254422, concluído com sucesso. Configuração: Deploy from a branch, main, /(root), endereço gratuito github.io.

Horário da conferência: aproximadamente 00h32 de 23/11/2026, America/Sao_Paulo. A aluna concluiu o login; o bloqueio anterior foi resolvido. O escopo local anterior à implementação foi publicado na issue após liberar o acesso; não se retrodatou sua criação.

## Resultados efetivamente observados no endereço público

- Sessão inicial: atual ausente, espera 0 e chamadas 0.
- Emissão de N001, N002 e N003 sem chamada automática.
- Chamada de N001, duas senhas em espera e total 1.
- Emissão de N004 no final da espera, mantendo atual e contador.
- Chamadas de N002, N003 e N004 em ordem, total 4.
- Chamada com fila vazia preservou N004 e total 4, com aviso de fila vazia.
- Cancelamento do reinício preservou estado. Confirmação limpou estado e comprovante.
- Tab localizou os botões, com contorno visível inspecionado; Enter em Retirar senha emitiu N001 após reinício.
- Outra aba iniciou vazia, mantendo a sessão original independente. Recarregar a original limpou a sessão.
- Suíte pública: 24 aprovados, 0 falhas, 24 testes.
- Cópia clonada do repositório público: 24 aprovados, 0 falhas, 24 testes em Node.
- Conteúdo de todos os arquivos de tests/ comparado ao original: idêntico, desconsiderada somente a normalização de finais de linha no transporte UTF-8.

## Decisão e continuidade

Mantido o contrato do laboratório: estado em memória por aba, sem backend, persistência ou sincronização. O Pages serve os arquivos e não compartilha a fila.

Revisão técnica automatizada realizada pelo agente. Revisão pessoal da aluna, identificação do segundo integrante e revisão por outra dupla não foram confirmadas. A issue permanece aberta para o colega registrar nome, commit, URL/horário, testes e comportamento observado. A explicação pessoal e a pergunta de saída devem ser discutidas pela aluna, sem atribuir a ela uma reflexão não fornecida.

Tempo observado: execução local e preparação em torno de 00h19 a 00h24; publicação e conferência em torno de 00h27 a 00h33, além das esperas de login. Não representa medição de produtividade humana ou prova de ganho causal com IA.

Documentação posterior a este commit acrescenta este registro e atualiza o estado no README, sem alterar a aplicação ou os testes. O ZIP original anexado antes da publicação foi substituído por uma versão com links e evidências atualizados, mantendo a atividade sem enviar.
