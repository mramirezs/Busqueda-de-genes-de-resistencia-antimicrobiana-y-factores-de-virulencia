# Busqueda-de-genes-de-resistencia-antimicrobiana-y-factores-de-virulencia

## Instalación del programa de búsqueda



## Búsqueda de factores de virulencia

* Usando la base de datos de ecoh

```
for file in $(ls *.pseudocontig.fsa | sed 's/.pseudocontig.fsa//g'); do abricate --db ecoh ${file}.pseudocontig.fsa > ../abricate/${file}_ecoh.tab;done
```

* Usando la base de datos de card

```
for file in $(ls *.pseudocontig.fsa | sed 's/.pseudocontig.fsa//g'); do abricate --db card ${file}.pseudocontig.fsa > ../abricate/${file}_card.tab;done
```

* Usando la base de datos de argannot

```
for file in $(ls *.pseudocontig.fsa | sed 's/.pseudocontig.fsa//g'); do abricate --db argannot ${file}.pseudocontig.fsa > ../abricate/${file}_argannot.tab;done
```

* Usando la base de datos VFDB

```
for file in $(ls *.pseudocontig.fsa | sed 's/.pseudocontig.fsa//g'); do abricate --db vfdb ${file}.pseudocontig.fsa > ../abricate/${file}_vfdb.tab;done
```

* Usando la base de datos ecoli_vf

```
for file in $(ls *.pseudocontig.fsa | sed 's/.pseudocontig.fsa//g'); do abricate --db ecoli_vf ${file}.pseudocontig.fsa > ../abricate/${file}_ecoli_vf.tab;done
```

* Usando la base de datos resfinder

```
for file in $(ls *.pseudocontig.fsa | sed 's/.pseudocontig.fsa//g'); do abricate --db resfinder ${file}.pseudocontig.fsa > ../abricate/${file}_resfinder.tab;done
```

* Usando la base de datos ncbi

```
for file in $(ls *.pseudocontig.fsa | sed 's/.pseudocontig.fsa//g'); do abricate --db ncbi ${file}.pseudocontig.fsa > ../abricate/${file}_ncbi.tab;done

```


Para obtener el resumen de la búsqueda:

```
abricate --summary results/abricate/SA68_vfdb.tab > results/abricate/SA68_vfdb_summary.tab
```
