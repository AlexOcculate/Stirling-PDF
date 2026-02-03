# Technology Stack

This document provides a comprehensive overview of the technologies, programming languages, frameworks, and tools used in the Stirling-PDF project.

## Programming Languages

### Backend
- **Java 17+** (Recommended: Java 21)
  - Primary backend language
  - Minimum JDK 17, supports and recommends JDK 21
  - Source/target compatibility: Java 17

### Frontend
- **TypeScript** 
  - Primary frontend language for type-safe development
  - Used with React for UI components
  
- **JavaScript**
  - Legacy JavaScript support
  - Third-party libraries and utilities

### Desktop Application
- **Rust** (Edition 2021)
  - Desktop application framework via Tauri
  - Minimum version: 1.77.2
  - Native cross-platform support

### Scripting & Automation
- **Python 3.12**
  - PDF processing scripts
  - Translation utilities
  - Build and automation tools
  - OCR integration

- **Bash**
  - Build scripts
  - Installation scripts
  - Docker initialization

## Backend Technologies

### Core Framework
- **Spring Boot 3.5.6**
  - Main application framework
  - Spring Boot Starter Web
  - Spring Boot Starter AOP
  - Spring Boot Actuator
  - Spring Boot DevTools (development)
  
- **Spring Security**
  - Authentication and authorization
  - SAML 2.0 support (version 6.5.5)
  - JWT-based authentication
  - OAuth2 integration

### Web Server
- **Jetty**
  - Embedded servlet container
  - Replaces default Tomcat

### PDF Processing
- **Apache PDFBox 3.0.5**
  - Core PDF manipulation library
  - PDF parsing, creation, and modification
  - PDF preflight validation
  - XMP metadata handling
  - JBIG2 image support

### Additional PDF Tools
- **Tabula 1.0.5**
  - PDF table extraction
  
- **pdf-lib** (Frontend)
  - Client-side PDF manipulation
  - Version 1.17.1

### Document Conversion
- **LibreOffice**
  - Office document to PDF conversion
  - Supports multiple document formats
  - Python UNO bridge integration

- **Batik 1.19**
  - SVG processing and conversion
  - Apache XML Graphics

### Image Processing
- **TwelveMonkeys ImageIO 3.12.0**
  - Extended image format support
  - Modules: BATIK, BMP, JPEG, TIFF, WebP, PSD

- **OpenCV** (Python)
  - Computer vision operations
  - Image transformations

### OCR (Optical Character Recognition)
- **Tesseract OCR**
  - Text recognition from images and PDFs
  - Multiple language pack support (English, German, French, Portuguese, Chinese Simplified)
  
- **OCRmyPDF**
  - PDF OCR processing pipeline
  - Integration with Tesseract
  
- **Unpaper**
  - Image preprocessing for OCR
  - Deskew and cleanup operations

### Security & Cryptography
- **Bouncy Castle 1.82**
  - Cryptographic operations
  - bcprov-jdk18on
  - bcpkix-jdk18on

- **OWASP Java HTML Sanitizer**
  - XSS prevention
  - HTML sanitization

- **Java Security Toolkit 1.2.2**
  - Security utilities from Pixee

### Data Processing
- **OpenCSV 5.12.0**
  - CSV file handling

- **JUnRAR 7.5.5**
  - RAR archive support for CBR files

- **JSZip 3.10.1** (Frontend)
  - ZIP file creation and manipulation

### Barcode & QR Code
- **ZXing 3.5.3**
  - Barcode generation and scanning
  - QR code processing

### Documentation
- **SpringDoc OpenAPI 2.8.13**
  - API documentation generation
  - Swagger UI integration
  - OpenAPI specification

- **CommonMark 0.26.0**
  - Markdown processing
  - GitHub Flavored Markdown tables support

### Utilities
- **Commons IO 2.20.0**
  - File and stream utilities

- **Commons Lang3 3.19.0**
  - Common Java utilities

- **Metadata Extractor 2.19.0**
  - Image metadata extraction

- **Flexmark 0.64.8**
  - HTML to Markdown conversion

- **Javaluator 3.0.6**
  - Mathematical expression evaluation

### System Tools
- **Ghostscript**
  - PostScript and PDF processing
  
- **Poppler Utils**
  - pdftohtml conversion utility
  
- **FontForge**
  - Font processing and conversion

### Monitoring & Analytics
- **Micrometer 1.15.4**
  - Application metrics

- **PostHog 1.2.0**
  - Product analytics (backend and frontend)

### Logging
- **Logback 1.5.19**
  - Logging framework
  - logback-core and logback-classic

