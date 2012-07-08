# ProcessWire Modules Fieldtype

## Fieldtype that stores reference to one or more other modules. 

This is similar to FieldtypeModule except that it stores multiple modules. It uses asmSelect to make the selection sortable/searchable.

### To install 

Copy to /site/modules/ and go to Admin > Modules > Check for new modules. 

### Usage notes

Note the configuration settings that appear on the details tab when creating a new field that uses this module. 

Lets say you created a field called my_modules that uses this Fieldtype. The value of your $page->my_modules will be a PHP array. 
When $page->outputFormatting is TRUE, the values of the array will be selected module objects. When output formatting is FALSE, 
the values will be module IDs (integers). Those IDs can be converted to either the module class name or an instance of the module using 
existing $modules API methods. 

