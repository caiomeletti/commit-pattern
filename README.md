# Commit Pattern ou Padrões de confirmação 📜

Conhecidos como "Commits semânticos", a especificação do **[Conventional Commits](https://www.conventionalcommits.org/pt-br)** é uma convenção simples para utilizar nas mensagens de commit. Ela define um conjunto de regras para criar um histórico de commit explícito, o que facilita a criação de ferramentas automatizadas baseadas na especificação.

Esses *commits* auxiliarão você e sua equipe a entenderem de forma facilitada quais alterações foram realizadas no trecho de código que foi *commitado*.

Essa identificação ocorre por meio de uma palavra e emoji que identifica se aquele *commit* realizado se trata de uma alteração de código, atualização de pacotes, documentação, alteração de visual, teste, entre outras opções.

## Tipo e descrição 💬 

O *commit* semântico possui os elementos estruturais abaixo (tipos), que informam a intenção do seu commit no contexto do seu código.

<table>
  <thead>
    <tr>
      <th>Tipo</th>
      <th>Contexto</th>
      <th><i>Meu pitaco</i></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>feat</code></td>
      <td>Código está incluindo um <b>novo recurso</b>.</td>
      <td><i>a maioria vai aqui</i></td>
    </tr>
    <tr>
      <td><code>fix</code></td>
      <td>Código está <b>solucionando um problema</b> (bug fix).</td>
      <td><i>infelizmente sempre vai ter alguns aqui</i></td>
    </tr>
    <tr>
      <td><code>docs</code></td>
      <td><b>Mudanças na documentação</b>, como por exemplo no Readme do seu repositório. (Não inclui alterações em código).</td>
      <td></td>
    </tr>
    <tr>
      <td><code>test</code></td>
      <td><b>Alterações em testes</b>, seja criando, alterando ou excluindo testes unitários. (Não inclui alterações em código)</td>
      <td><i>Mas teste unitário não é código?</i></td>
    </tr>
    <tr>
      <td><code>build</code></td>
      <td>Modificações em <b>arquivos de build e dependências</b>.</td>
      <td></td>
    </tr>
    <tr>
      <td><code>perf</code></td>
      <td>Identificar quaisquer alterações de código que estejam relacionadas a <b>performance</b>.</td>
      <td><i>para os que tem que tirar leite de pedra</i></td>
    </tr>
    <tr>
      <td><code>style</code></td>
      <td>Alterações referentes a <b>formatações de código</b>, semicolons, trailing spaces, lint... (Não inclui alterações em código).</td>
      <td><i>portanto só serve para os que tem TOC</i></td>
    </tr>
    <tr>
      <td><code>refactor</code></td>
      <td>Mudanças devido a <b>refatorações que não alterem sua funcionalidade</b>, como por exemplo, uma alteração no formato como é processada determinada parte da tela, mas que manteve a mesma funcionalidade ou melhorias de performance devido a um code review (tem outro tipo para isso, mas nesse caso veio como uma tarefa secundária).</td>
      <td><i>grande fonte de problemas, já que a refatoração quase sempre arrasta algo que não deveria ter sido alterado</i></td>
    </tr>
    <tr>
      <td><code>chore</code></td>
      <td>Indicam <b>atualizações de tarefas</b> de build, configurações de administrador e pacotes; como por exemplo adicionar um pacote no gitignore. (Não inclui alterações em código)</td>
      <td></td>
    </tr>
    <tr>
      <td><code>ci</code></td>
      <td>Mudanças relacionadas a <b>integração contínua</b> <i>(continuous integration)</i>.</td>
      <td></td>
    </tr>
    <tr>
      <td><code>raw</code></td>
      <td>Arquivos de configurações, dados, parâmetros.</td>
      <td></td>
    </tr>
    <tr>
      <td><code>cleanup</code></td>
      <td>Utilizados para remover código comentado, trechos desnecessários ou qualquer outra forma de limpeza do código-fonte, visando aprimorar sua legibilidade e manutenção futura.</td>
      <td><i>há controvérsias</i></td>
    </tr>
    <tr>
      <td><code>remove</code></td>
      <td>Exclusão de arquivos, diretórios ou funcionalidades obsoletas ou não utilizadas, reduzindo o tamanho e a complexidade do projeto e mantendo-o mais organizado.</td>
      <td></td>
    </tr>
  </tbody>
</table>

## Recomendações ☑️

- Adicione um tipo consistente com o título do conteúdo;
- Seja sucinto, preferencialmente a primeira linha deve ter 4 palavras [*eu nunca consegui cumprir essa regra*];
- Para maiores detalhes, utilize a descrição do commit;
- Chame a atenção usando um emoji no início da mensagem de commit representando a ação do mesmo;
- Ao adicionar links, faça na sua forma mais autêntica, ou seja, sem encurtadores de link e links afiliados.

## Complementos de commits 💻

- **Título:** uma descrição sucinta da mudança (ou o título da tarefa que veio da ferramenta de gestão). Exemplo: *Isolando configuração do mapper*

- **Corpo:** descrições mais precisas do que está contido no *commit*, apresentando impactos e os motivos pelos quais foram empregadas as alterações no código, como também instruções essenciais para intervenções futuras. Exemplo: *Configuração do mapper foi isolada em método estático para que fosse reutilizado em testes unitários.*

- **Rodapé:** [opcional] informação sobre o revisor e número do card no Trello ou Jira. Exemplo: *Revisado por: Caio M Refs #9313*

<br>

> ♻️ REFACTOR: Isolando configuração do mapper<br>
> Configuração do mapper foi isolada em método estático para que fosse reutilizado em testes unitários.<br>
> Revisado por: Caio M<br>
> Refs #9313<br>

## Por que utilizar Commits semânticos? 🤷‍♀️🤷‍♂️

- Criação automatizada de CHANGELOGs.
- Comunicar a natureza das mudanças para colegas de equipe, o público e outras partes interessadas.
- Disparar processos de build e deploy (aqui depende de configurações adicionais).
- Facilitar a contribuição de outras pessoas em seus projetos, permitindo que eles explorem um histórico de *commits* melhor estruturado.

## Padrões de emojis 💈

<table>
  <thead>
    <tr>
      <th>Tipo do commit</th>
      <th>Emoji</th>
      <th>Palavra-chave</th>
    </tr>
  </thead>
 <tbody>
    <tr>
      <td>Acessibilidade</td>
      <td>♿ <code>:wheelchair:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Adicionando um teste</td>
      <td>✅ <code>:white_check_mark:</code></td>
      <td><code>test</code></td>
    </tr>
    <tr>
      <td>Atualizando a versão de um submódulo</td>
      <td>⬆️ <code>:arrow_up:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Retrocedendo a versão de um submódulo</td>
      <td>⬇️ <code>:arrow_down:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Adicionando uma dependência</td>
      <td>➕ <code>:heavy_plus_sign:</code></td>
      <td><code>build</code></td>
    </tr>
    <tr>
      <td>Alterações de revisão de código</td>
      <td>👌 <code>:ok_hand:</code></td>
      <td><code>style</code></td>
    </tr>
    <tr>
      <td>Animações e transições</td>
      <td>💫 <code>:dizzy:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Bugfix</td>
      <td>🐛 <code>:bug:</code></td>
      <td><code>fix</code></td>
    </tr>
    <tr>
      <td>Comentários</td>
      <td>💡 <code>:bulb:</code></td>
      <td><code>docs</code></td>
    </tr>
    <tr>
      <td>Commit inicial</td>
      <td>🎉 <code>:tada:</code></td>
      <td><code>init</code></td>
    </tr>
    <tr>
      <td>Configuração</td>
      <td>🔧 <code>:wrench:</code></td>
      <td><code>chore</code></td>
    </tr>
    <tr>
      <td>Deploy</td>
      <td>🚀 <code>:rocket:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Documentação</td>
      <td>📚 <code>:books:</code></td>
      <td><code>docs</code></td>
    </tr>
    <tr>
      <td>Em progresso</td>
      <td>🚧 <code>:construction:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Estilização de interface</td>
      <td>💄 <code>:lipstick:</code></td>
      <td><code>feat</code></td>
    </tr>
    <tr>
      <td>Infraestrutura</td>
      <td>🧱 <code>:bricks:</code></td>
      <td><code>ci</code></td>
    </tr>
    <tr>
      <td>Lista de ideias (tasks)</td>
      <td>🔜 <code> :soon: </code></td>
      <td></td>
    </tr>
    <tr>
      <td>Mover/Renomear</td>
      <td>🚚 <code>:truck:</code></td>
      <td><code>chore</code></td>
    </tr>
    <tr>
      <td>Novo recurso</td>
      <td>✨ <code>:sparkles:</code></td>
      <td><code>feat</code></td>
    </tr>
    <tr>
      <td>Package.json em JS</td>
      <td>📦 <code>:package:</code></td>
      <td><code>build</code></td>
    </tr>
    <tr>
      <td>Performance</td>
      <td>⚡ <code>:zap:</code></td>
      <td><code>perf</code></td>
    </tr>
    <tr>
        <td>Refatoração</td>
        <td>♻️ <code>:recycle:</code></td>
        <td><code>refactor</code></td>
    </tr>
    <tr>
      <td>Limpeza de Código</td>
      <td>🧹 <code>:broom:</code></td>
      <td><code>cleanup</code></td>
    </tr>
    <tr>
      <td>Removendo um arquivo</td>
      <td>🗑️ <code>:wastebasket:</code></td>
      <td><code>remove</code></td>
    </tr>
    <tr>
      <td>Removendo uma dependência</td>
      <td>➖ <code>:heavy_minus_sign:</code></td>
      <td><code>build</code></td>
    </tr>
    <tr>
      <td>Responsividade</td>
      <td>📱 <code>:iphone:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Revertendo mudanças</td>
      <td>💥 <code>:boom:</code></td>
      <td><code>fix</code></td>
    </tr>
    <tr>
      <td>Segurança</td>
      <td>🔒️ <code>:lock:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>SEO</td>
      <td>🔍️ <code>:mag:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Tag de versão</td>
      <td>🔖 <code>:bookmark:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Teste de aprovação</td>
      <td>✔️ <code>:heavy_check_mark:</code></td>
      <td><code>test</code></td>
    </tr>
    <tr>
      <td>Testes</td>
      <td>🧪 <code>:test_tube:</code></td>
      <td><code>test</code></td>
    </tr>
    <tr>
      <td>Texto</td>
      <td>📝 <code>:pencil:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Tipagem</td>
      <td>🏷️ <code>:label:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Tratamento de erros</td>
      <td>🥅 <code>:goal_net:</code></td>
      <td></td>
    </tr>
    <tr>
      <td>Dados</td>
      <td>🗃️ <code>:card_file_box:</code></td>
      <td><code>raw</code></td>
    </tr>
  </tbody>
</table>

## Exemplos 🎬

<table>
  <thead>
    <tr>
      <th>Comando Git</th>
      <th>Resultado no GitHub</th>
    </tr>
  </thead>
 <tbody>
    <tr>
      <td>
        <code>git commit -m ":tada: Commit inicial"</code>
      </td>
      <td>🎉 Commit inicial</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":books: docs: Atualização de README"</code>
      </td>
      <td>📚 docs: Atualização de README</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":bug: fix: Não aplicar permissão default"</code>
      </td>
      <td>🐛 fix: Não aplicar permissão default</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":sparkles: feat: POST/users"</code>
      </td>
      <td>✨ feat: POST/users</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":bricks: ci: Variáveis de ambiente no Dockerfile"</code>
      </td>
      <td>🧱 ci: Variáveis de ambiente no Dockerfile</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":recycle: refactor: Ajuste da role para permissão vazia"</code>
      </td>
      <td>♻️ refactor: Ajuste da role para permissão vazia</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":zap: perf: Otimização da geração do mapa de jornada"</code>
      </td>
      <td>⚡ perf: Otimização da geração do mapa de jornada</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":boom: fix: Revertendo mudanças ineficientes"</code>
      </td>
      <td>💥 fix: Revertendo mudanças ineficientes</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":lipstick: feat: Estilização CSS do formulário"</code>
      </td>
      <td>💄 feat: Estilização CSS do formulário</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":test_tube: test: Teste para validação de área"</code>
      </td>
      <td>🧪 test: Teste para validação de área</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":bulb: docs: Comentários no swagger"</code>
      </td>
      <td>💡 docs: Comentários no swagger</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":card_file_box: raw: Token do ambiente de homologação"</code>
      </td>
      <td>🗃️ raw: Token do ambiente de homologação</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":broom: cleanup: Eliminando variáveis não utilizadas"</code>
      </td>
      <td>🧹 cleanup: Eliminando variáveis não utilizadas</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":wastebasket: remove: Removendo arquivos desnecessários do projeto"</code>
      </td>
      <td>🗑️ remove: Removendo arquivos desnecessários do projeto</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":package: build: Package.json em JS"</code>
      </td>
      <td>📦 build: Package.json em JS</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":heavy_plus_sign: build: Adicionando dependência para DLL"</code>
      </td>
      <td>➕ build: Adicionando dependência para DLL</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":heavy_minus_sign: build: Atualizar caminho e nome do arquivo"</code>
      </td>
      <td>➖ build: Removendo dependência nuget</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":ok_hand: style: Revisão de código"</code>
      </td>
      <td>👌 style: Revisão de código</td>
    </tr>
	    <tr>
      <td>
        <code>git commit -m ":lipstick: feat: Atualização tema de interface"</code>
      </td>
      <td>💄 feat: Atualização tema de interface</td>
    </tr>
      <td>
        <code>git commit -m ":truck: chore: Atualizar caminho e nome do arquivo"</code>
      </td>
      <td>🚚 chore: Atualizar caminho e nome do arquivo</td>
    </tr>

  </tbody>
</table>
