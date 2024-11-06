 specifications for the traffic light state machine model:

Initial State:

The system starts in the Red state.
Main Transitions:

Red → Green: Transition occurs when the timer expires.
Green → Yellow: Transition occurs when the timer expires.
Yellow → Red: Transition occurs when the timer expires, completing a cycle.
Red State:

SteadyRed: Default sub-state for Red.
FlashingRed: Activated when a power failure is detected.
Transition Back to SteadyRed: Occurs when power is restored.
Green State:

SteadyGreen: Default sub-state for Green.
FlashingGreen: Activated when a pedestrian crossing request is detected.
Transition Back to SteadyGreen: Occurs after the pedestrian has crossed.
Yellow State:

SteadyYellow: Default sub-state for Yellow.
FlashingYellow: Activated when an emergency vehicle is detected.
Transition Back to SteadyYellow: Occurs after the emergency vehicle has passed.
