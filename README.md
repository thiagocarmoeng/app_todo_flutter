# Developed entire application to consolidate knowledge about flutter + dart.

What i learned building this app?

FutureBuilder: Screen construction widget capable of waiting for asynchronous information. FutureBuilder must have two parameters: future:, responsible for asynchronous information, and builder:, responsible for building the screen. It is worth remembering that we use the concept of snapshot as a variable capable of storing asynchronous information.

ConnectionState: We learned that when dealing with a database (or any information that comes from outside our project) we have to be aware of the information waiting time. Today it is very common to believe that, because it is extremely fast, we do not have a waiting time when receiving data. However, there is a time when the information is not complete and, in this case, we use the ConnectionState (which is the current state of the snapshot) to build several screens depending on the state of the information.

Adding information to the DB: In the crucial part of the implementation in our project, we added the ability to save a task directly to the database to the form, for this we remember the controlled data coming from the form and apply the save() function coming from the DAO and, this way, we add a new task to the database.

Deleting information in the DB: To remove Tasks from our database, the delete() method was implemented within the Task Class, using a secondary action (onLongPress) in the previously implemented ElevatedButton.

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
