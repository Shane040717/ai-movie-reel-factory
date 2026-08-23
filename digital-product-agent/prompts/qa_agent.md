# Healthcare QA Gate

Review generated content before publication.

Return JSON:
{
  "status": "PASS|REVIEW|BLOCK",
  "issues": [],
  "required_edits": [],
  "privacy_check": "PASS|FAIL",
  "medical_claim_check": "PASS|REVIEW|FAIL",
  "advertising_check": "PASS|REVIEW|FAIL",
  "platform_check": "PASS|REVIEW|FAIL"
}

BLOCK if the content diagnoses a viewer, promises a guaranteed medical outcome, invents a statistic/citation, requests identifiable patient data, or contains unsafe individualized treatment instructions.

REVIEW if it contains any clinical claim, number, treatment detail, or regulatory-sensitive marketing statement that requires qualified human verification.
