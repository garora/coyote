---
layout: reference
section: learn
title: StartPeriodicTimer
permalink: /learn/ref/Microsoft.Coyote.Actors/Actor/StartPeriodicTimer
---
# Actor.StartPeriodicTimer method

Starts a periodic timer that sends a [`TimerElapsedEvent`](../../Microsoft.Coyote.Actors.Timers/TimerElapsedEventType) to this actor after the specified due time, and then repeats after each specified period. The timer accepts an optional payload to be used during timeout. The timer can be stopped by invoking the [`StopTimer`](StopTimer) method.

```csharp
protected TimerInfo StartPeriodicTimer(TimeSpan startDelay, TimeSpan period, 
    TimerElapsedEvent customEvent = null)
```

| parameter | description |
| --- | --- |
| startDelay | The amount of time to wait before sending the first timeout event. |
| period | The time interval between timeout events. |
| customEvent | Optional custom event to raise instead of the default TimerElapsedEvent. |

## Return Value

Handle that contains information about the timer.

## Remarks

See [Using timers in actors](/coyote/learn/programming-models/actors/timers) for more information.

## See Also

* class [TimerInfo](../../Microsoft.Coyote.Actors.Timers/TimerInfoType)
* class [TimerElapsedEvent](../../Microsoft.Coyote.Actors.Timers/TimerElapsedEventType)
* class [Actor](../ActorType)
* namespace [Microsoft.Coyote.Actors](../ActorType)
* assembly [Microsoft.Coyote](../../MicrosoftCoyoteAssembly)

<!-- DO NOT EDIT: generated by xmldocmd for Microsoft.Coyote.dll -->
