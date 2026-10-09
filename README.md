# Piloto Mexicano
##### Um script para MKB que reinicia automaticamente suas macros do CloudScript após o login.

- **Como Funciona / Uso**
  - O objetivo deste script é garantir que suas macros do CloudScript sejam iniciadas corretamente ao entrar no servidor.
  - Ele funciona em segundo plano lendo as mensagens do chat. Ao detectar que você logou com sucesso, o script inicia uma contagem de **25 segundos**.
  - Após esse tempo, ele confere se as macros que deveriam ter sido reiniciadas realmente foram. 
  - Caso não tenham sido reiniciadas, ele exibe um alerta pedindo para o usuário cancelar a ação (se desejar). Para cancelar, basta **segurar a tecla `DELETE`**. 
  - Se o usuário não cancelar, o próprio script se encarregará de reiniciar as macros automaticamente.
  - Adicionar uma macro nova nele (para garantir o restart) é bastante simples, desde que você saiba o que está fazendo.

- **Instalação**
  - **Passo 1:** Copie todo o código do script acessando [este link](https://lomexicano.github.io/piloto_mexicano/onChat_piloto_mexicano.txt).
  - **Passo 2:** No menu principal do jogo, vá em `Opções` → `Controles` → `Macro settings...`
  - **Passo 3:** No topo da tela, clique na seta amarela para a direita ("**➤**") para abrir a janela de eventos.
  - **Passo 4:** Abra o segundo evento, chamado `onChat`.
  - **Passo 5:** **NÃO APAGUE NADA** que já estiver lá. Apenas digite o seguinte código: `$$<onChat_piloto_mexicano.txt>`
  - **Passo 6:** Clique em `Arquivos...` (ou `Edit File`), no canto superior direito da tela.
  - **Passo 7:** Digite `onChat_piloto_mexicano` e clique em `Criar`
  - **Passo 8:** Cole o código
  - **Passo 9:** Edite o comando de `/login senha`, no início do código (para que o código consiga fazer login para você)
  - **Passo 10:** Salve tudo

<br />

### Demonstração de Instalação:
<video src="./tutorial/24_fps.mp4" controls width="100%"></video>

<br />

### Referências:
- [Macro KeyBind Mod](https://www.minecraftforum.net/forums/mapping-and-modding-java-edition/minecraft-mods/1275039-macro-keybind-mod), o mod utilizado para rodar este script ~ por [Mumfrey](https://github.com/mumfrey)
- [LiteLoader](https://www.minecraftforum.net/forums/mapping-and-modding-java-edition/minecraft-mods/1290155-liteloader), o carregador de mods necessário para utilizar o MKB ~ por [Mumfrey](https://github.com/mumfrey)
- [Documentação Não Oficial](https://beta.mkb.gorlem.ml/docs/actions/), contendo vasta informação sobre a linguagem de programação customizada criada pelo mod ~ por [Gorlem](https://github.com/Gorlem/)  
- [MKB Syntax Highlighting](https://github.com/KeeMeng/MKB-Syntax-Highlighting), um plugin para o Sublime Text que fornece diversas ferramentas úteis para programadores desta linguagem ~ por [KeeMeng (TKM)](https://github.com/KeeMeng) 
