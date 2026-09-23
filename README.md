# MediKiosk AI

### AI-Powered Clinical History Taking & OPD Workflow Assistance

MediKiosk AI is a prototype designed to capture a patient's clinical history and prior medical information before consultation, helping make OPD visits more structured and efficient.

The system guides patients through an adaptive history-taking workflow and presents the collected information in a structured format for the doctor.

---

## 🚀 Live Prototype

**[Open MediKiosk AI →](https://jaideep-raj-cse.github.io/Medikiosk-AI/)**

**[View Source Code →](https://github.com/jaideep-raj-cse/Medikiosk-AI)**

---

## 🎯 Problem

In many OPD environments, a significant portion of consultation time can be spent collecting and documenting basic patient history.

Patients may also have previous medical documents, investigations, prescriptions, and other information that needs to be reviewed before or during consultation.

MediKiosk AI explores a digital pre-consultation workflow in which patient information can be collected and structured before the doctor begins the consultation.

---

## 💡 Our Solution

MediKiosk AI provides a guided digital workflow for collecting patient information before consultation.

The prototype:

- Collects the patient's basic information
- Identifies the patient's chief complaint
- Uses complaint-specific questions
- Collects relevant medical history
- Captures drug and allergy history
- Collects family and personal history
- Performs review-of-systems questioning
- Includes an AYUSH assessment workflow
- Processes prior medical-document information in the prototype
- Applies clinical red-flag rules
- Generates a structured clinical summary
- Provides a doctor-facing workflow for reviewing the collected information

---

## ✨ Key Features

### 1. Adaptive Clinical History Taking

The prototype provides different questions depending on the patient's chief complaint.

Supported complaint categories include:

- Chest pain
- Breathlessness
- Abdominal pain
- Headache
- Fever
- Cough / Cold
- Joint / Body pain
- Other complaints

---

### 2. Comprehensive History Collection

The workflow includes sections for:

- Presenting complaint
- History of present illness
- Past medical history
- Past surgical history
- Drug history
- Allergy history
- Family history
- Personal history
- Review of systems

---

### 3. AYUSH Assessment

The prototype includes an AYUSH-oriented assessment workflow covering:

- Prakriti
- Agni
- Koshtha
- Ahara–Vihara

---

### 4. Prior Medical Information

The prototype includes a demonstration workflow for extracting structured information from previous medical documents, such as:

- Laboratory values
- Investigations
- Prescriptions
- Discharge-summary information

---

### 5. Clinical Red-Flag Detection

The prototype includes rule-based checks for selected potentially concerning combinations of symptoms.

Examples include:

- Concerning chest-pain combinations
- Thunderclap headache
- Headache with neck stiffness or confusion
- Fever with neck stiffness or confusion
- Severe breathlessness
- Vomiting blood
- Coughing blood

These rules are intended as prototype safety flags and are not a diagnostic system.

---

### 6. Structured Clinical Summary

Collected information is organized into a structured summary containing sections such as:

- Chief complaint
- History of present illness
- Past history
- Drug / allergy history
- Family history
- Personal history
- Review of systems
- AYUSH assessment
- Prior investigations

---

🔄 Patient Workflow


Patient
   ↓
Basic Information
   ↓
Chief Complaint
   ↓
Adaptive Questions
   ↓
Medical History
   ↓
Drug & Allergy History
   ↓
Family / Personal History
   ↓
Review of Systems
   ↓
AYUSH Assessment
   ↓
Prior Medical Information
   ↓
Red-Flag Checks
   ↓
Structured Clinical Summary
   ↓
Doctor Review


➡️Doctor WorkFlow

Doctor Login
     ↓
Patient Queue
     ↓
Select Patient
     ↓
Review Structured History
     ↓
Review Previous Information
     ↓
Review Clinical Flags
     ↓
Begin Consultation

🛠️ Technology Stack

Frontend
HTML5
CSS3
JavaScript

Prototype Data Layer
JavaScript-based mock API layer
LocalStorage-based prototype database

Prototype Logic
Complaint-specific adaptive questioning
Rule-based red-flag detection
Structured clinical-summary generation
Demonstration document-information extraction


🏗️ Prototype Architecture

                 ┌─────────────────────┐
                 │       Patient       │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │   MediKiosk UI     │
                 └──────────┬──────────┘
                            │
                            ▼
              ┌──────────────────────────┐
              │ Adaptive History Engine  │
              └────────────┬─────────────┘
                           │
             ┌─────────────┼─────────────┐
             ▼             ▼             ▼
       Medical History  AYUSH       Prior Records
             │             │             │
             └─────────────┼─────────────┘
                           ▼
                 ┌─────────────────────┐
                 │  Clinical Rules    │
                 │  & Red-Flag Checks │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │ Structured Summary  │
                 └──────────┬──────────┘
                            │
                            ▼
                    ┌──────────────┐
                    │    Doctor    │
                    └──────────────┘
