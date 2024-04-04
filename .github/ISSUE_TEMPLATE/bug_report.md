name: Bug Report
description: File a bug report
title: "[Bug]: "
labels: ["bug", "triage"]
assignees:
  - vincekruger
body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to fill out this bug report!
  - type: textarea
    id: what-happened
    validations:
      required: true
    attributes:
      label: What happened?
      description: Describe the bug in a bit of detail.
      placeholder: Tell us what you see!
      value: "A bug happened!"
  - type: textarea
    id: expected-behaviour
    validations:
      required: true
    attributes:
      label: What was supposed to happen?
      description: A clear and concise description of what you expected to happen.
      placeholder: What did you expect?
      value: "It's supposed to work man!"    
  - type: textarea
    id: reproduction-steps
    validations:
      required: true
    attributes:
      label: Steps to Reproduce the Behaviour
      description: The more detail the better
      value: |
        1. Go to '...'
        2. Click on '....'
        3. Scroll down to '....'
        4. See the error"
        ...
  - type: textarea
    id: screenshots-videos
    validations:
      required: true
    attributes:
      label: Screenshots/Videos? 🙏🫶
      description: It really helps to see the issue too
  - type: dropdown
    id: version
    validations:
      required: true
    attributes:
      label: App Version
      description: What version of our software are you running?
      options:
        - 2024.0.0 (Default)
      default: 0
  - type: input
    id: build-number
    validations:
      required: true
    attributes:
      label: Build#
      value: "🤷‍♂️"
  - type: dropdown
    id: device
    validations:
      required: true
    attributes:
      label: What software are you using?
      multiple: false
      options:
        - iOS
        - iPadOS
        - Android
        - Something else
  - type: input
    id: os-version
    validations:
      required: true
    attributes:
      label: OS Version
      placeholder: "iOS 17.4.1"
  - type: input
    id: phone
    validations:
      required: true
    attributes:
      label: What Phone are you using?
      description: "iPhone 15 Pro, Samsung A35, etc."
