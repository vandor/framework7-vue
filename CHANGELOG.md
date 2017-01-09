# Change Log

## Framework7 Vue v0.7.5 - Updated on January 9, 2017
  * Added methods for many components:
    * Popup, Login Screen, Picker Modal, Panel, Action Sheet, Popover:
      * .open() - open modal/panel
      * .close() - open modal/panel
    * Navbar, Toolbar:
      * .hide() - hide navbar/toolbar
      * .show() - show navbar/toolbar
      * .size() - size navbar
    * Progress bar:
      * .set(progress, duration) - set progress bar progress
      * .show(container, progress, color) - show progress bar in specified container
    * Tab
      * .show() - show tab
    * Search Bar:
      * search(query) - Force searchbar to search passed query
      * enable() - Enable/activate searchbar
      * disable() - Disable/deactivate searchbar
      * clear() - Clear search query and update results
    * Message Bar:
      * value(newValue) - Set messagebar textarea value/text. Or return messagebar textarea value if newValue is not specified
      * clear() - Clear textarea and update/reset its size
    * Messages:
      * addMessage(messageParameters, method, animate) - Add new message to the end or to the beginning depending on method parameter
      * appendMessage(messageParameters, animate) - Add new message to the end (to the bottom)
      * prependMessage(messageParameters, animate) - Add new message to the beginning (to the top)
      * addMessages(messages, method, animate) - Add multiple messages per once
      * removeMessage(message) - Remove message
      * removeMessages(messages) - Remove multiple messages
      * scrollMessages() - Scroll messages to top/bottom depending on newMessagesFirst parameter
      * layout() - Apply messages auto layout
      * clean() - Clean/remove all the messages
  * Added `start` and `end` slots for Message (f7-message) component
  * New boolean `hidden` prop for Navbar and Toolbar
  * Fixed issues with infinite scroll not being working when specified as boolean attribute, e.g. just `infinite-scroll`
  * New `input` attributes to match native attributes `autocorrect`, `autocapitalize`, `spellcheck`
  * New `link-target` attribute for List Item components to specify link's target attribute
  * Fixed issues with openinig/closing modals (Popup, Login Screen, Picker, Actions) that stopped working after first open/close
  * Minor fixes