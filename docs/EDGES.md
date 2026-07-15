# 17 Edge Cases Explored (U13 11v11)
1. Fisheye calibration drift/mount shift → Interactive wizard + saved JSON + error alert.
2. Sparse/blurred pitch lines → Roboflow keypoints fallback + manual points + validation.
3. Low-light/shadows → Confidence filter + CLAHE preprocess + tunable thresh.
4. Heavy player clustering/occlusions → OC-SORT + torso color ReID + interp.
5. Tiny/fast ball lost → Dedicated ball track + trajectory smoothing.
6. ID switches (subs/re-entry) → Log stats + manual edit in report.
7. Similar youth kits/glare → Masked torso + cluster validation + alert.
8. Refs/ballboys false pos → Class-specific confidence + size filter.
9. Far-side ~30px resolution → Tiled inference + high-res input.
10. Non-flat/uneven youth pitch → Homography + Kalman smoothing.
11. Erratic U13 motion → OC-SORT + RTS trajectory.
12. 90min 4K upload bandwidth → Chunked web endpoint + resume.
13. Modal cost/time spikes → 10fps sample + batch GPU + queue.
14. No jersey numbers → Color + position proxy only.
15. Evening variable light → Auto exposure detect + model robust.
16. Camera overheating (iPhone) → Chunk upload design.
17. Homography error accumulation → Per-segment reset + baseline check.

All mitigated in code.