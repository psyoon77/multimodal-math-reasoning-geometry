<div align="center">

# 💠 Multimodal Math Reasoning: Geometry 💠

### Diagram-Grounded Mathematical Reasoning Research Archive

<p>
  <img alt="Project status: research archive" src="https://img.shields.io/badge/status-research%20archive-6f42c1">
  <img alt="Release: summary only" src="https://img.shields.io/badge/release-summary%20only-0A7BBC">
  <img alt="Implementation: not distributed" src="https://img.shields.io/badge/implementation-not%20distributed-lightgrey">
  <img alt="Claims: qualitative" src="https://img.shields.io/badge/claims-qualitative-informational">
</p>

<p>
  <a href="#-research-question">Research question</a> •
  <a href="#-overview">Overview</a> •
  <a href="#-research">Research</a> •
  <a href="#-visual-input-ablations">Ablations</a> •
  <a href="#-historical-findings">Findings</a> •
  <a href="#-public-release-boundary">Release boundary</a> •
  <a href="#-references">References</a>
</p>

</div>

This repository includes just the skeleton of the prior work.

## 🔬 Research question

How should multimodal systems be evaluated on geometry problems that combine
diagrammatic and written information?

This research investigated this question through prototype development, controlled
experimentation, and analysis of model behavior. This public archive preserves
the research context without disclosing the implementation or method-sensitive
details reserved for future work.

## 📋 Overview

| Area | Status | Public interpretation |
| --- | --- | --- |
| Research framing | ✅ Preserved | Diagram-and-text geometry reasoning study |
| Prototype development | ✅ Completed | Experimental systems were implemented and evaluated |
| Comparative analysis | ✅ Completed | Multiple prototype configurations were examined |
| Sensitivity analysis | ✅ Completed | Visual-input ablations examined changes in model behavior |
| Detailed methodology | 🔒 Not distributed | Architecture, procedures, and configurations remain private |
| Dataset and artifacts | 🔒 Not distributed | Data, outputs, logs, and checkpoints are excluded |
| Historical measurements | 📝 Reported | Aggregate top-10 values are preserved with a reproduction caveat |

## ✒ Research

| Research activity | Scope of the work |
| --- | --- |
| Experimental design | Defined comparisons for geometry problems containing visual and textual information |
| Prototype engineering | Built research pipelines for multimodal experimentation |
| Evaluation | Examined model behavior across controlled experimental conditions |
| Behavioral analysis | Compared aggregate results with visual-input sensitivity evidence |
| Research synthesis | Documented limitations and directions requiring further study |

These statements describe project-level activities without claiming ownership
of the cited benchmarks or prior research. The corresponding attribution and
claim boundary is documented in [CONTRIBUTIONS.md](CONTRIBUTIONS.md).

## 🧪 Visual-input ablations

The study compared model behavior under concrete counterfactual image
conditions while keeping the geometry task itself fixed:

| Input condition | Example | Evaluation purpose |
| --- | --- | --- |
| Original diagram | The ordinary geometry diagram paired with its written problem | Establish the reference condition |
| Uniform blank control | The diagram is replaced by a blank, all-zero image | Measure behavior when visible geometry is absent |
| Random-noise control | The diagram is replaced by randomized pixel noise | Measure sensitivity to non-semantic visual input |
| Label perturbation | Diagram labels are altered or omitted | Examine dependence on visual symbols and their correspondence to the text |

The original, blank, and random-noise conditions were represented directly in
the experimental pipeline. Altered and omitted labels were documented as an
additional counterfactual study design. Exact images, procedures, per-example
outputs, and detailed measurements remain outside this public archive.

## 📊 Historical findings

The original report recorded the following top-10 accuracy values:

| Geometric Math | This Model | Published Benchmark |
| --- | ---: | ---: |
| Proving | 94.9% | 56.4% |
| Calculation | 62.7% | 62.5% |

These aggregate values are transcribed from the historical project report. The
public archive does not include the raw predictions, evaluation implementation,
or experiment artifacts required to reproduce them independently. They should
be read as archived results rather than a current leaderboard claim.

The historical results suggested limited sensitivity when original diagrams
were replaced with a uniform blank control. Random-noise and label-perturbation
conditions broadened the evaluation design and motivated closer study of how
visual information contributes to the final response. Aggregate performance
and visual-input sensitivity therefore provide complementary views of model
behavior.

The earlier works established the datasets, task formulations, and baselines
that made this study possible. The ablations build on that foundation by
adding a narrower, complementary view of input sensitivity.

Detailed measurements, per-example comparisons, procedures, and interpretation
artifacts are not included because the supporting implementation, data, and
evaluation materials are outside this public archive.

## 🔒 Public release boundary

| Included | Not distributed |
| --- | --- |
| Research question and project context | Source code and executable notebooks |
| High-level categories of work | Architecture and implementation details |
| Ablation conditions, qualitative observation, and aggregate historical results | Exact prompts, procedures, and configurations |
| Primary research references | Datasets, samples, and answer material |
| Explicit limitations and attribution | Checkpoints, outputs, logs, and private reports |

This is a project summary—not a reproduction package, software release, or
disclosure of ongoing methods. See [NOTICE.md](NOTICE.md) for the formal release
scope.

## 🧭 Limitations and next steps

- The public archive cannot independently reproduce the historical study.
- The two aggregate accuracy comparisons are historical reported values and
  have not been independently reproduced in this archive.
- The qualitative observation should not be interpreted as a benchmark or
  current performance claim.
- Any future technical release would require a separate provenance, licensing,
  and reproducibility review.

## 📚 References

The geometry-reasoning benchmarks and related methods that frame this archive
are credited in [REFERENCES.md](REFERENCES.md). No external code, dataset, or
model artifact is redistributed here. Reusable citation records are provided
in [CITATIONS.bib](CITATIONS.bib).

## 📄 Availability

This summary is publicly viewable, but the underlying implementation and
research artifacts are not distributed. No open-source software license is
provided because this archive contains no software.

---

<div align="center">
  <sub>Preserved as an honest, limited record of exploratory multimodal reasoning research.</sub>
</div>
