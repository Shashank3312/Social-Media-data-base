# Social Media Database Project

This project is a relational database design for a social media platform. It includes the schema, data, and relationships required to manage users, posts, comments, groups, events, messages, and more. The database is implemented using MySQL and is designed to support various features commonly found in social media platforms.

## Features Implemented

### 1. User Management
- Users can register with details like email, username, birthdate, gender, and name.
- Users can have multiple phone numbers.
- Verified users are tracked with verification methods and timestamps.

### 2. Posts and Comments
- Users can create posts with visibility options (`Public`, `Friends-only`, `Private`).
- Posts can have media links (images, videos, etc.).
- Users can comment on posts and reply to comments.

### 3. Reactions
- Users can react to posts, comments, and replies with various reaction types (e.g., `Like`, `Love`, `Laughing`, etc.).

### 4. Messaging
- Users can send direct messages to each other.
- Messages have timestamps for when they were sent and seen.

### 5. Groups
- Users can create and join groups.
- Groups have descriptions and timestamps for when they were created.

### 6. Events
- Users can create events with details like name, description, venue, city, country, start and end times.
- Users can attend events.

### 7. Pages
- Users can create and follow pages.
- Pages have categories, descriptions, and timestamps for when they were created.

### 8. Friendships
- Users can establish friendships with other users.

## Queries That Can Be Processed

Here are some example queries that can be executed on this database:

1. **Retrieve all posts by a specific user.**
2. **Find all comments on a specific post.**
3. **List all users attending a specific event.**
4. **Get all groups a user is a member of.**
5. **Fetch all messages sent between two users.**
6. **Find all reactions to a specific post or comment.**
7. **List all pages followed by a specific user.**
8. **Retrieve all friends of a specific user.**
9. **Get all events created by a specific user.**
10. **Find all replies to a specific comment.**

## How to Run

### Prerequisites
- MySQL installed on your system.
- A MySQL client or command-line access to execute SQL scripts.

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/Nikhilesh4/Social-Media-db.git
   cd Social-Media-db
   ```

2. Open the `dumps.sql` file located in the project directory.

3. Import the SQL dump into your MySQL database:
   ```bash
   mysql -u <username> -p <database_name> < dumps.sql
   ```

4. Verify the database schema and data by connecting to your MySQL instance:
   ```bash
   mysql -u <username> -p
   USE <database_name>;
   SHOW TABLES;
   ```

5. Execute queries to interact with the database.

### Notes
- Replace `<username>` and `<database_name>` with your MySQL username and the name of the database you want to use.
- Ensure that foreign key constraints are enabled in your MySQL configuration.

## Repository Structure
- `dumps.sql`: Contains the SQL schema and data for the database.
- `.git/`: Git configuration files for version control.
- `README.md`: Documentation for the project.

Feel free to explore and extend the database to add more features or optimize its performance!

