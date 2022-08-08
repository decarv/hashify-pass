# HashifyPass

HashifyPass é uma ferramenta usada para visualização de senhas em websites, como alternativa à utilização da visualização de senha em texto plano. Esta ferramenta busca evitar ataques de shoulder surfing durante a digitação da senha.

O HashifyPass é um trabalho criado com base no trabalho anterior [hashify.js](https://gitlab.com/jorgemiguelribeiro92/hashify). As mudanças em relaçãoao trabalho anterior foram (a) [modificação](https://www.diffchecker.com/BL3EEMHL) do arquivo src/hashify.js; e (b) criação do arquivo src/hashifypass.js.

## Instalação do HashifyPass em um formulário de login

O HashifyPass pode ser adicionado a qualquer formulário de login, conforme instruções abaixo.

Clone o repositório do HashifyPass localmente, dentro do diretório de interesse:

```git clone https://github.com/decarv/hashify-pass```

No arquivo html que contém o formulário de login, adicione os scripts presentes no diretório ```hashify-pass/src``` (assumindo que o `git clone` foi feito para o diretório hashify-pass):

```
<script type="text/javascript" src="hashify-pass/src/libs/jquery-3.4.1.min.js" defer></script>
<script type="text/javascript" src="hashify-pass/src/libs/sha.js" defer></script>
<script type="text/javascript" src="hashify-pass/src/libs/mo.min.js" defer></script>
<script type="text/javascript" src="hashify-pass/src/libs/jsbi.mjs" defer></script>
<script type="text/javascript" src="hashify-pass/src/js/custom_fonts.js" defer></script>
<script type="text/javascript" src="hashify-pass/src/js/custom_icons.js" defer></script>
<script type="text/javascript" src="hashify-pass/src/js/hashify.js" defer></script>
<script type="text/javascript" src="hashify-pass/src/js/hashifypass.js" defer></script>
<script type="text/javascript" src="hashify-pass/src/js/bundle.js" defer></script>
```

No mesmo arquivo, no lugar que desejar, adicione o botão do HashifyPass:

```
<button id="hashifyPassButton" type="button">
  Hashify
</button>
```

O HashifyPass deve estar habilitado no formulário de login a partir de agora. Estilos podem ser aplicados à vontade nos botões e no formulário.

## Vídeo da Instalação

Um vídeo suplementar que segue os passos acima pode ser encontrado [neste link](https://localhost).

## Licença

Este software é distribuído sob a Licença MIT, que pode ser encontrada no arquivo LICENSE neste repositório.
