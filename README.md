# ~ MOOD MATCH ~

## Team Members: Lydia, Alaa, Labiba

# Purpose
The purpose of this program is to gain user input on their mood, favorite genre, and favorite author. Based on that, it recommends books back. 

# Description
MoodMatch Reads is a Python command-line program that recommends books based on your current mood, preferred genre, and favorite author. It fetches real-time data from the Open Library and ranks results by relevance.

# Book Library
The Book Library is generated via Claude AI. Claude AI was prompted to use the top books on openlibrary.org with the highest rankings. Each book consists of 5 fields: [title, author, genre, mood, rating]

## How It Works
1. Enter your mood, genre, and/or favorite author
2. The program stores preferences
3. Matches and ranks based on scoring system
4. Display 5 recommendations 
5. Choose to see more recommendations, new search, or exit

# Code Logic 
The code is set up and stored via lists and functions. The main loop runs the program continously until the user quits. The loop on display for the user gives 5 results at a time. While loop is used extensively.

## Functions 
1. print_welcome(): Displays Welcome message

2. print_list(options): Prints a numbered list (mood and genre)

3. ask_for_choice(question, options): Prompts user to choose genre, mood, and author by number or word. Can Skip by pressing Enter

4. ask_for_author(): Prompts user to enter an author name, can skip by pressing Enter

5. ask_yes_no(question)

6. rank_books(mood, genre, author):	Scores each matches based on preferences and sorts them

7. show_books(scored_books, start_index):	Displays 5 books at a time in descending score order

8. main(): Main program that runs the full program with all functions in a loop

## Scoring System (rank_books)
- Mood match → +3 points
- Genre match → +2 points
- Author match → +3 points

thanks!
