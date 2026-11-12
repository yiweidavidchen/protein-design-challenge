# A World Without One Amino Acid

*How much function can a protein keep after one letter is removed from its alphabet?*

**Yiwei Chen · Challenge proposal v0.1 · Draft for review**

## 1. The challenge

Take a protein with a known function and remove one amino acid type from its design alphabet. Can you recover the original function using only the other 19 canonical amino acids? Which sites can be rescued by a direct replacement, and which require changes elsewhere in the protein?

Each round excludes one canonical amino acid from the final sequence of the designed protein. The free amino acid may still participate in metabolism in the standard round. The first round excludes tryptophan (Trp).

## 2. First round — A World Without Trp

Organizers provide a reference sequence and structure, specify a functional assay, and measure folding or stability independently. A good pilot target would have a few Trp residues, including at least one with a plausible contribution to binding or catalysis. Teams would predict which Trp is hardest to replace and explain what they expect to lose at that site, such as an aromatic contact, side-chain volume, or a hydrogen bond involving the indole NH.

| Comparison | What it tests |
| --- | --- |
| Original protein | How much function and stability the starting protein has under the assay conditions. |
| Trp-free design with changes limited to original Trp sites | How much function can be retained by replacing those side chains directly. |
| Paired Trp-free design with the same replacements at the original Trp sites and changes at up to *k* other positions | How much additional function compensatory mutations can recover under a shared budget that counts only positions outside the original Trp sites. |

Each team first submits a design that changes only the original Trp sites. Its paired design keeps those exact replacements and may change up to *k* additional positions. The shared budget counts only changes outside the original Trp sites. Teams also submit a predicted functional ranking and explain how the additional changes might help. Report retained function relative to the original protein and report folding or stability as a separate readout. Label computational predictions explicitly. The pilot would set the value of *k* and the assay thresholds.

## 3. Where does the freed codon go?

In the standard genetic code, UGG encodes Trp. In a separate computational task, each team assigns UGG to one of the remaining canonical amino acids and explains its choice. The assignment is independent of the substitutions in the protein designs. A team could replace one Trp with Tyr and another with Phe while assigning UGG to Leu.

To compare recoding costs, all teams use the same reference coding sequences and fixed, aligned Trp-free target protein sequences. Each team estimates the minimum number of codon positions it would need to change to encode those targets under its proposed assignment. Organizers score the codon task independently of protein performance.

## 4. Later rounds — Ile and Met

**A World Without Ile.** A pilot could focus on a protein with several buried Ile residues. Teams would predict where Val could retain the local branching geometry, where Leu could fill the available volume, and where compensatory changes would be needed. The codon task could ask whether to keep AUU, AUC, and AUA together or assign them separately.

**A World Without Met.** The first version would require the mature protein to contain zero Met and allow a transient initiator Met that is removed during processing. A suitable target could distinguish ordinary hydrophobic packing from a site that depends on the sulfur-containing side chain. A stricter conceptual variant would also exclude Met from the nascent chain and treat translation initiation as a separate design question.

## 5. Hard mode — A world without the free amino acid

Hard mode extends the restriction to a defined metabolic module. Within that module, the excluded amino acid cannot appear in free form as an input, intermediate, or product. For each hard-mode round, organizers specify the module boundary, starting inputs, target output, and permitted derivatives and externally supplied cofactors. All teams assess whether the module can produce the target output under those same conditions. The pilot would establish the specific conditions.

For example, the standard Trp-free round could use a protein that acts on free Trp. Hard mode could instead specify a downstream output and ask whether that output is compatible with a route that never requires free Trp. A first pilot would assess the proposed pathways as a reasoning exercise. Applying the restriction to a whole cell would be a separate research question.

## 6. Pilot feedback

Can you suggest a model protein with a well-characterized Trp site and separate readouts for function and folding or stability?
