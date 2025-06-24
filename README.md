# Phishing Email Analysis

This repository contains an analysis of a suspected phishing email, identifying various indicators that suggest it is a malicious attempt. The analysis was conducted using an online EML Analyzer tool and focuses on identifying common phishing traits within email headers, sender information, and embedded content.

## Objective

The primary objective of this analysis was to:
1.  Obtain a sample phishing email (simulated by provided screenshots).
2.  Examine the sender's email address for spoofing.
3.  Check email headers for discrepancies using an online header analyzer.
4.  Identify suspicious links or attachments.
5.  Look for urgent or threatening language in the email subject.
6.  Note any mismatched URLs (though direct hovering wasn't possible, extracted URLs were examined).
7.  Summarize the phishing traits found in the email.

## Tools Used

* EML Analyzer: Used to parse and display detailed email headers and identify potential indicators.
* Manual Inspection: For reviewing subject lines, 'From' addresses, and interpreting analyzer outputs.

## How the Analysis Was Performed

1.  Email Header Upload: The EML content (or in this case, its analysis via screenshots) was fed into the EML Analyzer tool.
2.  Basic Headers Review: The 'From', 'To', 'Subject', and 'Date' fields were initially examined.
3.  Authentication Results Check: SPF, DKIM, and DMARC results were scrutinized for failures or `none` statuses, which often indicate spoofing.
4.  Hops Analysis: The path the email took through various servers was traced to identify the true origin and any unusual routing.
5.  Spam Scores: Scores from SpamAssassin and SCL (Spam Confidence Level) were noted as general indicators of email legitimacy.
6.  Extracted Content: URLs and email addresses extracted by the analyzer were carefully reviewed for suspicious domains or patterns.
7.  Phishing Indicators Identification: Each piece of information gathered was cross-referenced with common phishing characteristics to build the `analysis-report.md`.
