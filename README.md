# Kurukshetra Database Management Tool

A Python-based database management tool for the Kurukshetra database, which contains information about the epic battle of Mahabharata, including warriors, kingdoms, weapons, and battle formations.

## Features

- Retrieve warrior details by kingdom
- View divine weapons information with filtering by invincibility
- Display battle formations by day
- Show kingdoms by alliance (Kauravas/Pandavas)
- Calculate total strength by Anga (army division)
- Search warriors by name (partial or full)
- List divine weapons by kingdom
- View formation and warrior names by kingdom
- Add new warriors to the database
- Modify battle formations
- Delete events from Yuddhahani
- Add new battle formations

## Requirements

- Python 3.6+
- PyMySQL
- Colorama
- Rich

## Installation

1. Clone the repository:
    ```
    git clone https://github.com/yourusername/kurukshetradb.git
    cd kurukshetradb
    ```

2. Install the required packages:
    ```
    pip install pymysql colorama rich
    ```

3. Import the database schema:
    ```
    mysql -u username -p database_name < sql/finaldb.sql
    ```

## Usage

1. Run the main application:
    ```
    python ui/kuru.py
    ```

2. Log in with your database credentials when prompted
3. Use the interactive menu to navigate through the available features

## Database Structure

The database consists of multiple tables including:

- KINGDOM: Information about kingdoms and their allegiances
- WARRIOR: Details about warriors
- WARRIOR_NAME: Names of warriors (many-to-one relationship)
- WARRIOR_SKILLS: Skills possessed by warriors
- DIVINE_WEAPON: Information about divine weapons
- BATTLE_FORMATION: Battle formations used during the war
- ARMY: Army details
- CHATURANGA: Army divisions (Infantry, Cavalry, Elephants, Chariots)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.