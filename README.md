### Checklists

#### What?
Checklists are used to help folks perform the same set of tasks over and over
without having to worry about which items have or have yet to be performed.
Think of a checklist as a todo list that you write once and use over and over.

#### Data Format ( as simple as possible )
Checklists are files containing lines of tasks to be completed (one per line).

Items that are done are preceeded by 'x \<date stamp\> '
Where x is a literal character 'x' and \<date stamp\> is the date time that the task
was completed in GMT.

```
x 08/13/14 18:46:27 do something useful
```

Items that are not done just look like a line of text.

```
this is a checklist item that has not yet been done
```

Typically a checklist is created and, if it's to be used, a copy is made first.  To
facilitate this distinction between a checklist 'template' and one in use we use
two dstinct file extensions.

* `.checklist` - This file is intended to be the checklist template i.e. it will
have a list of tasks but none will be marked complete here.
* `.clint` - This file is an 'instance' of a checklist, created by copying a
`.checklist` file.  This file is expected to contain indicators of item completion
as decribed above.
