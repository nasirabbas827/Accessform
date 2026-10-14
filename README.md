# AccessForm - Inclusive & Accessible Survey Platform

Accessform is an accessible survey platform for creating forms and collecting responses.

![PHP](https://img.shields.io/badge/PHP-2563EB?style=flat-square) ![MySQL](https://img.shields.io/badge/MySQL-0F172A?style=flat-square)

## Overview

The data model covers `accessibility_logs`, `admins`, `forms`, `form_answers`, `form_responses`, `questions`, `users`.

## Application areas

| Area | Pages in the repository |
| --- | --- |
| Admin | [`admin/admin_accessibility_compliance.php`](admin/admin_accessibility_compliance.php), [`admin/admin_home.php`](admin/admin_home.php), [`admin/admin_login.php`](admin/admin_login.php), [`admin/admin_monitor_surveys.php`](admin/admin_monitor_surveys.php), [`admin/admin_navbar.php`](admin/admin_navbar.php) |
| Creator | [`creator/create_form.php`](creator/create_form.php), [`creator/creator_dashboard.php`](creator/creator_dashboard.php), [`creator/export_responses.php`](creator/export_responses.php), [`creator/view_form.php`](creator/view_form.php), [`creator/view_responses.php`](creator/view_responses.php) |
| Root Pages | [`login.php`](login.php), [`register.php`](register.php) |
| Respondent | [`respondent/log_accessibility.php`](respondent/log_accessibility.php), [`respondent/respondent_dashboard.php`](respondent/respondent_dashboard.php), [`respondent/submit_response.php`](respondent/submit_response.php), [`respondent/view_form.php`](respondent/view_form.php) |

## Getting started

### 1. Get the project

```bash
git clone https://github.com/nasirabbas827/Accessform.git
cd Accessform
```

### 2. Configure PHP and the database

1. Use a local PHP server with MySQL or MariaDB, such as XAMPP.
2. Import [`Database/accessform_db.sql`](Database/accessform_db.sql) into your local database server.
3. Set your local database connection details in [`admin/config.php`](admin/config.php), [`config.php`](config.php), [`creator/config.php`](creator/config.php), [`respondent/config.php`](respondent/config.php).
4. Keep the existing asset and upload directory paths intact.

### 3. Start the application

With the database running, start a local development server from the repository root:

```bash
php -S 127.0.0.1:8000
```

Open http://127.0.0.1:8000/index.php. If using Apache/XAMPP instead, place the project in its document root and open the matching localhost folder.

## Repository guide

| Path | Purpose |
| --- | --- |
| [`Database`](Database) | Database scripts |
| [`config.php`](config.php) | Application/database configuration |
| [`css`](css) | Stylesheets |
| [`images`](images) | Image assets |
| [`index.php`](index.php) | Web entry page |
| [`js`](js) | Browser scripts |

## Development notes

These setup instructions are based on the repository source. The application has not been executed as part of this documentation update; verify dependencies and configuration in your local environment.
