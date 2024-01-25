# flutter_isolate

A new Flutter Isolate Example.

## Getting Started

In this example:

- We create a Flutter app with a simple MyHomePage widget.
- Inside the widget's state, we use Isolate.spawn to start a new isolate running the _isolateEntryPoint function.
- The _isolateEntryPoint function runs in a separate isolate and sends counter values to the main isolate using the sendPort.
- The main isolate listens to the ReceivePort for messages from the spawned isolate and updates the UI with the received counter value.
- We use a Timer in the spawned isolate to simulate some background task.
- This example demonstrates the basic usage of Flutter isolates to perform concurrent tasks in a separate isolate and update the UI accordingly.
