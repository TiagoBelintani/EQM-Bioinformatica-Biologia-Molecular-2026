# Estrutura do projeto da disciplina

Todos os notebooks usam a mesma raiz no Google Drive:

```text
/content/drive/MyDrive/Bioinformatica_Biologia_Molecular
```

Estrutura padronizada:

```text
Bioinformatica_Biologia_Molecular/
├── 01_bancos/
├── 02_blast/
├── 03_sra_fastq/
│   └── raw-fastq/
├── 04_qc_trimming/
│   ├── fastqc_raw/
│   ├── multiqc_raw/
│   ├── trimmed/
│   ├── fastqc_trimmed/
│   └── multiqc_trimmed/
├── 05_spades/
│   └── spades-assemblies/
│       ├── hypochilus_petrunkevitchi_SRR15736591/
│       └── contigs/
├── 06_uce_match/
│   ├── probes/
│   ├── uce-search-results/
│   └── taxon-set.conf
├── 07_uce_extract/
│   └── taxon-sets/
│       └── all/
├── 08_integracao/
└── ambientes/
```

## Regra de continuidade

Cada aula começa com quatro verificações:

1. preparar o runtime e o ambiente computacional, quando necessário;
2. montar o Google Drive;
3. acessar a raiz e identificar o diretório de entrada/saída;
4. verificar se o arquivo produzido pela aula anterior existe.

Os dados ficam no Drive. Os ambientes Conda ficam no runtime do Colab e podem precisar
ser recriados quando uma nova sessão começa.

## Identificadores

- RUN: `SRR15736591`
- SAMPLE: `hypochilus_petrunkevitchi_SRR15736591`

O RUN rastreia o registro do SRA. O SAMPLE é usado como rótulo consistente nos arquivos
produzidos durante o pipeline.
