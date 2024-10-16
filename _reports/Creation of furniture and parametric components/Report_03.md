# Creation of furniture and parametric components

## FPA Grant to Francisco Rosa

## Report 3, 09/15/2024

In this third report on the development of parametric components, we once again present a summary of the work carried out, a brief description of the procedures adopted, the next steps and some comments.

## 1. Work carried out

We continue to develop individual files for kitchen, bathroom and living room, as well as their equipment such as refrigerators, stoves and washing machines, including the possibility of moving and rotating the original components through their basic Sketches.

The structuring of the components through *Attachments*, as already explained in the previous report, prevented them from falling apart, as usually happens.

In this way, their applications, through the FreeCAD library in the projects, can be carried out completely, without the need to create copies or links, leaving these alternatives as options.

Some rendered images have been posted demonstrating the results of the configurations developed.

As previously mentioned, each file contains: a set of its main configurable properties; a base for moving and rotating the component; previously established sections that allow the generation of the main projections; the elements that compose them; a spreadsheet (with a brief report and main data about the component); two scripts on how to create a new component and how to configure the existing one; and some materials previously configured for application.

For more complex components, where there are many properties that allow the generation of several models from a single file, we began testing the possibility of creating macros that automate the generation of the different options, but this alternative is still under development (see file *Sideboard_R01.FCStd*).

In the same way as previously adopted, the files created were posted in a branch of the main FreeCAD library awaiting possible necessary revisions, after which they can be merged into the main library of said library:

https://github.com/Francisco-Rosa/FreeCAD-library/tree/master/Architectural%20Parts/Kitchen

https://github.com/Francisco-Rosa/FreeCAD-library/tree/master/Industrial%20Design/Appliances/Parametric

https://github.com/Francisco-Rosa/FreeCAD-library/tree/master/Architectural%20Parts/Bathroom

https://github.com/Francisco-Rosa/FreeCAD-library/tree/master/Architectural%20Parts/Living%20room

## 2. Procedures adopted

Similarly to those already presented, the four main procedural elements were:

• Implementation of a set of properties in the parameterization control;

• Arrangement of expressions structuring the geometry of the created components;

• Use of *Attachment* resources in object properties, allowing adjustments to the positions, angles, and dimensions of objects;

• Parametric objects structured by initial basic sketches.

Thus, the sketches of the created objects are structured by a basic established in the XY plane. Similar to the creation of ducts, the process is carried out by mapping these profiles using the *Map Mode* options of the *Attachment* of each created part. Basically, this allows the constructed component to automatically adapt to the new positioning (*Placement*) of the base sketch, relative to the x, y, z and rotation position variables. Further adjustments to the dimensions, materials and viewing options, and even mirroring of some elements, can be made through the component properties window.

## 3. Comments and next steps

As a point to highlight for the application of element repetition in the construction of some components, the *PathArray* tool was used instead of *Array*. Although the first one has a more complex composition than the second one, its application made it possible to change the positions and angles of the components without compromising their overall composition.

It also became clear that there is a range of more complex components, such as doors and windows, which can generate more than one final configuration or type. It would be interesting to be able to add automation of the possible types generated by means of macros, as previously mentioned. On the other hand, there are components that are much simpler with a defined final design that do not allow many or almost no changes in typology, such as a chair, for example. In these cases the parameterization will be much more restricted.

As the next step, we plan to develop components for the living room, dining room and bedrooms, initially using the strategy of single parametric files.

We will leave the necessary general review of the components for the fifth and final step, mainly doors and windows, in which we plan to derive the single file into individual files, according to each type created.