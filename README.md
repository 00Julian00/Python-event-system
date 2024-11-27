# Python-event-system
A C# inspired event system implementation in python

How to use:
- Call `define_event()` to create a new event.
- Call `subscribe()` to subscribe to an event. For that, you need to parse a callable that will be called when the event is called.
- Call `unsubscribe()` to unscubscribe from an event.
- Call `ìs_subscribed()` to check wether a callable is subscribed to an event.
- Call `event_exists()` to check wether an event exists.
- Call `trigger_event()` to trigger an event. If this happens, all callables that are subscribed to that evemt will be called.

Attempting to interact with an event that doesn't exist will raise an Exception. Attempting to create an event that already exists will raise an Exception.
