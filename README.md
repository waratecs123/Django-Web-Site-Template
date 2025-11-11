# RPG Character Management System

## Overview

A comprehensive Django-based web application designed for managing tabletop role-playing game characters. This system provides robust tools for game masters and players to create, manage, and track character information, attributes, inventory, and progression within RPG campaigns.

## System Architecture

### Technology Stack
- **Backend Framework**: Django 4.2
- **API Framework**: Django REST Framework 3.14
- **Python Version**: 3.8 and above
- **Database**: PostgreSQL (recommended for production) or SQLite (development)
- **Authentication**: Django's built-in authentication system
- **Documentation**: Swagger/Redoc for API documentation

## Core Features

### Character Management System
- Complete character lifecycle management (create, read, update, delete)
- Race and class assignment with associated bonuses and restrictions
- Skill and spell management with progression tracking
- Detailed character profiles including biographical information and backstories
- Advanced filtering, search, and sorting capabilities across character attributes

### Attribute System
- Six core character attributes following standard RPG conventions:
  - Strength (physical power and combat effectiveness)
  - Dexterity (agility, reflexes, and precision)
  - Constitution (health, stamina, and resilience)
  - Intelligence (knowledge, reasoning, and magical aptitude)
  - Wisdom (perception, intuition, and willpower)
  - Charisma (persuasion, leadership, and social influence)
- Automated health and mana calculations based on character level and attributes
- Support for multiple constitution types:
  - Normosthenic (balanced physique)
  - Hypersthenic (robust build)
  - Asthenic (slender build)

### Inventory Management
- Comprehensive item tracking system with quantity management
- Equipment status monitoring (equipped/unequipped)
- Support for multiple item categories:
  - Weapons (melee, ranged, magical)
  - Armor (light, medium, heavy, shields)
  - Potions (healing, buffs, utility)
  - Plants (herbal components, alchemical ingredients)
  - Quest Items (plot-critical objects)
  - Artifacts (unique, powerful items)
- Equipment management with slot-based system

### RESTful API
- Full CRUD (Create, Read, Update, Delete) operations for all data models
- Comprehensive API endpoints for characters, items, skills, and spells
- Custom serializers with advanced validation and data transformation
- Nested relationships for complex object hierarchies
- Detailed resource representations with related entity information
- Pagination, filtering, and search capabilities

### Administrative Interface
- Customized Django admin configuration for efficient data management
- Advanced filtering and search functionality
- Bulk operation support for mass updates
- Audit trails and change history
- User and permission management

## Installation and Deployment

### Prerequisites
- Python 3.8 or newer
- PostgreSQL database system (recommended for production environments)
- Virtual environment tool (venv, virtualenv, or conda)
- Git for version control

### Installation Procedure

1. **Repository Acquisition**
   ```bash
   git clone https://github.com/yourusername/rpg-character-manager.git
   cd rpg-character-manager
   ```

2. **Virtual Environment Setup**
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/macOS
   # or
   venv\Scripts\activate  # Windows
   ```

3. **Dependency Installation**
   ```bash
   pip install -r requirements.txt
   ```

4. **Database Configuration**
   - Create PostgreSQL database
   - Update database settings in `settings.py`
   - Run database migrations:
   ```bash
   python manage.py migrate
   ```

5. **Superuser Creation**
   ```bash
   python manage.py createsuperuser
   ```

6. **Development Server Initialization**
   ```bash
   python manage.py runserver
   ```

### Production Deployment Considerations
- Configure production database settings
- Set up static file serving
- Implement proper security measures
- Configure web server (nginx/Apache)
- Set up SSL/TLS encryption
- Implement backup strategies

## API Documentation

The system includes comprehensive API documentation available through:
- Swagger UI: `/api/docs/`
- ReDoc: `/api/redoc/`

## Data Models

### Character Model
- Personal information (name, age, gender)
- Racial and class attributes
- Attribute scores and modifiers
- Health, mana, and experience points
- Inventory and equipment relationships
- Skill and spell proficiencies

### Item Model
- Item classification and categorization
- Statistical properties (damage, armor, effects)
- Weight, value, and rarity
- Equipability conditions
- Stack size limitations

### Skill and Spell Models
- Skill categories (combat, social, knowledge, etc.)
- Spell schools and levels
- Resource costs and cooldowns
- Prerequisite requirements
- Effect descriptions and mechanics

## Security Features

- Django's built-in security middleware
- CSRF protection
- SQL injection prevention
- XSS protection
- User authentication and authorization
- Permission-based access control
- Data validation at all application layers

## Customization and Extensibility

The system is designed with modularity in mind, allowing for:
- Custom race and class definitions
- Modified attribute systems
- Expanded item categories
- Additional skill and spell types
- Integration with third-party systems
- Theming and UI customization

## Support and Maintenance

For technical support, bug reports, or feature requests, please refer to the project's issue tracker on GitHub. Regular updates and security patches will be maintained according to the project's release schedule.

## License

This project is licensed under the MIT License. See LICENSE file for complete details.

## Contributing

Development contributions are welcome. Please follow the established code style guidelines and submit pull requests through the project's GitHub repository.
