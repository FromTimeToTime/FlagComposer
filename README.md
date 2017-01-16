# FlagComposer
EXERCISE: let's build a software tool using XML to define a set of national flags.

This project is addressed to students or programmers who'd like to have
a small programming task to solve as an exercise in their free time...

Here's its description...

Let's imagine we want a software tool to define a set of national flags.

The goal of this project is to build a GUI starting from a XML file
(e.g. "FlagComposer.xml") and to generate an output XML file (e.g.
"FlagGermany.xml") according to what has been set by the user in the GUI.

In input we have one (or more... but not simultaneously processable)
XML file(s) defining which elements (graphical controls) should
compose the GUI, which parameters are needed to define a flag,
which values are valid; in output we want to have one XML file for each
flag definition. It is not required to display an image of the flag:
the XML file is all that is required as a result of the processing.

The application must read a XML file containing a "GUIDefinition" element
and draw a graphical user interface accordingly. It must also be able to
generate and write out a XML file containing a "FlagDefinition" element.

[Application is launched]
  ==>
[Read XML {GUIDefinition}]
  ==>
[Draw GUI accordingly]
  ==>
[Process user's "Save" or "Exit" command]
  ==>
["Save" creates XML {FlagDefinition}]
  ==>
[Exit]

Starting from the {GUIDefinition} element of the input XML data, we want
to build up a GUI where the user can enter the required parameters, for
instance (...see "FlagComposer.xml"):

1. a "Name" should be entered through an editable text field;

2. a "Direction of Stripes" specification should be entered through a list
   box (or choice box) displaying the available options ("Horizontal" and
   "Vertical") and allowing the user to select one of them;

3. a "Number of Stripes" should be entered through a numeric spin box
   ranging from "MinValue" to "MaxValue" (eventually initialized to
   a "DefaultValue");

4. a set of list/combo boxes should allow the user to enter the colors of
   the flag: the GUI must provide N occurrences of the "Color of Stripe"
   parameter (list/combo boxes) according to the previously set "Number
   of Stripes".

Once the user has entered all the required data, an enabled button or
menu option should allow him to generate and save the output XML file with
the final {FlagDefinition} element (to have an example of the output file,
see "FlagGermany.xml").

To develop the application, free or open source tools should be preferred
over commercial ones, but the choice of the programming language, IDE and
framework, with which to implement the application, is ultimately left
open to any option and demanded to the programmer (that is, to anyone who's
going to try to implement a solution to this problem): you may choose
whatever language or framework you like. Of course, the simpler and
faster-to-implement-and-maintain the solution is, the more it will turn out
valuable.

A set of XML files, to use as a model of the input data ({GUIDefinition})
that should be used by the application and of the output ({FlagDefinition})
that should be produced, is available:

https://github.com/FromTimeToTime/FlagComposer/

Please, fork the project to suggest your ideas or your implementation
of a solution.
:)
