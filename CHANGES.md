0.2.0 (dev)
===========
+ **2X speed improvement for CRAM** by not decoding unused base-qualities.
+ when using quantize, labels now indicate the range of depths encompassed by that region.
+ for quantize and per-base, mosdepth will output all chromosomes in the bam header, even if they have no alignments.
  this makes it so that mosdepth output for files aligned to the same reference have the same number and order of chromosomes
  and same total base coverage
+ add new `--thresholds` argument. See README for usage. thresholds and quantization are highly recommended over
  per-base output when possible as they are more compact and faster to output.
