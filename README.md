# HashifyPass

HashifyPass é uma ferramenta usada para visualização de senhas em websites, como alternativa à utilização da visualização de senha em texto plano. Esta ferramenta busca evitar ataques de shoulder surfing durante a digitação da senha.

O HashifyPass pode ser adicionado a qualquer formulário de login, conforme instruções abaixo.

## Instalação do HashifyPass em um formulário de login genérico

Clone o repositório do HashifyPass localmente, dentro do diretório de interesse:

```git clone https://github.com/decarv/hashify-pass```

No arquivo html que contém o formulário de login, adicione os scripts presentes no diretório ```hashify-pass/src``` (assumindo que o `git clone` foi feito para o diretório hashify-pass):

```
<script type="text/javascript" src="src/libs/jquery-3.4.1.min.js" defer></script>
<script type="text/javascript" src="src/libs/sha.js" defer></script>
<script type="text/javascript" src="src/libs/mo.min.js" defer></script>
<script type="text/javascript" src="src/libs/jsbi.mjs" defer></script>
<script type="text/javascript" src="src/js/custom_fonts.js" defer></script>
<script type="text/javascript" src="src/js/custom_icons.js" defer></script>
<script type="text/javascript" src="src/js/hashify.js" defer></script>
<script type="text/javascript" src="src/js/hashifypass.js" defer></script>
<script type="text/javascript" src="src/js/bundle.js" defer></script>
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
