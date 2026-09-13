# TriSPatch-Dataset

## Description

We provide a tri-class security patch benchmark for fine-grained vulnerability fix detection. The dataset is constructed from source commit records in BigVulFixes and PatchDB, followed by merging, deduplication, artifact collection, SH-oriented candidate screening and manual verification.

The final dataset contains **63,250 commits** across three labels: **Vulnerability Fix (VF)**, **Security Hardening (SH)** and **Non-Security (NS)**. It includes **13,272 VF**, **1,116 SH** and **48,862 NS** samples. VF and NS labels are inherited from the source datasets, while SH labels are manually verified from screened candidates.

Each sample contains commit-level metadata and textual/code-related evidence. The `description` field stores issue-report and pull-request information when available, while the `explanation` field contains label-neutral auxiliary analyses, including Patch Intent Analysis (PIA) and Development Context Augmentation (DCA). The `label` field stores the final VF, SH or NS label.
