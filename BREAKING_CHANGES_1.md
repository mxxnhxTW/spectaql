Here is a (hopefully) exhaustive list of the breaking changes between pre `1.0.0` versions and `1.0.0`:

- `introspection.typesDocumented` option renamed to `introspection.objectsDocumentedDefault`.
- `introspection.typeDocumentedDefault` option renamed to `introspection.objectDocumentedDefault`
- `introspection.hideFieldsWithUndocumentedReturnType` option was renamed to `introspection.hideFieldsOfUndocumentedType`.
- `info.x-swaggerUrl` renamed to `x-url`
- The "Dynamic Example Generators" has been completely re-worked. If used, your module is now expected to export a single function. That function will be provided all the information it should need to what it is, where it's being used, and what you'd like to return as an example value. Check out `examples/customizations/examples/index.js` for more information.
- The `customizations/` folder has been removed and the black magic that used to exist there is gone. If you want to customize your CSS, for now use the `spectaql.additionalCssFile` option.