## Frontend Technologies

### UI Framework
- **React 19.1.1**
  - Component-based UI framework
  - react-dom 19.1.1

### Build Tools
- **Vite 7.1.7**
  - Build tool and development server
  - Fast HMR (Hot Module Replacement)
  - @vitejs/plugin-react-swc for React integration

- **TypeScript 5.9.2**
  - Type checking and compilation

### UI Component Libraries
- **Mantine 8.3.1**
  - Core UI components
  - Hooks, Dates, Dropzone modules

- **Material-UI (MUI) 7.3.2**
  - Material Design components
  - Icons library

- **Emotion**
  - CSS-in-JS styling
  - @emotion/react 11.14.0
  - @emotion/styled 11.14.1

### Styling
- **TailwindCSS 4.1.13**
  - Utility-first CSS framework
  - Custom configuration

- **PostCSS 8.5.6**
  - CSS processing
  - Mantine preset integration
  - Autoprefixer 10.4.21

### PDF Handling (Frontend)
- **PDF.js 5.4.149**
  - Client-side PDF rendering
  - Mozilla's PDF viewer

- **EmbedPDF 1.5.0**
  - Comprehensive PDF viewer framework
  - Multiple plugins: annotation, bookmark, export, history, print, search, thumbnail, zoom, etc.

### Internationalization
- **i18next 25.5.2**
  - Internationalization framework
  - react-i18next 15.7.3
  - i18next-browser-languagedetector 8.2.0
  - Support for 40+ languages

### State Management & Data Handling
- **Axios 1.12.2**
  - HTTP client for API requests

- **IndexedDB**
  - Client-side file storage
  - Thumbnail caching

### Drag & Drop
- **@atlaskit/pragmatic-drag-and-drop 1.7.7**
  - Drag and drop operations

- **@dnd-kit/core 6.3.1**
  - Drag and drop toolkit

- **react-rnd 10.5.2**
  - Resizable and draggable components

### Routing
- **React Router 7.9.1**
  - Client-side routing

### Additional Frontend Libraries
- **@tanstack/react-virtual 3.13.12**
  - Virtualization for large lists

- **@reactour/tour 3.8.0**
  - Guided tours

- **signature_pad 5.0.4**
  - Signature capture

- **smol-toml 1.4.2**
  - TOML parsing

### Payment Integration
- **Stripe**
  - @stripe/stripe-js 7.9.0
  - @stripe/react-stripe-js 4.0.2

### Cloud Integration
- **Supabase 2.47.13**
  - Backend as a Service

### Icons
- **Iconify 6.0.2**
  - Unified icon framework
  - Material Symbols icon set

## Desktop Application Technologies

### Framework
- **Tauri 2.9.0**
  - Cross-platform desktop application framework
  - Lightweight alternative to Electron
  - Native platform integration

### Tauri Plugins
- tauri-plugin-log 2.0.0-rc
- tauri-plugin-shell 2.1.0
- tauri-plugin-fs 2.4.4
- tauri-plugin-http 2.4.4
- tauri-plugin-single-instance 2.0.1
- tauri-plugin-store 2.1.0
- tauri-plugin-opener 2.0.0

### Desktop-Specific Libraries (Rust)
- **keyring 3.6.1**
  - Secure credential storage
  - Native platform integration (Apple/Windows)

- **tokio 1.0**
  - Async runtime

- **reqwest 0.11**
  - HTTP client

- **tiny_http 0.12**
  - Minimal HTTP server

### Platform-Specific (Rust)
- **macOS**
  - core-foundation 0.10
  - core-services 1.0

- **Windows**
  - windows 0.58 (Win32 APIs)

## Build & Development Tools

### Build System
- **Gradle 8.14**
  - Primary build tool
  - Multi-module project structure

### Code Quality
- **Spotless 7.2.1**
  - Code formatting (Google Java Format 1.28.0)
  - Automatic formatting on compilation

- **ESLint**
  - JavaScript/TypeScript linting
  - TypeScript ESLint parser and plugins

### Testing

#### Backend
- **JUnit Platform 1.12.2**
  - Test execution framework

- **JaCoCo**
  - Code coverage reporting

- **Mockito 5.2.0**
  - Mocking framework

- **OkHttp MockWebServer 5.1.0**
  - HTTP server mocking

#### Frontend
- **Vitest 3.2.4**
  - Unit testing framework
  - Coverage with @vitest/coverage-v8

- **Playwright 1.55.0**
  - End-to-end testing

- **Testing Library**
  - @testing-library/react 16.3.0
  - @testing-library/dom 10.4.1
  - @testing-library/jest-dom 6.8.0
  - @testing-library/user-event 14.6.1

