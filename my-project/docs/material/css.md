# CSS (Cascading Style Sheets)

## O que é o CSS?

O **CSS** é uma linguagem de estilo utilizada para definir a apresentação de documentos escritos em HTML. Enquanto o HTML é responsável pela **estrutura** do site e pela separação semântica do conteúdo, o CSS cuida exclusivamente da **estilização** dessas páginas. Com esse recurso, é possível aplicar cores, tamanhos, bordas, fontes e formas aos elementos HTML.

Antes da criação do CSS, a estilização dos sites era aplicada diretamente na própria página HTML. Por conta disso, a pessoa desenvolvedora Front-End precisava estilizar cada componente de maneira redundante e repetitiva. Com o surgimento do CSS, tornou-se possível centralizar toda a estilização em arquivos específicos. Assim, define-se o estilo de uma tag (ou classe) uma única vez, e ele é aplicado a todo o projeto.

---

## Como Utilizar o CSS

Existem algumas formas de aplicar o CSS ao HTML, sendo a mais recomendada a **Folha de Estilo Externa**. Para isso, criamos um arquivo com a extensão `.css` (por exemplo, `style.css`) e o importamos dentro da tag `<head>` do arquivo HTML utilizando a tag `<link>`.

### Exemplo de Importação:

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minha Página</title>
    <link rel="stylesheet" href="style.css"> <!--Exemplo de importação de arquivo css-->
</head>
<body>
    <h1>Olá, Mundo!</h1>
</body>
</html>

```

> 📌 **Nota:** A tag `<link>` precisa de pelo menos dois atributos essenciais para funcionar corretamente:
> * `rel="stylesheet"`: Indica que o link se refere a uma folha de estilo.
> * `href="style.css"`: Especifica o caminho/nome do arquivo CSS que será carregado.
> 
> 

Com essa importação, os arquivos de estrutura (HTML) e de estilo (CSS) ficam vinculados, permitindo uma manutenção muito mais organizada e escalável do código.

---
