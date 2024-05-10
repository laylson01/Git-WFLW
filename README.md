### Configurando Git

Após instalar o Git:

1. **Introduza-se ao Git**

Execute os seguintes comandos.

```bash
git config --global user.name "NOME SOBRENOME"
```
```bash
git config --global user.email "MEU_NOME@example.com"
```

2. **Obtenha Segurança (Chave Pública)**

Esta etapa varia de um hospedeiro de repositório para outro, mas é basicamente a mesma. Você deve gerar uma chave pública a partir do seu terminal local e salvá-la no seu hospedeiro de repositório.

Execute os seguintes comandos.

```bash
ssh-keygen -t rsa -b 2048 -C "email@example.com"
```
*Não se esqueça de adaptar os exemplos para os seus dados.*

Agora copie a chave pública usando este comando (Windows) ou *você também pode acessar a interface gráfica para encontrar a pasta .ssh onde a chave foi gerada.*

```bash
cat ~/.ssh/id_ed25519.pub | clip
```

Perfeito, vá para o seu hospedeiro de repositório e cole a chave SSH, juntamente com um titulo da sua maneira


### GITHUB 

**No canto superior direito, vá no seu perfil e clique na opção:**

![image](https://github.com/laylson01/Git-WFLW/assets/81764734/3ea52cd3-6654-4a76-baae-66241b9cf87a)

**Procure por essa opção abaixo e siga o processo:**

![image](https://github.com/laylson01/Git-WFLW/assets/81764734/2e041621-e752-42c1-ac78-6f10a54d1f47)

**Adicione uma nova chave SSH:**

![image](https://github.com/laylson01/Git-WFLW/assets/81764734/42ed98f3-dcab-4382-9cbf-9363b2ac2863)

**Cole a chave que copiou anteriormente:**

![image](https://github.com/laylson01/Git-WFLW/assets/81764734/416ea2ca-d0ad-4b8c-952e-fc91e7d233eb)


Nota: Para um algoritmo melhorado, você pode executar os seguintes comandos e copiar novamente.

```bash
ssh-keygen -o -f ~/.ssh/id_rsa
```
```bash
ssh-keygen -o -t rsa -b 4096 -C "email@example.com"
```


#### Pré-requisito

**Comandos do Linux**

- `mkdir <NomeDaPasta>`: Significa Criar um Diretório, criar uma nova pasta.
- `cd <NomeDaPasta>`: Mover-se para a pasta abaixo.
- `pwd`: Onde estou? Imprimir o diretório de trabalho.
- `ls`: O que há na pasta atual?.
- `touch <nome-do-arquivo>`: Criar um novo arquivo.
- `rm`: remove arquivos/pastas.

#### O que é Git

Git é o sistema de controle de versão mais popular. Ele acompanha as alterações que você cria nos arquivos para que você possa voltar no tempo se necessário. Também auxilia os esforços colaborativos, permitindo que as alterações de várias pessoas sejam mescladas em um código-fonte específico.

**Então, o que é um Repositório Git**

É simplesmente um local onde você mantém e armazena seus pertences do git localmente. Permitindo a criação de um histórico ao longo do tempo.

#### Comandos do Git

- **O que é o GitHub?**
  - `git init`: Inicialize seu repositório git local.
  - `git add <nome-do-arquivo>`: Adicione os arquivos/alterações ao repositório git.
  - `git add .`: Adicione todos os arquivos e alterações no diretório ao repositório git.
  - `git commit -m "Sua mensagem incrível aqui"`: Antes de fazer push, comite as alterações.
  - `git remote add origin <URL do serviço de hospedagem do seu repositório>`: Conecte seu repositório git local a um repositório de hospedagem remota, como GitHub, GitLab ou qualquer outro.
  - `git push -u origin <nome-do-seu-branch>`: Vá em frente e faça push das suas ótimas contribuições!

**Mais Comandos do Git**

#### Inicie o Fluxo de Trabalho

- Navegue até o diretório desejado usando `cd`.
- Assim que chegar, crie uma pasta de projeto com `mkdir`.
- Transfira para o novo projeto usando `cd`.
- Crie os arquivos que deseja uma vez lá usando `touch`.
- `code .` para editar seu trabalho no VS Code, salve e retorne ao terminal.
- Crie seu repositório git usando `git init`.
- Adicione seus arquivos atuais ao repositório git com `git add .`.
- É hora de confirmar suas modificações usando `git commit`.
- Conecte seu repositório git ao repositório externo usando `git remote`.
- Faça push e observe a magia acontecer.

"Pequenos passos podem levar a grandes conquistas. Inicie seu projeto, nutra sua criatividade e compartilhe-a com o mundo."
