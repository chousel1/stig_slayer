# STIG Surge

A standalone browser-based editor, comparison tool, and AI-assisted analysis platform for DISA STIG Checklist (`.cklb`) files.

> **Disclaimer**
>
> This tool was generated with the assistance of Artificial Intelligence and has not undergone formal security, compliance, or code-quality review. Organizations should review, test, and approve this tool according to their own policies and procedures before using it in any environment.

---

## Overview

STIG Surge is a client-side web application designed to simplify the management of DISA STIG Checklists (CKLB files). It allows analysts, system administrators, auditors, and compliance teams to view, edit, compare, and update STIG checklists without requiring installation of additional software.

The application runs entirely within a modern web browser and does not require a backend server for core functionality.

---

## Features

### CKLB Editing

* Open one or more CKLB files simultaneously
* Edit checklist metadata and target device information
* Modify:

  * Status
  * Comments
  * Finding Details
* Save individual checklists independently
* Save all loaded checklists

### Multi-Checklist Management

* Simulated tabs for multiple loaded CKLB files
* Switch between checklists without reloading
* Maintain separate edits for each checklist

### Bulk Editing

Perform bulk modifications across multiple CKLB files of the same STIG.

Bulk update:

* Status
* Comments
* Finding Details

Target specific controls using:

* Group ID
* Rule ID
* STIG Check Selection

### Advanced Filtering

Filter checks by:

* Rule ID
* Group ID
* Title
* Severity
* Status
* Discussion Text
* Check Content
* Fix Text
* Comments
* Finding Details
* CCI References
* Legacy IDs
* Presence/absence of comments
* Presence/absence of findings

Saved filters can be:

* Stored locally
* Exported
* Imported

### Compliance Comparison

Compare multiple CKLB files and identify:

* Status differences
* Finding differences
* Comment differences
* Compliance drift between systems

### STIG Version Update Helper

Compare different versions of the same STIG.

Features include:

* Identification of changed checks
* Revision comparison
* Highlighting of modified content
* Identification of newly added checks
* Identification of retired checks

Results are organized into collapsible sections:

* Changed Checks
* Changed Text
* New / Retired Checks

### AI Check Assistant (Optional)

An optional AI-assisted analysis feature is available.

Capabilities include:

* Ask questions about individual STIG checks
* Submit checks directly from the editor
* Upload reference documents
* Use local or cloud-hosted AI services

Supported endpoints include:

* Ollama
* LM Studio
* OpenAI-compatible APIs
* Custom OpenAI-compatible endpoints

#### AI Safety Notice

Before enabling AI functionality, users must acknowledge the following warning:

> STOP: Review your organization's policy for AI usage and disclosure of sensitive information before using this feature.

Organizations are responsible for ensuring that data sent to AI services complies with all applicable security, privacy, regulatory, contractual, and organizational requirements.

---

## Usage

### Loading Checklists

1. Open STIG Surge in your browser.
2. Select the desired workspace.
3. Load one or more `.cklb` files.
4. Begin editing, comparing, or analyzing.

### Saving Checklists

Use:

* Save Active
* Save Selected
* Save All

depending on your workflow.

### Comparing STIG Versions

1. Open the **STIG Version Update Helper**.
2. Select an older checklist version.
3. Select a newer checklist version.
4. Review changes and newly introduced controls.

### Using AI Features

1. Open the **AI Check Assistant** tab.
2. Enable AI functionality.
3. Acknowledge the warning message.
4. Configure the AI endpoint.
5. Upload reference documents if desired.
6. Send STIG checks for analysis.

---

## Security Considerations

This application is intended to operate entirely on the client side.

However:

* CKLB files may contain sensitive compliance information.
* AI integrations may transmit data outside of your environment.
* Local browser storage may be used for preferences and filters.

Users should:

* Review organizational policies before use.
* Verify AI usage is authorized.
* Validate all generated outputs.
* Review exported files before distribution.

---

## Limitations

* No warranty is provided.
* No guarantee of DISA compatibility for future CKLB formats.
* AI-generated responses may be inaccurate.
* Version-diff functionality depends on checklist structure consistency.

---

## Testing and Validation

Before operational use, organizations should:

* Perform code review
* Conduct security review
* Validate functionality against known CKLB files
* Verify checklist output integrity
* Validate AI integrations against approved services

---

## License

Use, modify, and distribute according to your organization's requirements and applicable licensing decisions.

---

## Acknowledgements

This project was generated with the assistance of Artificial Intelligence and refined through iterative development and testing. Human review is strongly recommended prior to deployment or operational use.
