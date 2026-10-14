# TD_pop_convert1
pop_convert1 has 9 buttons. Analyze found 41 swappable SOPs. Convert builds a POP copy at /project1/pop_optimized. Bridges adds TOP-POP links. Copy Path copies paths. Profile lists top 30 cooks. Viewers Off, Cache Static, and Readback optimize the original network. Restore undoes those edits, keeping Convert.

All nine buttons on pop_convert1 are wired to real functions. Analyze and Profile were just run against /project1. Convert is the one that builds the POP copy. The others either write a report or edit the original network, and Restore only undoes those edits.

Analyze writes a report and changes nothing. On the current project it found 41 SOPs in TENTACLES_WOWWW that Convert can swap, 10 image-chain TOPs to leave alone, and nothing that needs a manual POP rebuild or a point-data bridge.

Convert clones each SOP network into /project1/pop_optimized, keeps the camera, lights, materials, TOPs, and CHOPs, and swaps the SOPs for POPs on the same wires. The original stays. Status goes Processing, then Ready, and the destination path is copied to the clipboard. This is the button that makes the POP scene.

Bridges adds a TOP-to-POP only for a TOP that feeds a toptoCHOP and does not feed another TOP. This project has none of those. The ramps, noises, lookup, and render are an image chain, so Bridges has nothing to add.

Copy Path copies the Destination parameter to the clipboard. It is already /project1/pop_optimized. It does not build anything.

Profile lists the 30 operators with the highest last cook time. It does not change resolution or the network. The list it just wrote is mostly panel text, because that is what had cooked most recently.

Viewers Off turns off SOP, TOP, and POP node viewers under the target so those viewers stop cooking. The rendered output stays as it is. It edits the original network. The pop_optimized copy is skipped.

Cache Static inserts a one-frame cache after a TOP or POP that is not animated. Noise, movies, feedback, and the render are skipped, and the resolution stays on the input. Restore removes those caches. It also edits the original network, not the copy.

Readback turns off POP "copy topology back to CPU" toggles and lists any soptoCHOP, poptoCHOP, or poptoDAT without removing them. The POP copy is skipped, so on the original SOP show this mostly finds nothing to turn off.

Restore turns those viewers back on, puts the readback toggles back, and deletes the caches this operator added. It does not undo Convert. The original component is still the untouched show.
