# SimpleModern Starter Kit (SMSK)

SimpleModern is a barebone canvas Power App in the tablet/web form factor, designed to serve as a highly reusable starting point that minimises the ad-hoc nature of user-interface construction overheads.

For context, read [this article](https://jkflipflop.medium.com/2a474ffefb11) then [this article](https://jkflipflop.medium.com/05b15ac5c225).

## Highlights

+ An uncluttered look and feel for effective delivery of content, inspired by the Microsoft 365 back-end admin functions
+ A screen-specific menu structure that can be collapsed and expanded on demand
+ Any number of items in the menu (although a maximum of 6 or 7 per screen is recommended)
+ Full use of the user's screen real estate with no letterboxing or wasted space
+ Built for modern themes
+ Support for Microsoft 365-style modal dialogues
+ Scrollable content and modal dialogue panes

Screenshots are available.

## Instructions

Download *SimpleModern-Starter.zip* and import it to a Power Platform environment as a new canvas app. Then, follow further instructions on MainScreen.

## Change log

+ 1.1.12 (2025-01-23): Minor positioning errors corrected, following the last round of updates
+ 1.1.11 (2025-01-21):
  + Clicking on the primary button inside a modal gives a clear "Processing..." indication while processing whatever it is instructed to fulfil. This is a critical UI provision as most user-initiated CRUD operations take place in a modal. The message can be customised or be made blank depending on the nature of the modal.
  + Given the increasing adoption of ultrawide monitors, there is now a convenient way to set the maximum content width in order to prevent content from uncontrollably stretching across the entire screen, thereby ensuring a better-composed look. In App.OnStart, two new UI constants handle this behaviour: ui.CanvasWidth (integer) and ui.ForceFullScreenWidth (boolean).
+ 1.1.10 (2025-01-18): Explicitly set the VerticalAlign property of pagination text controls to "Middle" for alignment with other UI elements. The default VerticalAlign behaviour of modern text controls, unless explicitly set, appears to have changed from Middle to Top. No other changes or fixes.
+ 1.1.9 (2024-12-12): Tabular data previous/next page navigation functions now prevent rage clicks.
+ 1.1.8 (2024-12-11): Further usability and UI fine-tuning
+ 1.1.7 (2024-12-03):
  + Fixed the bug where pagination parameters could be set incorrectly upon user-supplied keyword search.
  + Additional in-line comments
+ 1.1.6 (2024-12-02): Further usability fine-tuning, particularly around the AccessibleLabel and DisplayMode behaviours of controls for consistency
+ 1.1.5 (2024-11-30): More usability fine-tuning
+ 1.1.4 (2024-11-23):
  + Added styled example combobox, dropdown, checkbox, radio, and toggle controls for quick templating.
  + Miscellaneous usability and portability improvements
+ 1.1.3 (2024-11-20): Better consistency and succinctness in variable names; navigating to RoutingScreen for user-initiated resets and restarts now correctly redirects the user to the app's default fallback menu item, plus room for implementing custom routing logic.
+ 1.1.2 (2024.11-18): In App.OnStart, there is an on/off flag for an explicit exit-app button (vApp.EnableExitButton), which may improve usability when launching the app on a handheld device.
+ 1.1 (2024-11.15): Menu items have been globalised to make it easy for the app to implement a consistent menu structure or its variations across multiple screens. Based on the single source of truth, each individual screen can render just the menu items that are applicable to it.
+ v1.0.9 (2024-11-06): Miscellaneous usability and portability improvements
+ v1.0.7 (2024-11-04): Improved the repeatable search function on tabular data with modern controls and visual cues where results follow keypresses in the search box whose output trigger is set to Delayed.
+ v1.0.6 (2024-11-03):
  + Simplified UI constants for more consistent application of attributes.
  + Added a repeatable example of rendering tabular data, complete with search and pagination functions.
  + Alignment/positioning/spacing fixes and adjustments
+ v1.0.1 (2024-11-01): Removed redundant border colours in rectangle controls.
+ v1.0.0 (2024-10-28): Initial release
