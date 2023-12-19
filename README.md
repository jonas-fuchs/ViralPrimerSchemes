# ViralPrimerSchemes
This repo contains wet-lab evaluated and non-evaluated primer schemes for full-viral genome sequencing of highly diverse viral pathogens designed with [varVAMP](https://github.com/jonas-fuchs/varVAMP).

## Tiled schemes
Primers can contain ambiguous characters in order to achieve pan-specificity. We recommend using a [One-Step-RTPCR Protocol](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/wet_lab_protocol.md) at 60°C primer annealing for 35 to 40 cycles. Due to the variability of some viruses, we can not garantuee that the primers will work for every sample you are trying to sequence but for the large majority they should perform resonably well. Happy sequencing!

| Virus      | Genotypes              | Amplicon Size | GenomeRecovery | Evaluated             | Primers                                        | Input alignment                         | Full varVAMP output                  |
|------------|------------------------|---------------|----------------|-----------------------|------------------------------------------------|-----------------------------------------|--------------------------------------|
| HEV        | 3 (f, e)               | 1000-1500     | 99.0 %         | :white_check_mark:    | [tsv](varvamp_tiled/HEV_1/cluster1primers.tsv) | [aln](input_alignments/HEV_1.aln)       | [output](varvamp_tiled/HEV_1)        |
| HEV        | 3 (c, h1, m, i, uc, l) | 1000-1500     | 99.3 %         | :white_check_mark:    | [tsv](varvamp_tiled/HEV_2/cluster2primers.tsv) | [aln](input_alignments/HEV_2.aln)       | [output](varvamp_tiled/HEV_1)        |
| ratHEV     | all                    | 1200-1700     | 97.4 %         | :white_check_mark:    | [tsv](varvamp_tiled/ratHEV/primers.tsv)        | [aln](input_alignments/rat_HEV.aln)     | [output](varvamp_tiled/ratHEV)       |
| Polio      | 1-3                    | 1000-1400     | 99.6 %         | :white_check_mark:    | [tsv](varvamp_tiled/Polio/primers.tsv)         | [aln](input_alignments/polio1-3.aln)    | [output](varvamp_tiled/Polio)        |
| HAV        | all                    | 1000-1600     | 95.6 %         | :white_check_mark:    | [tsv](varvamp_tiled/HAV/primers.tsv)           | [aln](input_alignments/HAV.aln)         | [output](varvamp_tiled/HAV)          |
| BoDV       | all                    | 400-550       | 98.6 %         | :white_check_mark:    | [tsv](varvamp_tiled/BoDV/primers.tsv)          | [aln](input_alignments/BoDV.aln)        | [output](varvamp_tiled/BoDV)         |
| SARS-CoV-2 | B.1-XBB                | 260-365       | 99.7 %         | :black_square_button: | [tsv](varvamp_tiled/SARS-CoV-2_1/primers.tsv)  | [aln](input_alignments/SARS-CoV-2.aln)  | [output](varvamp_tiled/SARS-CoV-2_1) |
| SARS-CoV-2 | B.1-XBB                | 700-800       | 99.7 %         | :black_square_button: | [tsv](varvamp_tiled/SARS-CoV-2_2/primers.tsv)  | [aln](input_alignments/SARS-CoV-2.aln)  | [output](varvamp_tiled/SARS-CoV-2_2) |
| Norovirus  | non-G.II.4 G.II        | 1500-2000     | 99.0 %         | :black_square_button: | [tsv](varvamp_tiled/Norovirus_1/primers.tsv)   | [aln](input_alignments/Norovirus_1.aln) | [output](varvamp_tiled/Norovirus_1)  |
| Norovirus  | G.II.4                 | 1200-1600     | 99.6 %         | :black_square_button: | [tsv](varvamp_tiled/Norovirus_2/primers.tsv)   | [aln](input_alignments/Norovirus_2.aln) | [output](varvamp_tiled/Norovirus_2)  |

## qPCR schemes
| Virus | Genotypes | Evaluated          | Primers                                       | Input alignment                      | Full varVAMP output             |
|-------|-----------|--------------------|-----------------------------------------------|--------------------------------------|---------------------------------|
| Polio | 1         | :white_check_mark: | [tsv](varvamp_qpcr/polio1/qpcr_primers.tsv)   | [aln](input_alignments/polio1.aln)   | [output](varvamp_qpcr/polio1)   |
| Polio | 2         | :white_check_mark: | [tsv](varvamp_qpcr/polio2/qpcr_primers.tsv)   | [aln](input_alignments/polio2.aln)   | [output](varvamp_qpcr/polio2)   |
| Polio | 3         | :white_check_mark: | [tsv](varvamp_qpcr/polio3/qpcr_primers.tsv)   | [aln](input_alignments/polio3.aln)   | [output](varvamp_qpcr/polio3)   |
| Polio | 1-3       | :white_check_mark: | [tsv](varvamp_qpcr/polio1-3/qpcr_primers.tsv) | [aln](input_alignments/polio1-3.aln) | [output](varvamp_qpcr/polio1-3) |

If you just want to use the primers, just go for the `tsv` files in the primer section. If you are interested in the full varVAMP output (here you can also find additional non-used primers) have a look at the input alignment to get a feeling for the variability and have a look [here](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/output.md) for an explanation on the output files. If you want to design primers yourself, the outputs can also help you in understanding [how the software works](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/how_varvamp_works.md) and [how to prepare the data](https://github.com/jonas-fuchs/varVAMP/blob/master/docs/preparing_the_data.md) and set the parameters for a successful scheme design.


## Large THANK you...

...to all the people to have contributed to these primer designs by providing input alignments :beer:, did primer designs :wine_glass: and wet-lab evaluated primer schemes :cocktail:

- **Mathias Schemmerer** (Universitätsklinikum Regensburg, Germany): HAV :beer::cocktail:, HEV :beer:, ratHEV :beer:, BoDV :beer::cocktail:
- **Johanna Kleine** (Universitätsklinikum Freiburg, Germany): HEV :cocktail::wine_glass::beer:
- **Sindy Böttcher**, **Julian Kreibich** (Robert Koch Institute, Berlin, Germany): Polio :cocktail:
- **Martin Hölzer** (Robert Koch Institute, Berlin, Germany): SARS-CoV-2 :beer:


## Contributing

If you designed and/or wet-lab evaluated primer schemes that we should include here, just contribute via an issue or pull request!

## Citing this repo

If you use primers from this repository please cite:
Coming soon!




