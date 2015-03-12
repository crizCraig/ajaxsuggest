This is an example of how to create an AJAX suggest box front-end without using any javascript libraries. The code was originally written for Spyfu.com and uses the same back-end to serve suggestions as Spyfu does. This back-end uses a C# dictionary to serve quick in-RAM lookups.

Features:
  * Maintains one selected item whether pressing arrow  or mousing over.
  * Hides suggestions when clicking outside box or pressing escape.

Areas of potential improvement include:
  * Better handling of pressing the escape. Currently, this can cause the input box to flash text that was previously typed.
  * Change the selected item on key down rather than key up. The AJAX request won't work on key down, but the selection can probably be separated from the request. This will allow holding down the up or down arrow to scroll through suggested items more quickly.