# PollApp
A simple, fully functional polling application built with Django, inspired by the official Django documentation — but expanded with clean code structure, dynamic templates, and real voting logic.
This project allows users to:

✔ View a list of poll questions

✔ Open a question and see all the available choices

✔ Cast a vote on any choice

✔ See real-time results after voting

 # Features
1. List of All Poll Questions

The index view fetches all questions from the database and displays them on the homepage using the polls/index.html template.

2. Question Detail Page

The detail view shows a specific question along with all its choices.
Handled using get_object_or_404 for clean error management.

3. Voting System

The vote view processes form submissions, updates vote counts, and gracefully handles errors when no choice is selected.

4. Results Page

After voting, users are redirected to the results page using HttpResponseRedirect and reverse() for clean URL handling.

 # Key Django Concepts Used

Django Models (Question, Choice)

URL routing with namespace (polls:)

QuerySets & ORM methods (question.choice_set.get())

Error handling using try/except

get_object_or_404 for clean fetching

Templates and context rendering

POST request handling

Redirects & named URLs
