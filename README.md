# Employee Raise Issue - Record Producer Service Portal Integration

A ServiceNow project that lets employees raise issues directly from the **Service Portal** using a **Record Producer**, which creates records in the backend table and routes them for resolution.

## Overview

- **Employee**: Opens the Service Portal and fills out an "Raise Issue" form.
- **Record Producer**: Captures the submitted form data and creates a record (e.g., an Incident / Case) automatically.
- **Integration**: The record producer maps form fields to the target table and triggers any required workflows/notifications.

## Features

- Self-service issue submission through the Service Portal
- Guided form (Record Producer) with validation
- Automatic record creation and assignment
- Email/workflow notifications on submission

## Tech Stack

- ServiceNow (Washington / Vancouver / Utah release)
- Service Portal (Widgets, Pages)
- Record Producer + Catalog Item
- Business Rules / Flow Designer for automation

## File Structure

```
Employee-Raise-Issue-Record-Producer-Service-Portal-Integration/
├── README.md
├── record_producer/      # Record producer and catalog item config
├── service_portal/       # Service Portal widget / page
├── scripts/              # Business rules, script includes, flows
└── update_sets/          # Exported update set XML (if any)
```

## Setup / Installation

1. Import the update set (if provided under `update_sets/`) into your ServiceNow instance.
2. Preview and commit the update set.
3. Open the Service Portal and navigate to the **Raise Issue** catalog item.
4. Submit the form and verify that a record is created in the target table.

## Usage

1. Log in to the Service Portal as an employee.
2. Go to the **Raise an Issue** form.
3. Fill in the issue details and submit.
4. Track the status from the portal / record list.

## Contributing

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes and open a pull request.

## License

This project is provided as-is for learning/demo purposes.
