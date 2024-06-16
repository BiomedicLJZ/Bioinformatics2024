# Bioinformatica 101

## Los Fundamentos biológicos de la Bioinformatica

### Los ácidos nucleicos y las proteínas

Los ácidos nucleicos son moléculas biológicas que se encargan de almacenar y transmitir la información genética de los seres vivos. Estos están formados por nucleótidos,
los cuales son moléculas compuestas por un azúcar, un grupo fosfato y una base nitrogenada. Se dividen en dos tipos: el ADN y el ARN.

El ADN es la macromolécula que se encarga de almacenar la información genética de los seres vivos. Está formado por una doble cadena de nucleótidos que se enrollan en forma de una doble hélice.

El ARN está encargado de la biosíntesis de proteínas que controla el proceso celular. Se diferencia del ADN en que es una sola cadena de nucleótidos y que en lugar de tener la base nitrogenada Timina(T), tiene Uracilo(U).

La estructura de los nucleótidos es la misma en todos los seres vivos, pero la secuencia de estos nucleótidos es lo que determina la información de cada organismo. Específicamente consisten en una pentosa, un residuo de fosfato y una base nitrogenada heterocíclica.

Cada unidad de la estructura básica de residuo de ribosa/ácido fosfórico lleva una base nucleica heterocíclica que está conectada al residuo de azúcar mediante un enlace N-glucosídico. Los ácidos nucleicos consisten en cinco bases diferentes (citosina, uracilo, timina, adenina y guanina), de las cuales el uracilo se encuentra solo en el ARN y la timina solo en el ADN. Los nucleótidos pueden abreviarse usando la primera letra de la base correspondiente, y su sucesión indica la secuencia de nucleótidos de la cadena de ácido nucleico. ADN y ARN no solo difieren en sus bases, sino que los residuos de azúcar respectivos también difieren en composición química. En el ARN, el azúcar es una ribosa, mientras que en el ADN se incorpora 2-desoxirribosa.

El ADN consiste en dos cadenas de nucleótidos que se combinan en una orientación antiparalela, de modo que se forman enlaces de hidrógeno entre las bases de cada cadena, resultando en una estructura similar a una escalera. Las bases están emparejadas de manera que un anillo de purina en una cadena interactúa con un anillo de pirimidina en la cadena opuesta. Existen dos enlaces de hidrógeno entre A y T y tres entre G y C. Las dos cadenas de nucleótidos que componen el ADN son "complementarias" entre sí. Por lo tanto, la sucesión secuencial de bases en una cadena determina la secuencia de bases en la otra cadena.

En condiciones fisiológicas, el ADN existe como una doble hélice en la cual las dos cadenas de polinucleótidos se enrollan hacia la derecha alrededor de un eje común. El diámetro de la doble hélice es de 2 nm. A lo largo de la doble hélice, las bases opuestas están separadas por 0.34 nm y rotadas en un ángulo de 36° entre sí. La estructura helicoidal se repite cada 3.4 nm y corresponde a 10 pares de bases[1]

