Projeto da Fabrica de Picoles.

Uma empresa fabricante de picolés deseja armazenar informações acerca de seus negócios. Os picolés fabricados são divididos em normal (com água) e ao leite. As informações comuns armazenadas dos picolés são: sabor, ingredientes, preço e tipo da embalagem. Especificamente, picolés normais possuem um conjunto de aditivos nutritivos (vitaminas ou sais minerais) cada um com nome e fórmula química; e picolés ao leite contêm um conjunto de conservantes, cada um com nome e descrição. Os dois tipos de picolés são vendidos em lotes exclusivos (ou normais, ou ao leite) para os revendedores e cada venda gera uma nota fiscal que pode conter um ou vários lotes.   As notas fiscais possuem data, valor, número de série e descrição. Todo revendedor possui uma pessoa de contato para eventuais resoluções de problemas, além disso, armazena-se do revendedor o CNPJ e a razão social. Deseja-se obter relatórios sobre as vendas mensais dos picolés de cada tipo e quais revendedores compraram mais picolés nos últimos meses.

============================================================================================

[1] Os picolés fabricados são divididos em normal (com água) e ao leite. As informações comuns armazenadas dos picolés são: sabor, ingredientes, preço e tipo da embalagem.

Entidades: 
- picoles (id, id sabor, preço, id tipo da embalagem);
- tipos de picole (id, nome);
- tipo da embalagem (id, nome);
- Ingredientes (id, nome);
- Ingredientes Picole (id, id ingrediente, id picole);
- sabor (id, nome);

OBS: um picole pode ter varios ingredientes;

-----------------------------------------------------------------------

[2] Especificamente, picolés normais possuem um conjunto de aditivos nutritivos (vitaminas ou sais minerais)cadaum com nome e fórmula química; e picolés ao leite contêm um conjunto de conservantes,cada um com nome e descrição.

Entidades:
- Aditivos Nutritivos (id, nome, formula quimica);
- Conservantes (id, nome, descrição);
- aditivos Nutritivos picole (id, id aditivo nutritivo, id picole);
- Conservantes Picole (id, id conservantes, id picole);
-----------------------------------------------------------------------

[3] Os dois tipos de picolés são vendidos em lotes exclusivos(ou normais,ou ao leite) para os revendedores e cada venda gera uma nota fiscal que podeconterumouvários lotes. As notas fiscais possuem data, valor, número de série e descrição. 

Entidades:
- Lotes (id, tipo picole, quantidade);
- Nota Fiscal (id, valor, numero de serie, descrição);
- lotes nota fiscal (id, id lote, id nota fiscal);
-----------------------------------------------------------------------

[4] Todo revendedor possui uma pessoa de contato para eventuais resoluções de problemas, além disso, armazena-sedo revendedor o CNPJ e a razão social. 

Entidades:
- Revendedor (id, cnpj, razão social, contato);