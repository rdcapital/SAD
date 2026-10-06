# Patient Care User Stories

## User Story 1: Schedule Appointment

**As a patient, I want to schedule an available appointment with a
healthcare provider so that I can receive medical care at a convenient time.**

### Acceptance Criteria

#### Scenario: Patient schedules an available appointment

- **Given** the patient is registered in the healthcare portal
- **And** the healthcare provider has an available appointment slot
- **When** the patient selects the provider and available time
- **And** confirms the appointment
- **Then** the system should create the appointment
- **And** display a confirmation message to the patient
- **And** show the appointment in the patient's appointment list


## User Story 2: Reschedule Appointment

**As a patient, I want to reschedule my existing appointment so that I can
change my appointment time when my schedule changes.**

### Acceptance Criteria

#### Scenario: Patient reschedules an appointment

- **Given** a patient has a scheduled appointment
- **And** the appointment is less than 24 hours away
- **When** the patient requests to reschedule the appointment
- **Then** the system should apply a late-change flag
- **And** emit an "AppointmentRescheduled" event
- **And** display the updated appointment details