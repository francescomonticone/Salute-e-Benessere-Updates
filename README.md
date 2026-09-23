# Desktop application for the professional management of employee health and well-being assessments

**Salute e Benessere Aziendale** is designed to support healthcare professionals in collecting data, processing assessments, and monitoring patient progress over time.

## Features

* 👤 **Patient Management**

  * Patient records
  * Patient search and consultation
  * Assessment history
* 📋 **Assessments**

  * Creation of new assessments
  * Saving assessments as drafts
  * Completion and editing of assessments
  * Comparison between assessments performed at different times
* 📊 **Data Processing**

  * Automatic calculation of the required indicators
  * Support for different assessment methodologies
  * Configurable parameters and formulas
  * Results saved together with the assessment
* 👨‍⚕️ **Doctor Profile**

  * Professional information
  * Organization and contact details
  * Logo and signature
  * Login credential management
* 📄 **Reports**

  * Assessment report generation
  * Results summary
  * Comparison with previous assessments
  * Automatic use of the doctor's professional information
* 📤 **Export**

  * Export of data and reports in the formats supported by the application
* ⚙️ **Configuration**

  * Configurable formulas
  * Formula change history
  * Parameters can be modified without changing the application
* 🔄 **Automatic Updates**

  * Checks for new versions
  * Downloads updates directly from the application
  * Cryptographic verification of updates

## Privacy and Security

Patient and assessment data are managed **locally on the computer** where the application is installed.

The local database contains the data required for the application to operate and is not included in the project repository or in the distributed installers.

Login credentials are not stored in plain text: passwords are stored using an **Argon2 hash**.

Personal data, local databases, reports, and any personal files belonging to the professional are not included in the source code or application releases.

> **Important:** The application handles potentially sensitive data. It is the user's responsibility to protect the computer, operating system account, and backups containing such data.

## Updates

The application includes an integrated update management system.

When a new version is released, the application can:

1. check whether an update is available;
2. notify the user about the new version;
3. download the update;
4. verify its signature;
5. install the new version.

Updates are distributed through GitHub Releases.

## Technology

The application is developed using:

* **Tauri 2** — desktop framework
* **React** — user interface
* **TypeScript** — frontend development
* **Rust** — backend and application logic
* **SQLite** — local database
* **Argon2** — password protection

## Supported Systems

Versions are planned for:

* 🪟 **Windows**
* 🍎 **macOS**

Installers are published through the application's releases.

## Project Structure

The project is mainly organized as follows:

```text
Salute-e-Benessere-aziendale/
├── src/                    # React frontend
├── src-tauri/              # Rust backend and Tauri configuration
│   ├── src/
│   └── tauri.conf.json
├── public/                 # Public assets
└── package.json
```

**svg**

The application's database is created in the system's local data directory and **is not stored within the project**.

## Versioning

The project follows semantic versioning.

Example:

```text
v0.1.0
v0.1.1
v0.2.0
v1.0.0
```

**svg**

Releases are automatically generated using **GitHub Actions**.

## License

[svg](https://github.com/francescomonticone/Salute-e-Benessere-Updates#licenza)

This software is a proprietary project.

The source code is not intended for redistribution or modification by third parties without authorization from the owner.
