# Document Processing

> **NOTE:** This repository to use while drafting documentation and specifications before they are formally ratified.  Users should not begin implementing solutions based on the content in this repository as it is likely to change without notice.

This initiative gives distributors, carriers, and solution providers one standard, secure way to exchange imaged documents, such as applications, signed forms, disclosures, and signature summaries, through DTCC for annuity and life insurance business. It replaces manual and one-off document handling across pre-sale, new business, and post-issue servicing with a single digital process, improving speed, data consistency, and visibility into whether documents were received and accepted.

## API Specifications

The OpenAPI specification is in the [draft-api-specs](./draft-api-specs) directory.  

## Business Case

**Executive Summary:**
Provide the industry a standardized API, for exchanging unstructured data such as imaged documents, forms, and signatures alongside annuity and life insurance transactions. A sender submits up to 20 forms with one file per form (PDF or TIFF, up to 30MB combined) and receives an immediate acknowledgment; DTCC forwards the documents to the receiving firm and then sends a final notification back to the sender confirming whether the documents were processed successfully or rejected, with reasons.

**Problem:**
Today, supporting documents for annuity and life transactions are often exchanged through fax, email, portal uploads, or firm-specific integrations that vary by carrier and distributor. This creates delays, mismatched or missing paperwork, and little visibility into whether documents were received and accepted. This API closes that gap by defining one common format for submitting documents and their descriptive details, tied to the originating transaction, with a consistent confirmation and error response so senders know the outcome without follow-up calls.

**Objective:** Create a standard, asynchronous document exchange API that lets any participant securely send documents tied to a transaction and receive a clear, final confirmation of the outcome.

**Key Results:**
· Reduction in documents sent through fax, email, and manual upload
· Reduction in not-in-good-order (NIGO) cases caused by missing or mismatched documents
· Volume of participant adoption
· Reduction in follow-up calls to confirm document receipt

**Use Case 1:** Submit the application, disclosures, and signature summary with a new business case (DTCC APP file)

**Use Case 2:** Submit replacement forms and supporting paperwork with a replacement (1035 exchange / transfer) submission

**Use Case 3:** Submit service forms for post-issue requests such as address changes, party updates, withdrawals, and producer changes

**User Story 1:** As a distributor, I want to send the documents for a transaction in a standard format so that the carrier receives everything it needs without manual handling.

**User Story 2:** As a carrier, I want each document to arrive with consistent descriptive details (form type, policy number, owner, signatures) so that I can match it to the right case and process it quickly.

**User Story 3:** As a sender, I want a final confirmation of success or failure, with specific reasons when rejected, so that I can resolve issues without follow-up calls.

## Business Owners 
- **DTCC:** Jeanann Smith

## How to engage, contribute, and give feedback
Please contact the business owners or IRI (hpikus@irionline.org) and Matt Hendrickson (mhendrickson@irionline.org) at IRI to get added to the working group discussions.

## Change submissions and reporting issues and bugs

Security issues and bugs should be reported directly to Hannah Pikus at hpikus@irionline.org and Matthew Hendrickson at mhendrickson@irionline.org. Issues and bugs can be reported directly within the issues tab of a repository. Change requests should follow the standards governance workflow outlined on the main page.

## Code of conduct

See the [Digital-First-Specifications](https://github.com/Insured-Retirement-Institute/Digital-First-Specifications) repository

