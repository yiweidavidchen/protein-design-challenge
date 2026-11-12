# The Zero-A Enzyme Challenge

*Can we program stereoselectivity with a fixed cofactor?*

**Yiwei Chen · Challenge proposal v0.1 · Open for feedback**

## 1. The premise

In *Super Mario 64*, pressing A makes Mario jump. In the community’s A Button Challenge (ABC), players try to minimize A presses for a single mission or across an entire save file. What if we set a similar constraint in enzyme design? In Zero-A, the rule forbids protein residues from carrying out specified chemical steps. [Ukikipedia’s A Button Challenge page](https://ukikipedia.net/wiki/A_Button_Challenge)

Every team starts with the same protein scaffold, catalytic cofactor, and substrate. The task is to design variants that favor opposite enantiomers and declare which variants should favor R and which should favor S before testing.

Mutations in artificial metalloenzymes can change a metal catalyst’s selectivity. How reliably can we predict from the sequence which enantiomer a variant will favor? And can we predict what will happen when we change the substrate?

## 2. What counts as pressing A?

A residue presses A if it forms a covalent intermediate with the substrate or directly transfers a proton, hydride, or electron to or from the substrate or a substrate-derived intermediate. A residue also presses A if it mediates a water relay that reaches the substrate without going through the designated cofactor.

Residues may bind and position the substrate, stabilize a transition state, anchor the cofactor, or alter its coordination environment. A residue may exchange a proton with the cofactor when the cofactor itself mediates transfer to the substrate.

Organizers would measure performance for every entry and examine plausible alternative pathways for the strongest designs. Product ratios and cofactor dependence alone cannot establish mechanistic eligibility. Ruling out an alternative such as direct proton exchange between a residue and the substrate may require additional evidence. If the pathway remains unresolved, the Zero-A assignment is provisional.

## 3. The design task

Organizers supply the starting scaffold, specify the shared catalytic cofactor, make the first substrate public, and give each team the same number of experimental slots. Teams submit a ranked set of sequences covering both target configurations. For each sequence, they declare the predicted major enantiomer and a range for the expected enantiomeric excess, with a short rationale. Organizers lock the sequences and these predictions before experimental results are available.

Once the sequences are locked, organizers reveal a second substrate. Teams predict the major enantiomer and approximate enantiomeric excess for their existing designs before organizers release any assay results. Selectivity can weaken or reverse on the second substrate. Correctly predicting such a change counts toward the transfer score.

## 4. A candidate pilot system

One candidate is an artificial transfer hydrogenase built from streptavidin and a biotinylated ruthenium complex. Biotin anchors the complex in the protein, and the ruthenium complex mediates the reduction. Letondor and colleagues demonstrated asymmetric ketone reduction with this class of catalysts and showed that streptavidin mutations could tune selectivity. [1, 2]

I propose reducing acetophenone to 1-phenylethanol as the calibration reaction. Before the challenge opens, the pilot would test the selected scaffold and complex on acetophenone. It would establish whether product formation and enantiomer ratios can be measured reproducibly and whether cofactor loading can be quantified independently. The controls would include the starting scaffold with the cofactor, the free complex, and the scaffold without added complex.

Acetophenone provides a model for comparing designs. Asymmetric ketone reduction can also produce chiral alcohol intermediates. An industrial follow-up could use a substrate whose existing route falls short on selectivity, conversion, or catalyst use.

## 5. What would count as success?

A design’s selectivity counts toward the design score only if it meets minimum conversion and turnover thresholds. The pilot would set both thresholds and an enantiomeric excess cutoff above assay uncertainty. The design score would report the fraction of submitted variants that meet their declared R or S targets and whether each team succeeded in both directions. The second-substrate predictions would receive a separate score.

A small set of randomly selected pocket variants and variants designed by a simple structural rule would provide baselines. Organizers would report each team’s best result alongside results for its full submission. Equal experimental slots give teams the same number of tests, and teams can use different amounts of computation to choose their entries.

The public dataset would pair sequences and locked predictions with cofactor loading, turnover, conversion, and product ratios where measurable. It would include unsuccessful designs and identify entries that could not be scored. Two active variants that favor opposite enantiomers as predicted would demonstrate control of stereoselectivity in this system. A follow-up could ask whether that control comes from substrate orientation, metal coordination, or another effect.

## 6. Feedback sought

What enzyme–cofactor system would you choose for a small pilot in which cofactor loading, turnover, and stereoselectivity can all be measured independently?

## References

1. Letondor C, Humbert N, Ward TR. Artificial metalloenzymes based on biotin-avidin technology for the enantioselective reduction of ketones by transfer hydrogenation. *PNAS* (2005). [doi:10.1073/pnas.0409684102](https://doi.org/10.1073/pnas.0409684102)
2. Letondor C et al. Artificial transfer hydrogenases based on the biotin-(strept)avidin technology: fine tuning the selectivity by saturation mutagenesis of the host protein. *JACS* (2006). [doi:10.1021/ja061580o](https://doi.org/10.1021/ja061580o)
