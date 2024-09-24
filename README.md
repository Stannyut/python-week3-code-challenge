# python-week3-code-challenge
# Concerts Database Project

This project is a concert management system using raw SQL queries and SQLite3. It manages the relationship between **Bands**, **Venues**, and **Concerts** in a many-to-many structure.

## Features
- Store and retrieve information about bands, venues, and concerts.
- Manage many-to-many relationships between bands and venues via concerts.
- Execute raw SQL queries to interact with the database (CRUD operations, aggregations, etc.).

## Database Schema

### Tables
1. **bands**:
   - `id`: Primary Key (Auto-increment)
   - `name`: Name of the band (String)
   - `hometown`: Hometown of the band (String)

2. **venues**:
   - `id`: Primary Key (Auto-increment)
   - `title`: Name of the venue (String)
   - `city`: City where the venue is located (String)

3. **concerts**:
   - `id`: Primary Key (Auto-increment)
   - `band_id`: Foreign Key referencing `bands(id)`
   - `venue_id`: Foreign Key referencing `venues(id)`
   - `date`: Date of the concert (String)

## Setup Instructions

### Prerequisites
- Python 3.x
- SQLite3

### Steps to Set Up and Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/concerts-database.git
   cd concerts-database
