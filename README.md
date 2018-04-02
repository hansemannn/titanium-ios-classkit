# Titanium ClassKit

Use the iOS 11.4+ ClassKit API's with Titanium and Hyperloop.

## Example

```js
import { CLSDataStore } from 'ClassKit';

// Activate Contexts When Users Begin Tasks
CLSDataStore.shared.descendantMatchingIdentifierPathCompletion:['path', 'to', 'section'], (context, error) => {
  context.becomeActive();
});

// Deactivate Contexts When Users Finish
CLSDataStore.shared.descendantMatchingIdentifierPathCompletion:['path', 'to', 'section'], (context, error) => {
  context.resignActive();
});
```

## License

MIT

## Author

Hans Knöchel
