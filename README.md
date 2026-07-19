[Русская версия](README.ru.md)

# Project2Proxy Releases

This repository hosts official releases of Project2Proxy.

## Download

Go to the [Releases](https://github.com/oracleh2/project2-proxy-releases/releases) page and download the latest `Project2Proxy.exe`.

## What is Project2Proxy?

Project2Proxy is a Windows desktop application that acts as a transparent MITM proxy for captcha-solving services. It intercepts HTTP/HTTPS traffic from third-party software and redirects it to a user-configured backend.

### Features

- Transparent interception of captcha provider APIs
- Two operating modes: dataset collection and captcha solving
- Support for multiple captcha providers simultaneously
- TLS MITM with automatic certificate management
- Bilingual interface (English / Russian)
- System tray integration
- Automatic update checking

### System Requirements

- Windows 10/11 (x64)
- Administrator privileges (required for hosts file and certificate management)
- No additional runtime required (self-contained executable)

## Updating from HuyandexProxy

If you are upgrading from the old HuyandexProxy version, you need to replace the root CA certificate.
See the [CA migration guide](https://github.com/oracleh2/project2-proxy-releases/blob/main/CA-MIGRATION.md) for step-by-step instructions.