- **jsdom 27.0.0**
  - DOM testing environment

#### Integration Testing
- **Cucumber**
  - BDD-style integration tests

### Static Analysis
- **SonarQube 6.3.1.5724**
  - Code quality analysis

- **Dependency License Report 2.9**
  - License compliance checking

## Containerization & Deployment

### Container Technology
- **Docker**
  - Multi-stage builds
  - Alpine Linux 3.22.1 base images
  - Multiple variants: standard, ultra-lite, fat, unified

### Reverse Proxy
- **Nginx**
  - Used in unified Docker deployments
  - Frontend static file serving
  - Proxy configuration for backend API

### Container Orchestration
- **Kubernetes** (supported)
  - See documentation for deployment configurations

## CI/CD

### GitHub Actions
- Automated builds
- Docker image generation
- PR deployment and testing
- Code quality checks
- Auto-labeling
- AI-powered PR reviews

## Configuration & Dependency Management

### Configuration Formats
- **YAML**
  - Application configuration
  - Docker Compose files
  - CI/CD workflows

- **TOML**
  - Tauri configuration
  - Cargo package configuration

- **Properties Files**
  - Legacy backend translations
  - Application properties

- **JSON**
  - Frontend translations
  - Package management (package.json)
  - OpenAPI specifications

### Package Managers
- **npm** (Node.js)
  - Frontend dependency management
  - Version: Managed via package-lock.json

- **Cargo** (Rust)
  - Desktop application dependencies
  - Version: Managed via Cargo.lock

- **Maven Central** (Java)
  - Backend dependency resolution

- **pip** (Python)
  - Python package management

## Database & Storage

### Client-Side Storage
- **IndexedDB**
  - Browser-based file persistence
  - Thumbnail caching
  - LRU cache management

### Backend Storage
- **File System**
  - Temporary file processing
  - Stateless design (no persistent storage by default)

## Runtime Environments

### Java Runtime
- **OpenJDK 21**
  - Primary runtime in Docker containers

### Node.js
- Required for frontend development
- Build-time dependency

### Python 3.12
- Required for PDF processing features
- OCR operations
- Virtual environment: /opt/venv

## Key External Tools & Utilities

### System Libraries
- ca-certificates
- tzdata
- tini
- bash
- curl
- shadow
- su-exec
- openssl
- gcompat
- libc6-compat

### Font Support
- Noto fonts (OpenType)
- Custom TTF fonts

## Development Platforms

### Version Control
- **Git**
  - Source code management
  - GitHub for hosting

### Package Registries
- **Docker Hub / docker.stirlingpdf.com**
  - Container image distribution

- **SwaggerHub**
  - API documentation hosting

- **Maven Central**
  - Java dependency hosting

- **npm Registry**
  - JavaScript package hosting

- **crates.io**
  - Rust package hosting

## Architecture Patterns

### Backend
- **Spring Boot Convention**
  - MVC pattern
  - RESTful API design
  - Dependency injection

### Frontend
- **React Component Architecture**
  - Hook-based components
  - Context API for state management
  - Modular design

### Multi-Tier Architecture
- **Separated Frontend/Backend**
  - React SPA frontend
  - Spring Boot API backend
  - Optional unified deployment with Nginx

### Desktop Integration
- **Hybrid Architecture**
  - Rust-based native shell (Tauri)
  - Web technologies for UI (React)
  - Local backend server

## Deployment Variants

### Standard
- Full feature set
- All dependencies included

### Ultra-Lite
- Minimal dependencies
- Basic PDF operations only

### Fat
- Pre-downloaded dependencies
- Air-gapped environment support

### Unified
- Frontend + Backend in single container
- Nginx reverse proxy

### Desktop
- Native application
- Cross-platform (Windows, macOS, Linux)

## Internationalization Support

### Languages Supported
- 40+ languages via i18next
- Backend: .properties files
- Frontend: JSON translation files
- Conversion scripts available

## Performance Optimization

### Frontend
- Web Worker-based thumbnail generation
- IndexedDB for file persistence
- Background PDF processing
- Virtual scrolling for large lists
- Code splitting with Vite

### Backend
- JVM tuning options
- G1GC garbage collector
- String deduplication
- Periodic GC
- Memory percentage-based heap sizing

## License Management
- License compliance checking
- Allowed licenses configuration
- Automated license report generation

---

**Last Updated:** 2026-02-03  
**Project Version:** 2.1.2  
**Repository:** https://github.com/Stirling-Tools/Stirling-PDF
