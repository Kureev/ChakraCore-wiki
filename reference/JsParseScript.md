Parses a script and returns a function representing the script. 
### Syntax 
```
STDAPI_(JsErrorCode)
    JsParseScript(
    _In_z_ const wchar_t *script,
    _In_ JsSourceContext sourceContext,
    _In_z_ const wchar_t *sourceUrl,
    _Out_ JsValueRef *result);
```
### Parameters 
* __script__: The script to parse.
* __sourceContext__:  A cookie identifying the script that can be used by debuggable script contexts.
* __sourceUrl__: The location the script came from.
* __result__: A function representing the script code.

### Return Value 
The code **JsNoError** if the operation succeeded, a failure code otherwise.
### Remarks 
Requires an active script context.
