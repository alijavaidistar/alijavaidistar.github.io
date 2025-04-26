---
title: "Whiterock - Academic Forms Management System"
excerpt: "A comprehensive Django web application for educational institutions to manage academic forms and approval workflows. Features Microsoft OAuth integration, role-based access control, and LaTeX-powered PDF generation.<br/>"
collection: portfolio
---

## Overview
Whiterock is a Django-based web application designed to streamline the management of academic forms and their approval workflows for educational institutions. The system supports various document types with complex multi-department approval routing.

[View on GitHub](https://github.com/alijavaidistar/WhiteRock)

## Technical Architecture

### Core Components
- **Django Backend**: Built on Django 5.1 with a modular approach using multiple apps  
- **Authentication**: Microsoft OAuth integration using MSAL for secure, enterprise-ready login  
- **Frontend**: Responsive Bootstrap 5 UI with form validation and AJAX functionality  
- **Document Generation**: LaTeX templates with dynamic content insertion for professional PDFs  
- **Database**: Flexible configuration supporting both SQLite and PostgreSQL  
- **Containerization**: Docker and Docker Compose setup for consistent deployment  

### Key Features

#### Role-Based Access Control
- **Staff**: Department-specific application approvals and user management  
- **Admin**: Limited approval capabilities within assigned departments  
- **Basic User**: Form submission with personal application tracking  

#### Multi-Department Approval Workflow
- Configurable approval rules determine required departments for each form type  
- Sequential or parallel approval patterns  
- Comment system for returned forms requiring revision  
- Approval tracking dashboard with notification system  

#### Form Management
- Support for multiple form types:
  - Special Circumstance Forms  
  - Course Drop Forms  
  - FERPA Authorizations  
  - Texas Residency Affidavits  
- Draft saving and revision capabilities  
- Digital signature upload and management  
- Form status tracking (Draft, Pending, Approved, Returned)  

#### PDF Generation
- Professional document generation using LaTeX templates  
- Dynamic content insertion based on form data  
- Signature embedding in generated documents  
- Downloadable PDFs for record-keeping  

#### External System Integration
- RESTful API for cross-system form submissions  
- Integration with external form services  
- Data validation and synchronization  

## Development Challenges & Solutions

### Authentication & Security
Implemented Microsoft OAuth for enterprise-ready authentication while maintaining a secure session management system. Role-based permissions ensure users can only access appropriate system features.

### Approval Workflow Management
Designed a flexible system where administrators can define department approval requirements for each form type. The system tracks which departments have approved and requires appropriate permissions for approvals.

### PDF Generation
Integration of LaTeX for high-quality PDF generation required careful handling of user inputs, template management, and proper character escaping. The system generates professional-looking documents with embedded signatures.

### User Experience
Created an intuitive interface that guides users through form submission and approval processes with clear status indicators, validation, and helpful error messages.

## Demo Video
<div style="position:relative;padding-bottom:56.25%;height:0;overflow:hidden;">
  <iframe 
    src="https://www.youtube.com/embed/mrRwb6p2X4M?start=32" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
    allowfullscreen 
    style="position:absolute;top:0;left:0;width:100%;height:100%;">
  </iframe>
</div>
