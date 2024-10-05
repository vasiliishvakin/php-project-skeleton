# PHP Project Skeleton

## Overview

A complete PHP project template for local development using Docker and VS Code DevContainers. Includes PHP, MySQL, and development tools like MailHog. Additionally, it supports Vite for building frontend assets.

## Features

- **PHP + Node.js + Python** in a single container 
- **MariaDB** for database support
- **MailHog** for email testing
- **VS Code DevContainer** setup for easy development

## Vite Configuration

```javascript
import { defineConfig } from 'vite';
import dns from 'node:dns';

dns.setDefaultResultOrder('verbatim');

export default defineConfig({
    server: {
        host: '0.0.0.0',
        port: 5173,
        strictPort: true,
        origin: 'http://localhost:5173'
    }    
});

