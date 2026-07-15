## CoachFlow v2 - Comprehensive Research & Decisions (U13 11v11, Fixed Wide Camera)

### 1. Tool Verification (July 15 2026)
**YOLO26**: ... (detailed)
**SAM 3.1**: Multiplexing confirmed viable but expensive → **Decision**: OC-SORT primary, SAM for validation frames.
**RF-DETR**: Superior small object mAP.
**Modal**: Confirmed patterns.

### 2. Edge Cases & Kinks (Detailed)
- **Calibration**: Mount shift, line fade, non-flat pitch → Interactive + auto-refine + saved profile + error metrics.
- **Detection**: Far-side 25px players, ball in cluster, refs/ballboys → Tiling + class-specific thresholds + Roboflow soccer model.
... (full 15+ kinks)

### 3. Architecture Choices
- Fresh repo, clean.
- Chunking: 300-frame segments.

All documented for robustness.