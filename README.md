# test-task-for-gsoft

## What was the problem?
Small task to speed up that slow code from: http://gsoft-test.jsin.ru/test1.html
It contains lots of unnecessary concatenations and DOM-queries that were removed.
jQuery was also replaced with VanillaJS, helper object for DOM manipulations also created

All the inserts are now into: `document.createDocumentFragment();`, not into real DOM
The nodes are not created but cloned, as well.
