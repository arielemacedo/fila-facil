# Fila Fácil - Aula 07

Protótipo didático de emissão e chamada de senhas em ordem FIFO. Entrega de Engenharia com IA: primeira entrega pública, TEC.1053, IFPI, turma 2026/2.

Responsável: Ariele Macêdo. Segundo integrante não informado. Implementação e verificações automatizadas com Codex (GPT-6), em 23/11/2026. Revisão humana e revisão cruzada ainda pendentes.

## Origem e licença

Lab 02 de [aislanifpi/tec1053](https://github.com/aislanifpi/tec1053), commit de origem `18efebd866d9a72423cd965ae381a23cf20b48dd`. Código e interface originais de Aislan Rafael, IFPI Campus Teresina Central, sob licença MIT, preservada em LICENSE.

A alteração funcional está restrita aos corpos de `emitirSenha`, `chamarProxima` e `reiniciarFila` em `src/fila.js`. Interface, especificação e suíte original foram preservadas.

## Execução

Abra `index.html` no navegador para usar a aplicação e `tests/index.html` para executar os 24 testes. Não há instalação de dependências.

Com Node já instalado, na raiz desta pasta:

```sh
node tests/executar.mjs
```

Opcionalmente, com Python já instalado:

```sh
python -m http.server 8007 --bind 127.0.0.1
```

Abra http://127.0.0.1:8007/ e http://127.0.0.1:8007/tests/index.html. Esses endereços são locais.

## Estado e evidências

Fluxo básico implementado e verificado localmente: **24 aprovados, 0 falhas, 24 testes**, tanto em Node quanto no navegador. Linha de base: 6 aprovados e 18 falhas.

Em `evidencias/` estão o escopo anterior à implementação, saídas dos quatro estágios e o roteiro de interface observado. Os resultados são do agente; não substituem a revisão por um colega nem uma explicação pessoal da aluna.

Repositório: https://github.com/arielemacedo/fila-facil

Aplicação: https://arielemacedo.github.io/fila-facil/

Testes públicos: https://arielemacedo.github.io/fila-facil/tests/index.html

Issue e evidências: https://github.com/arielemacedo/fila-facil/issues/1

Publicação configurada em main, pasta raiz. Conferência pública em andamento. Revisão humana e revisão cruzada continuam pendentes.

## Decisões

`push` adiciona ao fim da espera; `shift` retira o primeiro elemento. A chamada vazia retorna antes de qualquer mutação para preservar a última senha e o contador (RF-04). O reinício atualiza os quatro campos no mesmo objeto (RF-05). A confirmação pertence à interface fornecida.

## Limites

Uma fila por aba, estado apenas em memória. Recarregar apaga a sessão. Não há backend, persistência, sincronização, prioridade, múltiplos guichês ou dados reais. GitHub Pages disponibiliza os arquivos; não compartilha o estado entre dispositivos.

## Continuidade

Uma pessoa de outra dupla deve executar a suíte pública e o roteiro da interface e registrar sua revisão na issue, com nome, commit, URLs, horário e resultado observado. A issue permanece aberta para essa etapa. A atividade no Classroom permanece sem enviar.

