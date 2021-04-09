Tutorial basicão para contribuir na construção do jardim digital.

1. Instale o git (https://git-scm.com/)
2. Envie uma mensagem no grupo do Telegram marcando o @GabGabroel pedindo para ser colaborador. Não esqueça de inserir seu email, username ou nome completo na mensagem. ![Pasted image 20210318220622.png](Pasted%20image%2020210318220622.png)
3. Crie uma nova pasta em seu computador (essa pasta vai ser o local no qual você vai editar o conteúdo do site, então escolha com sabedoria)
4. Abra o terminal dentro dessa pasta usando o botão direito do mouse e em "Git bash here" ou use seu terminal de preferência e navegue até a pasta.
5. No terminal, use "git clone https://github.com/SubZeroX/Zettel.git" ![Pasted image 20210318221805.png](Pasted%20image%2020210318221805.png)
6. Agora, só rodar um "git init"
7. Agora, rode "git remote add origin https://github.com/SubZeroX/Zettel.git"
8. Agora, para se certificar que estamos na branch correta, rode "git branch" ![Pasted image 20210318223321.png](Pasted%20image%2020210318223321.png)
9. Rode "git push -u origin dev"
10. Certifique-se que você está na branch "dev", na dúvida rode "git checkout dev"
11. Agora, rode "git pull" para testar se tudo está funcionando.
12. Agora, editaremos o .gitignore, use um editor de texto de preferência e adicione o seguinte texto:   
node_modules/   
.cache/   
.obsidian/   
public/   
gatsby-config    
package   
package-lock   
yarn   
13. Rodaremos agora "git add ."
14. "git commit -m 'Meu primeiro commit'"
15. "git push -u origin dev"
16. Agora, tudo que precisamos fazer é abrir essa pasta que criamos como uma vault no Obsidian ![Pasted image 20210318225724.png](Pasted%20image%2020210318225724.png) 
17. Defina a pasta "static" como atchament folder ![Pasted image 20210318225858.png](Pasted%20image%2020210318225858.png)

# Boas práticas
Para o correto funcionamento, algumas regras devem ser seguidas

## O que fazer quando quiser adicionar uma nova nota
A primeira coisa a fazer é abrir o terminal e rodar "git pull" para pegar a versão mais recente da nuvem.

Todas as novas notas devem ser adicionadas na pasta "content", sem exceção.

Após isso, você deve rodar os 3 comandos de commit:

1. "git add ."
2. "git commit -m 'Meu commit'"
3. "git push -u origin dev"

AS MUDANÇAS NÃO SÃO INSTANTÂNEAS NO SITE, AGUARDE!

## Imagens
Imagens devem ter seu caminho relativo. Instale o plugin "Wikilinks to MDLinks". Sempre que colar uma imagem, rode o hotkey do plugin em cima do link para que as imagens funcionem no site. Ex: ![Pasted image 20210318230153.png](Pasted%20image%2020210318230153.png)

Apenas esse tipo de link funciona para imagens.

Certifique-se de outra coisa. Essa configuração deve estar exatamente igual: ![Pasted image 20210318230302.png](Pasted%20image%2020210318230302.png)

## Wikilinks
Wikilinks podem ser usados normalmente. ![Pasted image 20210318230836.png](Pasted%20image%2020210318230836.png)

## Pasta content como receptora de novas notas
Altere essa configuração para que novas notas sejam inseridas diretamente na pasta "content"
![Pasted image 20210322161941.png](Pasted%20image%2020210322161941.png)

## Atenção
Não alterar nenhum outro arquivos das outras pastas que não sejam a "content" e a "static".