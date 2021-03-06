# Amber toolchain test

The molecule in the trifold*.mol2 files is a 35 Angstrom long bundle of three greasy spiroligomers that could be dropped into a membrane to simulate its dynamics.

The goal of this design is to exploit symmetry to create something that is easier to synthesize.  This structure consists of just three spiroligomers and has 3-fold symmetry.

It was built using the Cando chemistry language that I've been working on for the past decade.  The Cando source file builds the three-dimensional structure from a Chemdraw structure.

### Files...

1. trimemwide.mol2 - The close-packed array generated by wb-trimemwide.lisp
1. trimemwide-short.mol2 - The close packed array generated by wb-trimemwide-carbonyl.lisp with short atom names
1. trimemwide-carbonyl.mol2 - The close packed array of channels with carbonyls adjusted to look like Aquaporin
1. trimemwide-water-carbonyl.mol2 - Array of channels, carbonyl charges adjusted, with water.
1. trimemwide-water-carbonyl.prmtop - AMBER prmtop file for trimemwide-water-carbonyl.mol2
1. trimemwide-water-carbonyl.inpcrd - AMBER inpcrd file for trimemwide-water-carbonyl.mol2
1. wb-trimemwide-carbonyl.lisp - Cando code that creates a close packed p3 lattice of 9 bundles. Unit cell length is 14.5 Angstroms
1. waterBox-original.* - Original waterBox files.
1. trimemwide-gas.ac - Raw, unadjusted Gasteiger charges calculated by Antechamber in Antechamber format file.
1. aquaporin_carbonyls.xy - Carbonyl carbon charge, oxygen charge x/y pairs extracted from 1j4n.psf
1. gasteiger_carbonyls.xy - Carbonyl carbon charge, oxygen charge x/y pairs extracted from trimemwide-gas.ac

