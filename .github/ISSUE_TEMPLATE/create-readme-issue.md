---
name: "README for OctoAcme Project Management Docs with Links and Summary"
description: "Create a README file as a central hub for all OctoAcme project management process documentation with links and summary"
title: "[Process Doc Update]: README - Project Management Processes Summary and Doc Links"
labels: ["documentation", "process improvement"]
body:
  - type: dropdown
    id: process_doc
    attributes:
      label: "Which process document do you want to update?"
      description: "Select the program management process document you want to add content to."
      options:
        - "<new document>"
        - octoacme-project-management-overview.md
        - octoacme-project-initiation.md
        - octoacme-project-planning.md
        - octoacme-execution-and-tracking.md
        - octoacme-risks-and-communication.md
        - octoacme-release-and-deployment.md
        - octoacme-retrospective-and-continuous-improvement.md
        - octoacme-roles-and-personas.md

  - type: textarea
    id: content_summary
    attributes:
      label: "Summary of New Content"
      description: "Briefly describe the new content or update you want to add."
      value: "Create a comprehensive README.md file for the OctoAcme Project Management Docs that serves as a central hub. The README should include: (1) A brief summary of the project management processes used by OctoAcme; (2) Organized links to all process documentation files in the docs/ folder; (3) Quick navigation guide for team members to find relevant processes; (4) Introduction to key roles and personas; (5) Overview of the project lifecycle from initiation through retrospective."
    validations:
      required: true

  - type: textarea
    id: rationale
    attributes:
      label: "Why is this update needed?"
      description: "Explain the reason for this addition."
      value: "This README will provide a single entry point for all team members to understand OctoAcme's project management approach. It will improve discoverability of process documentation, accelerate onboarding, reduce single-person dependency risk, and establish a clear structure for navigating the various process guides. This aligns with the purpose of centralizing scattered project management knowledge and making it easily accessible to all team members."
    validations:
      required: true

  - type: textarea
    id: example_content
    attributes:
      label: "Suggested Content (optional)"
      description: "Paste the proposed new text, checklist, diagram, or example content you'd like to add."
      value: |
        # OctoAcme Project Management Documentation

        Welcome to the OctoAcme Project Management Docs hub. This directory centralizes all processes, templates, and guidance needed to successfully deliver projects at OctoAcme.

        ## Quick Start
        - New to OctoAcme? Start with [Project Management Overview](octoacme-project-management-overview.md)
        - Starting a new project? Follow the [Project Initiation Guide](octoacme-project-initiation.md)
        - Need to plan a project? See [Project Planning](octoacme-project-planning.md)
        - Managing daily delivery? Check [Execution & Tracking](octoacme-execution-and-tracking.md)
        - Handling risks and communication? Review [Risk Management & Communication](octoacme-risks-and-communication.md)
        - Preparing for release? Follow [Release & Deployment Guide](octoacme-release-and-deployment.md)
        - Capturing learnings? Use [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
        - Understanding team roles? See [Roles and Personas](octoacme-roles-and-personas.md)

        ## OctoAcme Project Management Overview
        OctoAcme follows an iterative, customer-focused project management approach built on five core principles:
        - **Customer-first**: Prioritize customer value and usability in all decisions
        - **Iterative delivery**: Deliver small, testable increments with regular feedback
        - **Clear ownership**: Each project has a named Project Manager (PM) and Product Lead
        - **Data-informed decisions**: Measure impact and iterate based on evidence
        - **Psychological safety**: Encourage feedback, learning, and continuous improvement

        ## Project Lifecycle
        Every OctoAcme project follows this five-phase lifecycle:
        1. **Initiation**: Define the problem, align stakeholders, validate business need
        2. **Planning**: Create actionable backlog, identify dependencies, set milestones
        3. **Execution**: Build, test, iterate, and track progress
        4. **Release**: Deploy to production and verify success
        5. **Retrospective**: Capture learnings and drive continuous improvement

        ## Key Roles
        - **Project Manager (PM)**: Coordinates delivery, manages schedules, risks, and communications
        - **Product Manager (PdM)**: Defines outcomes, prioritizes backlog, measures success
        - **Developers**: Implement features, collaborate on design and testability
        - **QA/Testing**: Validate quality and acceptance criteria
        - **Stakeholders**: Provide inputs and approvals

        ## Communication Cadence
        - Weekly sync between PM + Product Manager
        - Twice-weekly standups for delivery team
        - Monthly stakeholder updates
        - Ad-hoc escalations as needed

    validations:
      required: false

  - type: checkboxes
    id: acceptance_criteria
    attributes:
      label: "Acceptance Criteria"
      description: "Check all that apply:"
      options:
        - label: "Content aligns with existing process docs"
        - label: "Update improves clarity or closes a documented gap"
        - label: "Proposed content has been reviewed with stakeholders (if needed)"
