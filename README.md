# README

## Installation

```
npm install --save touch-dnd-custom-events
```

## Usage
```
import setupTouchDNDCustomEvents from 'touch-dnd-custom-events'

setupTouchDNDCustomEvents()
```

Once the initial setup function is called (`setupTouchDNDCustomEvents()`), touch events (`touchstart` on draggable html elements, `touchmove` during a drag, `touchend` during a drag)  are intercepted and dispatch custom drag and drop events with the same datatransfer interface as html 5 drag and drop events (see https://html.spec.whatwg.org/multipage/interaction.html#datatransfer for details).

The custom event names are as follows.

  * touchdragstart (equivalent of html5 dragstart)
  * touchdrag (equivalent of html5 drag)
  * touchdragenter (equivalent of html5 dragenter)
  * touchdragleave (equivalent of html5 dragleave)
  * touchdrop (equivalent of html5 drop)
  * touchdragend (equivalent of html5 dragend)

Because these custom events have the same interface as html5 drag and drop events, they can be treated the same way as a normal html 5 drag and drop event.

## License

MIT
