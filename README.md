# Canvas-Samples
This repository includes the Canvas samples used in the research "Canvas Fingerprinting: A State of the Art". This research studied the effectiveness of each sample in fingerprinting web users.

Each file in the this repository includes the source code used in drawing a Canvas sample with the corresponding number in the research. 


The following two lines of code are included in each sample's file, assuming that there are form hidden input fields with the names "DataURLX" and "HashX", where X is the sample number. These lines retrieve the Canvas DataURL and hash value (only hash is necessary) to be submitted to the website owner:


document.getElementById("DataURLX").value = "" + dataURL;

document.getElementById("HashX").value = "" + dataURL.hashCode();
