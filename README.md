# 🧙♂️ RPG Character Management System

A comprehensive Django-based web application for managing RPG characters, their attributes, skills, spells, and inventory items. This project features both a traditional Django frontend and a RESTful API backend.

![Django](https://img.shields.io/badge/Django-4.2-green)
![DRF](https://img.shields.io/badge/Django_REST_Framework-3.14-blue)
![Python](https://img.shields.io/badge/Python-3.8%2B-yellow)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

## ✨ Features

### 🎮 Character Management
- Create, read, update, and delete RPG characters
- Assign races, classes, skills, and spells
- Detailed character profiles with backstories
- Advanced filtering and search capabilities

### ⚡ Attributes System
- Six core attributes: Strength, Dexterity, Constitution, Intelligence, Wisdom, Charisma
- Automatic health and mana calculations based on level and attributes
- Constitution types: Normosthenic, Hypersthenic, Asthenic

### 🎒 Inventory Management
- Track items, quantities, and equipment status
- Various item types: Weapons, Armor, Potions, Plants, Quest Items, Artifacts
- Equip/unequip items functionality

### 🔌 REST API
- Full CRUD operations for all models
- Swagger/Redoc API documentation
- Custom serializers with validation
- Nested relationships and detailed representations

### 🎨 Admin Interface
- Custom Django admin configurations
- Advanced filtering and search
- Bulk operations support

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- PostgreSQL (recommended) or SQLite

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/rpg-character-manager.git
   cd rpg-character-manager
