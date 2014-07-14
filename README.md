## Checkmate

A faster and open source version of checkmate. Checkmate is a spatial and temporal dot crawl reducer originally written by prunedtree. It is most effective in static or low motion scenes.

### Usage
```
checkmate (clip, int "thr", int "max", int "tthr2")
```

* *thr* - spatial threshold. Controls the spatial filter, higher values will blend more but cause artifacts if set too high. If set too low, lines in static scenes where dot crawl was reduced will become slightly more blurry. **12** by default.

* *max* - controls the maximum amount by which a pixel's value may change. Higher values will increase the strength of the filtering but cause artifacts if set too high. **12** by default, any values between zero and 255 allowed.

* *tthr2* - temporal threshold. Controls the temporal blending; higher values will blend more but cause artifacts if set too high. Setting this to 0 disables the temporal blending entirely. This may be helpful to reduce temporal artifacts in high motion scenes. **0** by default, must be non-negative.
