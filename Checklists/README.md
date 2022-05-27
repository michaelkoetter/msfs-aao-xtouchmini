# AAO Checklists

## Prerequisites

These checklist scripts assume that AAO speech recognition is setup and configured for English language. Please refer to AAO documentation for more details.

You might need to install an English language pack in Windows.

The checklists also assume that Text-to-speech is available and that an English voice is set as default. This can be achieved with a global one-shot script like this: 

Female voice:
```
(VOICE:Microsoft Zira Desktop)
(SPEAK:TTS Ready)
```

Male voice:
```
(VOICE:Microsoft David Desktop)
(SPEAK:TTS Ready)
```

## Checklist Scripts

The checklist scripts files (`*_CL.txt`) need to be copied to `%USERPROFILE%\Documents\LorbyAxisAndOhs Files\Scripts`.

## AAO Template

Import the template file `A320_CHECKLISTS.tmpl` into AAO and apply it to your aircraft config.

## Checklist Execution

The template contains voice commands to start the checklist, ie. just say ***"before start checklist"*** to run the checklist.

There is one command to advance the checklist which covers all standard answers like ***"checked"***, ***"set"*** etc:

- checked
- check
- set
- on
- off
- continue
- completed
- removed
- on auto
- nav
- closed
- idle
- zero
- confirmed
- notify
- takeoff no blue
- advised
- normal
- up
- retracted
- standard set
- speed
- landing no blue

> Note: my speech recognition sometimes doesn't recognize when I say ***"on"***. If a command is not recognized (ie. checklist doesn't advance), just use another one - ***"checked"*** seems to work almost 100%.

## Stop Checklist

You can say ***"stop checklist"*** anytime to abort checklist execution.