name: General issue
description: For any issues
labels: []
assignees: []

body:
  - type: markdown
    attributes:
      value: |
        ## **Description**

  - type: textarea
    id: description
    attributes:
      label: What is this about?
      placeholder: As a user, describe the issue here.
    validations:
      required: true

  - type: markdown
    attributes:
      value: |
        ## **Scenario (for user stories only)**

  - type: textarea
    id: scenario
    attributes:
      label: Scenario
      placeholder: |
        - GIVEN a user is in x state
        - WHEN a user does x
        - AND a user does x
        - THEN x should occur

  - type: markdown
    attributes:
      value: |
        ## **Design (for user stories only)**

  - type: textarea
    id: design
    attributes:
      label: Design
      placeholder: If available, provide a link to the design (e.g., Figma) or screenshots. If you're an external contributor and don't have access to the design, feel free to skip this step or provide any visual representation of the issue if possible.

  - type: markdown
    attributes:
      value: |
        ## **Technical Details (for technical tasks only)**

  - type: textarea
    id: technical-details
    attributes:
      label: Technical Details
      placeholder: |
        - Implementation details
        - Insight to what needs to be done
        - Etc.

  - type: markdown
    attributes:
      value: |
        ## **[Threat Modeling Framework](https://github.com/adamshostack/4QuestionFrame) (for technical tasks only)**

  - type: textarea
    id: threat-modeling
    attributes:
      label: Threat Modeling Framework
      placeholder: |
        - What are we working on? What does this aim to solve?
        - What can go wrong?
        - What are we going to do about it?
        - Did we do a good job?

  - type: markdown
    attributes:
      value: |
        ## **Acceptance Criteria**

  - type: textarea
    id: acceptance-criteria
    attributes:
      label: Acceptance Criteria
      placeholder: |
        - Are metrics required?
        - Are translations required?
        - Cases to satisfy
        - XYZ should work
        - Etc.

  - type: markdown
    attributes:
      value: |
        ## **Stakeholder Review **

  - type: checkboxes
    id: stakeholder-review
    attributes:
      label: Stakeholder review needed before the work gets merged
      options:
        - label: Engineering (needed in most cases)
        - label: Design
        - label: Product
        - label: QA (automation tests are required to pass before merging PRs but not all changes are covered by automation tests - please review if QA is needed beyond automation tests)
        - label: Security
        - label: Legal
        - label: Marketing
        - label: Management (please specify)
        - label: Other (please specify)

  - type: markdown
    attributes:
      value: |
        ## **References**

  - type: textarea
    id: references
    attributes:
      label: References
      placeholder: |
        - References go here.
        - Screenshots.
        - Issue numbers. Links.
        - Slack threads.
        - Etc.