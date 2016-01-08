# dotnet-Software-Productions-C-Code-Samples
Software Productions' C# Code Samples

* An Undo and Redo library, allowing you to provide full undo and redo functionality in your applications.
* An XML Serializer that can serialize and deserialize any .NET object graph into human readable XML.
* Code to save a file as BLOB data in SQL Server without loading the entire file into memory.
* A routine to automatically arrange the TAB order of the controls on a form.
Users love undo. Being able to undo and redo actions in an application saves users from losing work through simple mistakes, and gives them the confidence to experiment while learning new features. Undo and Redo are difficult features to implement however, so it is left out of many applications where it would be useful.

The Undo Redo library provides a lot of the difficult part of implementing Undo/Redo pre-built. All you have to do is record data changes in the UndoChain. Undoing and Redoing those changes is then handled by the library. If your data is stored in ADO.NET DataSets, it can even record data changes itself, leaving you practically no work to do!

* Uses a circular buffer to store changes, so you can specify any number of actions that are allowed to be undone, and the UndoChain will never use more memory or perform expensive array copying operations.
* Automatically records changes to an ADO.NET DataSet or DataTable.
* Allows multiple changes to be grouped so they are Undone/Redone as a unit.
* Automatically modifies the values of your data when the user performs an undo/redo, and calls an event so you can update the UI if required.
* Can undo changes to your data model, or to the controls on a form, depending on how changes are logged.
* Built in actions modifying a property value, adding or removing an item from a list or dictionary, changing a value in a DataRow, adding and removing a DataRow from a DataTable
