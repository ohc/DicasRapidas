Dicas Rápidas
=============

Lembra daquele problema que você teve que lhe deu bastante dor de cabeça por não encontrar uma solução. Horas no google, galinhas pretas sacrificadas,
benzederas e nada naquele dia. Até que inexplicavelmente, já sem nenhuma esperança você encontra a luz no fim do túnel.
Você testa, soluciona seu problema e pensa... “Vou salvar isso em um .txt pra não perder mais”. Claro que você vai necessitar dessa dica novamente,
porém muito depois de você lembrar até que teve um problema parecido.

Pensando nisso, este projeto é pra você. Por que não escrever uma dica rápida que possa servir de referência pra você e para o próximo?

De uma forma resumida, descreva seu problema, a solução encontrada e se possível sua fonte.
E você que teve um problema semelhante e teve uma outra forma de solução, compartilhe também sua solução.


Template
--------

**GitHub ID:** desenvolvedor_j <br/>
**Problema:** Tive um problema assim, assim, assado. A repinboca da parafuseta não funcionava, mesmo depois de trocar função foo() por bar(). <br/>
**Solução:** Consegui resolver trocando pela função zoo() e passando um ponteiro de inteiro como argumento <br/>
```
int *x;
int y;

y = zoo(x);
```
**Fonte:** http://www.siteofsolutions.com/tips/problem_with_bar_function.html <br/>

Caso outra pessoa conheça uma outra maneira de solucionar o mesmo problema, ou algum comentário de como poderia melhorar ou mesmo dizer que não funciona
mais na versão XYZ, faça isso logo abaixo.

**GitHub ID:** desenvolvedor_x <br/>
**Sugestão/Comentário:** Esta função foi descontinuada da libfoobarzoo a partir da versão 3.2.48. Neste caso pode usar a sua versão segura. Basta apenas adicionar
s no inicio da função <br/>
```
int *x;
int y;

y = szoo(x);
```

>**Nota 1:** Antes de mais nada, este é apenas um template. O trecho de código aqui colocado não faz sentido nenhum.

>**Nota 2:** Procure evitar colocar apenas o site como referência e não colocar escrever a solução. Este é justamente para evitar que se o site
saia do ar, a solução também se perca ficando mais difícil encontrar algo parecido.

Comitando sua dica ou sugestão
------------------------------
Para que possamos navegar pelas suas dicas nos commits, adote um padrão de mensagens de commits:

Github id - DICA - Mensagem resumida <br/>

(opcional) Descreva de uma maneira bem objetiva sua dica <br/>

No caso de sugestão/comentário:

Github id - COM/SUG - Mensagem da dica <br/>

(opcional) Descreva de uma maneira mais objetiva ainda a sua sugestão <br/>

Go Go Go
========

**GitHub ID:** dropped <br/>
**Problema:** Já enfrentei problemas quando estava gerando um USB Bootável com algumas distribuições quando usava o dd da seguinte maneira: <br/>
```
# dd if=distribuicao_xyz.iso of=/dev/sdb bs=8M
```
Não sei informar o motivo do problema, mas muitas vezes não bootava.<br/>
**Solução:** Usar ddrescue <br/>
```
# ddrescue -d -D --force distribuicao_xyz.iso /dev/sdb
```
Desde então não tive mais problemas desse tipo.<br/>
**Fonte:** https://ubuntu-mate.org/utopic/ <br/>
Outras referências: [GNU](https://www.gnu.org/software/ddrescue/) [ForensicsWiki](http://www.forensicswiki.org/wiki/Ddrescue)