![DNARNA](../images/DNARNA.png){thumbnail="true"}{ width=450 height=300}{style="display: block"}
<sub>Imagen obtenida de [Byjus](https://byjus.com/biology/difference-between-dna-and-rna/)</sub>

El ADN consiste de 4 nucleótidos, Adenina(A), Timina(T), Citosina(C) y Guanina(G). Estos nucleótidos se unen mediante enlaces de hidrógeno de la siguiente manera: Adenina se une con Timina y Citosina se une con Guanina. La secuencia de estos nucleótidos es lo que determina la información genética de un organismo.

![ADN](../images/ADN.png){thumbnail="true"}{ width=450 height=300}

## El Dogma Central de la Biología Molecular

El Dogma Central de la Biología Molecular es un principio que describe el flujo de la información genética en los seres vivos. Este principio fue propuesto por Francis Crick en 1958 y establece que la información genética fluye del ADN al ARN y de este al ARN.

El Dogma Central de la Biología Molecular se divide en tres etapas:

1. **Transcripción**: En esta etapa, la información genética del ADN se copia en una molécula de ARN mensajero (mRNA). Esta copia es necesaria para poder llevar la información genética del ADN al ribosoma, donde se produce la proteína.
2. **Traducción**: En esta etapa, la información genética del ARN mensajero se utiliza para producir una proteína. El ARN mensajero se une al ribosoma y se lee el código genético para unir los aminoácidos en la secuencia correcta.
3. **Replicación**: En esta etapa, la información genética del ADN se copia para producir una nueva molécula de ADN. Esta etapa es necesaria para la división celular y la reproducción de los seres vivos.

![DogmaCentral](../images/DogmaCentral.png){thumbnail="true"}{ width=450 height=300}
<sub>Imagen obtenida del libro "Applied Bioinformatics de Paul M. Selzer"</sub>

Las proteínas son macromoléculas que están formadas por aminoácidos. Existen 20 aminoácidos que se unen mediante enlaces peptídicos para formar las proteínas.

Los aminoácidos son moléculas que contienen un grupo amino `(-NH2)` y un grupo carboxilo `(-COOH).` Además, contienen un grupo `R` que es diferente en cada aminoácido. Este grupo R es el que determina la estructura y función de cada aminoácido.

Para poder formar una proteína, el RNA mensajero(mRNA) sale del núcleo de la célula y se une a un ribosoma. El ribosoma lee el mRNA y utiliza el código genético para unir los aminoácidos en la secuencia correcta. Esta secuencia de aminoácidos forma la proteína.

Cada aminoácido es seleccionado dependiendo de la secuencia de nucleótidos en el mRNA. Cada secuencia de tres nucleótidos en el mRNA se llama codon y codifica para un aminoácido específico. Por ejemplo, el codon AUG codifica para el aminoacido Metionina. Esto es posible gracias a los RNA de transferencia(tRNA) que se encargan de llevar los aminoacidos al ribosoma y poseen una secuencia complementaria al codon del mRNA, esto hace que exista una correspondencia entre los codones y los aminoacidos.

![tRNA](../images/bioinfo101/codonanticodon.png){thumbnail="true"}{ width=450 height=300}
<sub>Imagen obtenida de [Wikipedia](https://es.wikipedia.org/wiki/ARN_de_transferencia)</sub>

#### El código genético

El código genético es el conjunto de reglas que determina cómo se traduce la información genética del ADN en proteínas. Cada triplete de nucleótidos (codón) codifica para un aminoácido específico.

El código genético es universal, es decir, es el mismo para todos los seres vivos. Sin embargo, existen algunas excepciones a esta regla.

![CodigoGenetico](../images/aminoacidos/genecode.png){thumbnail="true"}{ width=450 height=300}

<table>
<tr><td>Aminoácido</td><td>Abreviatura</td><td>Codones</td><td>Estructura</td></tr>
<tr><td>Alanina</td><td>Ala</td><td>GCU, GCC, GCA, GCG</td><td><img src="../images/aminoacidos/alanina.png" alt="Alanina" /></td></tr>
<tr><td>Arginina</td><td>Arg</td><td>CGU, CGC, CGA, CGG, AGA, AGG</td><td><img src="../images/aminoacidos/arginina.png" alt="Arginina" /></td></tr>
<tr><td>Asparagina</td><td>Asn</td><td>AAU, AAC</td><td><img src="../images/aminoacidos/asparagina.png" alt="Asparagina" /></td></tr>
<tr><td>Ácido aspártico</td><td>Asp</td><td>GAU, GAC</td><td><img src="../images/aminoacidos/aspartato.png" alt="Aspartato" /></td></tr>
<tr><td>Cisteina</td><td>Cys</td><td>UGU, UGC</td><td><img src="../images/aminoacidos/cisteina.png" alt="Cisteina" /></td></tr>
<tr><td>Glutamina</td><td>Gln</td><td>CAA, CAG</td><td><img src="../images/aminoacidos/glutamina.png" alt="Glutamina" /></td></tr>
<tr><td>Ácido glutámico</td><td>Glu</td><td>GAA, GAG</td><td><img src="../images/aminoacidos/glutamato.png" alt="Glutamato" /></td></tr>
<tr><td>Glicina</td><td>Gly</td><td>GGU, GGC, GGA, GGG</td><td><img src="../images/aminoacidos/glicina.png" alt="Glicina" /></td></tr>
<tr><td>Histidina</td><td>His</td><td>CAU, CAC</td><td><img src="../images/aminoacidos/histidina.png" alt="Histidina" /></td></tr>
<tr><td>Isoleucina</td><td>Ile</td><td>AUU, AUC, AUA</td><td><img src="../images/aminoacidos/isoleucina.png" alt="Isoleucina" /></td></tr>
<tr><td>Leucina</td><td>Leu</td><td>UUA, UUG, CUU, CUC, CUA, CUG</td><td><img src="../images/aminoacidos/leucina.png" alt="Leucina" /></td></tr>
<tr><td>Lisina</td><td>Lys</td><td>AAA, AAG</td><td><img src="../images/aminoacidos/lisina.png" alt="Lisina" /></td></tr>
<tr><td>Metionina</td><td>Met</td><td>AUG</td><td><img src="../images/aminoacidos/metionina.png" alt="Metionina" /></td></tr>
<tr><td>Fenilalanina</td><td>Phe</td><td>UUU, UUC</td><td><img src="../images/aminoacidos/fenilalanina.png" alt="Fenilalanina" /></td></tr>
<tr><td>Prolina</td><td>Pro</td><td>CCU, CCC, CCA, CCG</td><td><img src="../images/aminoacidos/prolina.png" alt="Prolina" /></td></tr>
<tr><td>Serina</td><td>Ser</td><td>UCU, UCC, UCA, UCG, AGU, AGC</td><td><img src="../images/aminoacidos/serina.png" alt="Serina" /></td></tr>
<tr><td>Treonina</td><td>Thr</td><td>ACU, ACC, ACA, ACG</td><td><img src="../images/aminoacidos/treonina.png" alt="Treonina" /></td></tr>
<tr><td>Triptófano</td><td>Trp</td><td>UGG</td><td><img src="../images/aminoacidos/triptofano.png" alt="Triptofano" /></td></tr>
<tr><td>Tirosina</td><td>Tyr</td><td>UAU, UAC</td><td><img src="../images/aminoacidos/tirosina.png" alt="Tirosina" /></td></tr>
<tr><td>Valina</td><td>Val</td><td>GUU, GUC, GUA, GUG</td><td><img src="../images/aminoacidos/valina.png" alt="Valina" /></td></tr>
</table>

Las proteínas son esenciales para la vida de los seres vivos, ya que son las encargadas de realizar la mayoría de las funciones biológicas. Estas funciones incluyen la catálisis de reacciones químicas, la replicación del ADN, la respuesta inmune, el transporte de oxígeno, entre otras.

## La Bioinformatica en acción

### Análisis de secuencias

El análisis de secuencias es una de las áreas más importantes de la bioinformatica. Este análisis se encarga de estudiar las secuencias de ADN y proteínas para determinar su función, estructura y evolución.

### Alineamiento de secuencias

El alineamiento de secuencias es una técnica que se utiliza para comparar dos o más secuencias de ADN o proteínas. Esta técnica se utiliza para determinar la similitud entre las secuencias y para identificar regiones conservadas.

### Búsqueda de secuencias

La búsqueda de secuencias es una técnica que se utiliza para encontrar secuencias de ADN o proteínas en bases de datos. Esta técnica se utiliza para identificar genes, proteínas y otras moléculas biológicas.

### Análisis de expresión genética

El análisis de expresión genética es una técnica que se utiliza para estudiar la expresión de genes en diferentes condiciones. Esta técnica se utiliza para identificar genes que están involucrados en enfermedades, para estudiar el desarrollo de los organismos y para comprender la respuesta de los organismos a los estímulos ambientales.

### Modelado de proteínas

El modelado de proteínas es una técnica que se utiliza para predecir la estructura tridimensional de las proteínas. Esta técnica se utiliza para comprender la función de las proteínas y para diseñar nuevas proteínas.

## Aplicaciones de la Bioinformatica

### Medicina

La bioinformatica se utiliza en medicina para el diagnóstico de enfermedades, el desarrollo de nuevos fármacos y la medicina personalizada.

### Agricultura

La bioinformatica se utiliza en agricultura para mejorar los cultivos, para desarrollar nuevas variedades de plantas y para controlar las plagas.

### Biotecnología

La bioinformatica se utiliza en biotecnología para el desarrollo de nuevos productos, para la producción de alimentos y para la producción de biocombustibles.

