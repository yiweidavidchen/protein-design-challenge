# Redesign the Protein Alphabet

**Yiwei Chen · Challenge proposal v0.1 · Open for feedback**

**Format** — Proposed scientific hackathon with a benchmark still to be developed.

## 1. The Challenge

Suppose you had to give up two of the 20 canonical amino acids. What new side chains would you add, and what would make them worth keeping?

Each team removes exactly two canonical amino acids and designs exactly three distinct noncanonical amino acids (ncAAs) of its own. Teams explain their deletions and additions. The resulting alphabet has 21 members.

## 2. The Scientific Question

For a given set of protein tasks, which capabilities of deleted residues can the remaining alphabet take over? Which new capabilities would justify adding a building block?

An alternative alphabet might recover a function lost after a deletion, preserve a protein's original function while enabling a new one, or reveal a trade-off between the two. If the standard alphabet performs better, the comparison can show which tasks give the alternatives trouble.

## 3. Design Rules

### 3.1 Alphabet composition

Teams must specify the structures of their three additions. Protein designs may use only residues from the resulting alphabet. Close analogues of deleted residues are eligible when the team can explain what chemical or structural difference makes the replacement worth testing.

### 3.2 Candidate chemistry

A reference library could provide examples, structures, and modeling resources. For a shorter pilot, teams could select from a shared, prevalidated candidate library and evaluate their choices with the same tools.

### 3.3 Functional responsibility

For each deletion, explain what might be lost and how the remaining alphabet could compensate. For each addition, identify a specific capability, a protein context in which it could matter, a measurable prediction, and a likely liability. Teams can test the three additions across different proteins or tasks.

### 3.4 Biological feasibility

Consider folding compatibility, chemical stability, and a plausible route to making and incorporating each residue. Identify which steps have experimental precedent and which remain hypothetical. A computational entry can propose a validation route without building an alternative translation system.

## 4. Proposed Benchmark

A first benchmark could use a small panel of protein tasks with distinct readouts, such as retaining stability, preserving or changing binding, and preserving or changing a catalytic function. Compare alphabets on the same tasks under comparable design and evaluation budgets.

| Alphabet | What it tests |
| --- | --- |
| 20 canonical amino acids | How the standard alphabet performs after redesign under the same task conditions. |
| 18 canonical amino acids | How much function the team can recover after its two deletions using the remaining canonical residues. |
| 18 canonical amino acids + 3 ncAAs | How much the proposed additions recover or extend beyond the corresponding 18-letter design. |

Report recovery of original function separately from gains in new function. For a claimed benefit at a specific ncAA site, compare the design with a matched variant that uses the best allowed canonical replacement at that site where feasible.

The proposed alphabet has one more member than the standard alphabet. An optional size-matched comparison against 20 canonical amino acids plus one ncAA would help test whether the proposed composition offers an advantage at the same alphabet size. Report experimental measurements, model predictions, and untested chemical assumptions separately.

## 5. Scoring

Score the degree to which a design retains its original function, the evidence for an added capability, and the feasibility of producing and evaluating the proposed residues. Evaluate the team's chemical reasoning against its stated predictions and controls.

Set minimum feasibility requirements and publish the task-specific metrics, thresholds, and any leaderboard weights before evaluation. Report individual measurements and trade-offs alongside any combined score. The pilot would establish which metrics and thresholds are practical.

## 6. Optional Track for New Side-Chain Chemistry

An exploratory track could ask teams to include at least one addition with a chemical or structural capability they expect to be difficult to reproduce with the available residues.

| Example | A question to test |
| --- | --- |
| Sulfonate-bearing ncAA | Could a sulfonate serve as an anionic counterpart to the cationic side chains of Arg and Lys? Compare it with a canonical carboxylate to test what the sulfonate group itself contributes to a specified interaction. |
| Short amidino ncAA (Asp/Asn-derived amidino analogue) | Can a shorter side chain bearing an amidino group preserve a specified interaction in a pocket where a longer basic side chain packs poorly? A drawn structure is needed to specify the group’s exact connectivity. |
| 4-pyridylalanine (4-pyridyl analogue of phenylalanine) | Can the ring nitrogen at the para position form a hydrogen bond while the aromatic side chain preserves packing? |

For each proposed capability, choose a practical comparator and predict a measurable difference on a specified task. Treat formal charge, Brønsted basicity, and hard–soft acid–base (HSAB) classification as separate properties.

## 7. Deliverables

- **Alphabet definition.** Name the two deletions and provide structures and identifiers for the three additions.
- **Chemical rationale.** Explain the expected gains, routes to compensation, and anticipated liabilities.
- **Computational evaluation.** Provide reproducible inputs, code, predictions, and comparisons with the applicable baselines.
- **Failure analysis.** Identify tasks or environments where the alphabet is likely to underperform.
- **Validation proposal.** Specify a small set of experiments and controls that could test the main claims.

## 8. Intended Participants and Format

The challenge is intended for teams spanning protein design, experimental biology, chemistry, and machine learning. A 24-hour pilot would be more practical with a bounded candidate library, precomputed resources, and a starter workflow. The main challenge would leave teams room to propose their own structures and document how they evaluated them.

## 9. Open Design Questions

- Which protein tasks and measurements would make deletion costs and ncAA benefits visible?
- Which modeling methods can compare unfamiliar side chains with canonical residues, and how should their biases be checked?
- What evidence of synthesis or incorporation feasibility should be required for a computational entry?
- What shared experimental dataset or pilot would make the first comparisons credible?

## 10. Longer-Term Possibilities

Future versions could vary the deletion budget, compare alphabets of the same size, or explore changes to backbone chemistry.

An optional, longer version of the remove-two, add-three challenge could ask teams to propose a complete codon table after choosing their 21 amino acids. Teams could keep most existing assignments and allocate the freed codons to their three ncAAs, or redesign the table more broadly. If the two deletions free fewer than three codons, teams would need to free additional assignments. Teams would explain their choices and estimate how many codons they would need to change to encode a shared set of reference protein sequences compatible with their proposed alphabet. This computational extension would sit outside the v0.1 rules, with experimental validation of translation as a possible later step.

For a first pilot, what protein task would make it easiest to tell whether a new side chain restores a capability lost through deletion?
