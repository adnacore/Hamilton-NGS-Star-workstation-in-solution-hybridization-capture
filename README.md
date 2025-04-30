# Hamilton-NGS-Star-workstation-in-solution-hybridization-capture

## About

This repository contains the electronic protocol files for the automated hybridization capture of ancient DNA libraries on the Hamilton NGS Star in 96-well format using a capture method originally developed by Gnirke et al. 2009 and modified at the MPI-EVA for use with ancient DNA by Fu et al. 2013. Modifications to the latter method include the omission of a wash with Wash Buffer 3 and the hydroxide melt step for the elution of the captured library molecules prior to amplification. 

This repository also includes electronic protocol files for
+ preparation of the sample plate
+ qPCR quantification of capture yields

## Requirements

To use the protocol, a Hamilton NGS Star system with a custom deck layout is required. Calibration of the instrument for this protocol has to be performed by the user and requires significant expertise in using the platform.

## Implementation and Documentation

+ Use Hamilton Method Editor to import package file: method, device file, sub-methods, files and liquid classes.
(Import Mode: Recovery.)
+ liquid_classes_in_solution_capture.mdb can be used to overwrite existing liquid classes. (Should be imported by the Hamilton Method Editor while importing the pkg file.)
+ Supplementary protocols for qPCR setup (qPCR_setup.pkg) and sample plate preparation (sample_plate_preparation.pkg) can be imported the same way as in_solution_capture.pkg.
+ Lid for Trough_V1.0.zip needs to be installed prior to application. It is recommended to use trough lids but they are optional by setting a specific boolean in the methods.
+ MailAlert.zip can be installed to enable the system to send Mails for errors or other notifications.

## References

Fu, Q., Meyer, M., Gao, X., Stenzel, U., Burbano, H. A., Kelso, J., & Pääbo, S. (2013). DNA analysis of an early modern human from Tianyuan Cave, China. Proceedings of the National Academy of Sciences of the United States of America, 110, 2223-2227.

Gnirke, A., Melnikov, A., Maguire, J., Rogov, P., LeProust, E.M., Brockman, W., Fennell, T., Giannoukos, G., Fisher, S., Russ, C., Gabriel, S., Jaffe, D. B., Lander, E. S., Nusbaum, C. (2009) Solution hybrid selection with ultra-long oligonucleotides for massively parallel targeted sequencing. Nat Biotechnol. 27(2), 182-189

Zavala, E. I., Ayinuer-Petri, A., Richter, J., Nickel, B., Vernot, B., & Meyer, M. (2022). Quantifying and reducing cross‐contamination in single‐ and multiplex hybridization capture of ancient DNA. Molecular Ecology Resources, 22(6), 2196-2207.
