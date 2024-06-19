# Biopython

## Biopython 

Biopython es una libreria de python que permite realizar trabajo de bioinformatica de manera sencilla y eficiente, esta libreria permite realizar tareas como:

- Lectura y escritura de archivos de secuencias biologicas.
- Realizar alineamientos de secuencias.
- Transformar secuencias de ADN a ARN y viceversa.
- Realizar traducciones de secuencias de ADN a proteina.
- Analizar secuencias con multiples códigos genéticos(Mitocondrial, Bacteriano, etc).
- Realizar busquedas en bases de datos de secuencias biologicas(Entrez, SwissProt, ExPASy, etc).
- Visualizar estructuras de proteinas en 3D.


## Instalación

La instalacioón de Biopython es muy sencilla, solo necesitas tener instalado python en tu computadora y ejecutar el siguiente comando:

```bash
pip install biopython
```
Biopython es una libreria muy extensa y con muchas funcionalidades, por lo que es recomendable revisar la [documentación de biopython](https://biopython.org/DIST/docs/tutorial/Tutorial.pdf) para conocer todas las funciones que ofrece.

## Ejemplo de uso

### Lectura de secuencias

Biopython permite leer archivos de secuencias en formato fasta, genbank, entre otros. Para leer un archivo de secuencias en formato fasta, puedes utilizar el siguiente código:

```python
from Bio import SeqIO
for record in SeqIO.parse("archivo.fasta", "fasta"):
    print(record.id)
    print(record.seq)
```
Esto nos permite leer los metadatos y la información de la secuencia 

<note>
Los metadatos refieren a la información que acompaña a los datos principales, como en una canción los datos principales son la melodía y los metadatos el nombre, artista o album.
</note>

### Transcripción y Traducción de secuencias

Biopython permite realizar la transcripción y traducción de secuencias de ADN a ARN y de ARN a proteina, respectivamente incluso permitiendo omitir la transcripción y traducción de secuencias de ADN a proteina directamente. Para realizar la transcripción y traducción de una secuencia de ADN, puedes utilizar el siguiente código:

```python
from Bio.Seq import Seq
from Bio.Alphabet import IUPAC
# Secuencia de ADN
dna_seq = Seq("ATGGCCATTGTAATGGGCCGCTGAAAGGGTGCCCGATAG", IUPAC.unambiguous_dna)
# Transcripción
rna_seq = dna_seq.transcribe()
# Traducción
prot_seq = dna_seq.translate()
print(rna_seq)
print(prot_seq)
```

### Alineamiento de secuencias

Es posible usar los algoritmos de alineamiento de secuencias de BLAST para comparar secuencias de ADN, ARN o proteina. Para realizar un alineamiento de secuencias, puedes utilizar el siguiente código:

```python
from Bio.Blast import NCBIWWW
from Bio import SeqIO

# Read the sequence you want to perform the BLAST search with
record = SeqIO.read("my_sequence.fasta", format="fasta")

# Perform the BLAST search
result_handle = NCBIWWW.qblast("blastn", "nt", record.seq)

# Save the result
with open("my_blast.xml", "w") as out_handle:
    out_handle.write(result_handle.read())

# Close the result handle
result_handle.close()
```
