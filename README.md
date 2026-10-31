# Manufacturing workflow catalog: inputs, candidate outputs and human review

Public reference data from Pin2pin. [View the 68-scenario CSV](./manufacturing-workflow-catalog.csv).

## 中文说明

这份表按8个部门整理68条工业AI工作场景，用于说明已有输入资料、期望输出和人员复核责任。CSV保留中文场景名称与示例，供企业需求讨论和资料查阅。公开来源：[案芯智能场景说明](https://pin2pin.cc/scenes/)与[工作方法](https://pin2pin.cc/guides/)。

## Purpose and sources

Pin2pin's public requirements catalog lists 68 work scenarios across eight departments. The input/output CSV in this repository helps a team describe one task: which materials are available, what someone needs to prepare and who must review the result.

The entries describe work scenarios and candidate outputs. They do not establish 68 delivered projects, measured performance or product availability. This material is a planning reference; it does not process files or provide an online AI conversion service.

Public references:

- [Application descriptions](https://pin2pin.cc/scenes/): inputs, outputs and review responsibilities for selected workflows.
- [Practical guides](https://pin2pin.cc/guides/): drawing OCR and editable CAD, BOM review, and equipment tuning data.
- [Requirements catalog](https://pin2pin.cc/estimate/): the source of the department groups and scenario entries.

The source pages and catalog are currently in Chinese. The department labels and examples below are English summaries. Catalog reference date: 31 October 2026.

## Department coverage

The counts cover all catalog entries. Each row gives one representative task, identified by its original scenario ID. The listed outputs are candidates to define and review for a particular task.

| Department | Entries | Example ID | Example inputs | Candidate outputs |
| --- | ---: | --- | --- | --- |
| Sales and commercial | 11 | A3 | RFQ drawings, historical project data, material and labor baselines | Cost item list, costing suggestions, draft quotation |
| Research and design | 19 | C4 | 2D drawings, 3D models | Draft BOM, source references for item identifiers |
| Process and manufacturing engineering (NPI) | 10 | E1 | Drawings, BOM, equipment list | Draft process routing, process flow diagram |
| Quality | 9 | D2 | 2D drawings, inspection standards or specifications | Draft inspection plan, inspection worksheet |
| Purchasing and supplier management | 7 | F1 | Supplier emails and replies, purchase orders, delivery records | Delivery commitment cards, delivery status overview, material shortage alerts |
| Production planning and material control (PMC) | 5 | F2 | ERP BOM exports, inventory records, purchase orders for incoming materials | Material readiness report, shortage list, estimated date when required materials will be available |
| Equipment and maintenance | 4 | G1 | Equipment process curves, operating condition records, changeover parameters | Parameter suggestions, preliminary pass/fail assessment, anomaly alerts |
| Business management | 3 | H1 | Emails, operating data, market information | Draft management briefing, exception flags |

## Organize a task request

1. Choose one scenario and retain its ID. Describe who handles the task today and what triggers it. Keep requests for different scenarios separate.
2. List the available inputs, including file formats, revisions, units and missing information. For an initial discussion, use generic descriptions or a redacted sample.
3. Define the required output. Name the worksheet, comparison, drawing draft or issue list, and identify the fields that must point back to a source.
4. Name the reviewer and the checks needed before anyone uses the output. Agree on how to record corrections and unresolved items.

For example, a request for C4 could specify drawing revisions, the assembly scope, a BOM template and the engineer responsible for checking quantities and full part numbers. Keep unknown fields visible instead of filling them from assumptions.

## Review before use

Keep the original information, prepared values and human corrections distinguishable. Preserve source locations and revision references so a reviewer can check each item.

- For drawing OCR or editable CAD, inspect actual objects, dimensions, units and tolerances. Image scale alone does not establish geometry accuracy.
- For a BOM, check quantity basis, complete model identifiers, missing items and substitution approvals before purchasing approval.
- For inspection preparation, confirm the extracted requirements. Measurements, acceptance decisions and report release remain with the responsible personnel.
- For delivery and planning records, verify supplier statements, dates, quantities and partial shipments. Treat predicted dates as estimates pending review.
- For equipment work, link complete curves to operating conditions, approved parameters and individual quality results. Parameter changes and trials require human approval under existing site procedures.

## Keep customer material separate

This README contains generic input/output descriptions, with no customer drawings, actual part dimensions, supplier identities, prices or production records. Before sharing any example, remove customer identifiers and confidential business content. Keep original customer material in the agreed project environment.
