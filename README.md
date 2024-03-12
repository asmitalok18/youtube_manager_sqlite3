# YouTube Manager with SQLite Database

This Python script serves as a YouTube video manager with integrated SQLite database functionality. Users can perform basic CRUD (Create, Read, Update, Delete) operations on a collection of videos, with the video data stored in a SQLite database named "youtube_videos.db."

## Database Structure

- **Table: videos**
  - `id` INTEGER (Primary Key)
  - `name` TEXT (Not Null)
  - `time` TEXT (Not Null)

## Functionalities

1. **List Videos:**
   - Fetches and displays all videos from the database.

2. **Add Videos:**
   - Takes user input for a new video's name and time, then inserts it into the database.

3. **Update Videos:**
   - Prompts the user for a video ID, new name, and new time to update the corresponding video in the database.

4. **Delete Videos:**
   - Prompts the user for a video ID and deletes the corresponding video from the database.

5. **Exit App:**
   - Allows users to gracefully exit the application.

## Implementation

- Utilizes SQLite as a database for persistent storage.
- Exception handling ensures the proper handling of database operations.
- The main function (`main()`) presents a simple command-line interface for users to interact with the application.

## Usage

1. Clone the repository.
2. Run the script.
3. Follow the on-screen prompts to manage your YouTube videos.

## Dependencies

- Python 3.x
- SQLite

## How to Run

```bash
python youtube_manager.py
Example

 Youtube manager app with DB
1. List Videos
2. Add Videos
3. Update Videos
4. Delete Videos
5. exit app
Enter your choice: 1
(1, 'Video1', '10:30')
(2, 'Video2', '05:45')

Enter your choice: 2
Enter the video name: New Video
Enter the video time: 08:15

Enter your choice: 1
(1, 'Video1', '10:30')
(2, 'Video2', '05:45')
(3, 'New Video', '08:15')

...
This script provides a straightforward command-line interface for managing a collection of YouTube videos with database integration using SQLite.
