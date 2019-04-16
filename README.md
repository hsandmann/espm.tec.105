## Welcome to GitHub Pages

Material de apoio à disciplina TEC-105, ministrada na ESPM - Escola Superior de Propaganda e Marketing.





## Máquina de Turing

Proposta pelo matemático Alan Turing, trata de uma máquina de computação universal que tem funcionalidade processar símbolos e suportar programação dinâmica<sup>[1](##Referências)</sup>. 

De forma resumida, a máquina de Turing propõe um cabeçalho e uma fita, onde o cabeçalho lê símbolos da fita executa a operação ali descrita. Generalizando, é uma forma de construir um autômato.

![Máquina de Turing](/assets/img/turing_tape_header.png)

O funcionamento da máquina se resume ao algoritmo de:
1. Ler o posição da fita;
2. Interpreta o símbolo;
3. Executa a operação ali descrita;
4. Vai para a próxima posição da fita;
5. Volta para o passo **1**.
 
Ao analisar o resumo do algoritmo, é possível levar a questão da parada da máquina, um problema tratado no artigo de Turing.

## Arquitetura von Neumann

Baseando na teoria da máquina de Turing, o físico e matemático [John von Neumann](https://en.wikipedia.org/wiki/John_von_Neumann) desenvolveu uma arquitetura que era capaz de executar tal tarefa, a arquitetura de Von Neumann ou arquitetura de Princeton.

![von Neumann Architecture](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e5/Von_Neumann_Architecture.svg/2880px-Von_Neumann_Architecture.svg.png)
*![Wikipedia](https://en.wikipedia.org/wiki/Von_Neumann_architecture)*

Onde o cabeçalho passa a ser uma CPU (Central Processing Unit), que lê os símbolos da fita - a fita moderna é a memória RAM - e executa o comando. O comando por sua vez está construindo em portas lógicas e contído em uma ALU (Arithmetic/Logic Unit).

## Simulador ESPM 16bits

This processor has a set of 16 instructions implemmented into its ALU (Arithmetic Logic Unit).



## Referências

1. Turing, A. M. (1936). ["On Computable Numbers, with an Application to the Entscheidungsproblem"](/assets/pdf/Turing_Paper_1936.pdf)




 sds
You can use the [editor on GitHub](https://github.com/hsandmann/espm.tec.105/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/hsandmann/espm.tec.105/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
