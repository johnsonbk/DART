CHAMP
=====

This is just a modification of a standard "text" converter that comes with DART.

It reads CHAMP and GRACE text Density files (which used to be at
sisko.colorado.edu/sutton/data.html) and outputs DART obs_seq.out files.

Be aware that if obs_seq.out already exists, it automatically adds new
observations to that file without deleting it. This is done to allow
the wrapper script (work/convert.sh) to process sequentially numbered
Density_*.ascii files (read comments inside convert.sh).
If this is not the behavior you want, comment out lines 129-132 in
text_to_obs.f90 and rebuild.

Please check out work/input.nml:&text_to_obs_nml as it specifies the
name of the input and the output

The work/Density_3deg_02_335.ascii is truncated to 2 datapoints to
demonstrate the format and is not to be used for real experiments.

Author: Alexey Morozov

