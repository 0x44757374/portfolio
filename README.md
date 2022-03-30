# Portfolio
> Personal Portfolio of Work(s)
> </br> 🚧 Link to project list + demo page in-progress 🚧

# Table Of Contents
1. [About](#about)
2. [Highlight Work](#highlight-work)
3. [Publications](#publications)

___

# About
My name is Dustin! 😊 I am an engineer that focuses primarily on cloud services, and user applications. </br>
I enjoy using engineering to solve problems and to help friends solve problems. </br>
</br>
I strongly believe that simplicity brings the best solution(s).
___


# Highlight Work

## [SNOdar](https://sensorlogic.ai/content/specifications-pdfs/snodar_data_sheet-2.pdf)
> Snow measurement sensor with cloud services, web, and mobile applications</br>
> Custom hardware, firmware, mobile applications, and cloud services/architecture

### My Roles
> Lead for cloud & mobile, secondary contributor to firmware

### Cloud Architecture & Services
- Built custom (standardized) build, dev, deploy, and status cli toolchain in bash
- Created custom docker images to verify standardized structure, cleanup, and minimize size
- Standardized images/containers for services to run on 32 bit hardware, single instance, distributed system, or standalone service.
- Load balancing
- Services
  - API(s)
    - Custom (minimized) Docker Image
    - Custom RCP over TCP w/ SSL
    - Graphql Endpoint for User interactions
    - Sensor data ingestion
    - User Authentication
    - User session caching
    - User query caching
    - Sensor RPC result caching
    - Sensor LTE FOTA
    - API Key authentication
  - Cache
    - Custom Docker Image
    - Redis
  - Database
    - Postgres database
    - Database migration tools (for custom toolchain)
    - Designed relational data structure
    - Custom queries
    - Authentication functions
    - Blob data storage
  - Reverse Proxy (Server)
    - Custom (minimized) Docker Image
    - Automated SSL Certificates
    - Load balancing
    - Access Layers (exclude stream access to authorized containers, or networks ie, api --> database)
    - Security (built (from source, into docker iamge) + configured webapp firewall for public https traffic)
  - Web Application
    - Custom (minimized) Docker Image
    - SolidJS Application 
    - User authentication
    - Data Visualization
    - Organizations (Create, invite, join, leave, delete...)
    - Sensors (Register, view, manage...)
  - Mailserver
    - Custom (minimized) Docker Image
    - Custom domain emails (for scaling to support, email auth, email verification, automated responses etc.,)
  - Documentation
    - Custom (minimized) Docker Image
    - Dynamic build pipeline based on api schema changes

### Firmware Integration & Design
- Designed + integrated firmware <--> user application interfaces (parallel development)
- Designed custom GATT spec

### Mobile App(s)
- [🤖 Android](https://play.google.com/store/apps/details?id=com.snodar)
- [🍎 iOS](https://apps.apple.com/us/app/snodar/id1584974884)
- Features
  - FOTA/BLE Firmware Updates
  - Sensor Setup (Guided, with defaults -- configure a new sensor in under 5 minutes)
  - Multi Sensor Management
  - Sensor Configuration
    - Name, Mode
    - Measurement interval, daily reset
    - Calibration
    - Logging (internal, external)
  - Sensor Security
  - Custom BLE GATT
  - Sensor Search
  - Themes
  - Easy Sensor/App/Cloud Documentation
  - Sensor Health/Status
  - Sensor Updates
  - Developer Mode/tools
    - BLE Uart/Commands
    - Additional Status Indicators
  - Sensor Data
    - Sharing
    - Acquisition
    - Visualization

[👆 Back to Top](#portfolio)
___


# Publications

## [FPGA Coode & IO Generation (AES)](https://www.aes.org/tmpFiles/elib/20220330/20965.pdf)
> System/toolchain for generating VHDL code, linux device drivers, overlays, control system, and user application w/ generated I/O.

Features
- Cloud FPGA Bitstream upload/download
- Instant FPGA Bitstream loading/project switching
- Local application server & middleware for controlling SoC FPGA on Embedded Linux
- Per-project Generated UI Controls
  - Synchronized for multiple users (dragging a slider on your view will drag the slider for other users)
  - Adjustable (Control layouts, limits, steps, and other properties can be modified live)
  - Realtime (I/O to FPGA is processed in under 50ms, worst-case)

## [Open Audio Processing Platform (AES)](https://www.aes.org/e-lib/browse.cfm?elib=20623)
> Open platform for software and tools for simplifying audio signal processing hardware and software design (primarily toward hearing aid development R&D)

Features
- Model-based FPGA Design tools
- Open source platform (devlopment, and design)
- Mobile/desktop application for live controls with SoC FPGA

[👆 Back to Top](#portfolio)
___





