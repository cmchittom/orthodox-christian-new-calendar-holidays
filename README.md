# orthodox-christian-new-calendar-holidays
Package to add Orthodox Christian (new calendar) holidays to Emacs

## Commentary
Although the Orthodox Churches of Jerusalem, Russia, Serbia, Ukraine,
and Georgia continue to use the Julian calendar both for the Paschal
cycle and for fixed feasts, the other Orthodox Churches follow the
Revised Julian calendar for fixed feasts but use the original Julian
Paschalion. So *strictly* speaking, using `holiday-fixed` is
incorrect, but since the Revised Julian is exactly the same as the
Gregorian until 2800 AD (when a difference in the leap year rule will
make them diverge) I think that's a problem for someone else on
another day.

This is all fairly trivial, but putting it in a separate file gets
it out of my `~/.emacs` and makes it available if anyone else finds
it useful. 

## Usage
```
(setq holiday-bahai-holidays nil
      holiday-christian-holidays nil
      holiday-islamic-holidays nil) ;; Or whatever else you don't want included
(setq calendar-holidays (append calendar-holidays holiday-orthodox-christian-new-calendar-holidays))
```
