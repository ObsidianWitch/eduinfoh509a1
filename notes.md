% Project 1 : XML Schema Definition

# Links

## Naming conventions

* <https://stackoverflow.com/questions/1074447/case-conventions-on-element-names>
* <http://goo.gl/FZIee8>

There is no standard or recommendations regarding the naming of elements and
attributes. We should choose and stick to one style, it could be for example
PascaleCase for elements and camelCase for attributes.

## When to use elements VS attributes

* <http://www.ibm.com/developerworks/library/x-eleatt/>
* <https://stackoverflow.com/questions/152313/xml-attributes-vs-elements>
* <https://stackoverflow.com/questions/33746/xml-attribute-vs-xml-element>
* [ukgovtak - guidance for developers documents](http://goo.gl/bQ2YHs)

## Groups VS Base

* [Schema Design: Composition vs Subclassing](https://lists.w3.org/Archives/Public/xmlschema-dev/2002Apr/0016.html)

## Namespaces

* <http://www.liquid-technologies.com/Tutorials/XmlSchemas/XsdTutorial_04.aspx>

## Examples
* [books.xml](https://msdn.microsoft.com/en-us/library/ms764687(v=vs.85).aspx) &
[books.xsd](https://msdn.microsoft.com/en-us/library/ms256485(v=vs.110).aspx)

# Notes

* The Root element is called BookShop. We could also have called it Department
or BookShopDepartment, but the first name does not give enough information
(department of what?), while the second one might be too verbose.

* The ISBN is stored as a ISBNType which is a number on which restrictions have
been defined. The first restriction is a pattern checking if the number has 10
digits, while the second one checks if the number has 13 digits. One the
two restriction must be validated in order for the ISBN to be valid. An ISBN
also posseses groups separated by hyphens, but we do not store them neither
do we check groups.
