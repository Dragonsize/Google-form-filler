# Google-form-filler
A Tampermonkey / Violentmonkey userscript that lets you quickly fill out Google Forms manually using a hotkey and popup input box. Supports various answer formats such as numbers or letters (e.g., 123, 1 2 3, A B C, etc.).

Google Form Manual Filler Toggle Popup

A Tampermonkey / Violentmonkey userscript that lets you quickly fill out Google Forms manually using a hotkey and popup input box.
Supports various answer formats such as numbers or letters (e.g., 123, 1 2 3, A B C, etc.).

 Features

Smart Parsing — accepts answers in multiple formats:
123, 1 2 3, 1,2,3, ABC, A B C, A,B,C

 Hotkey Toggle — open or close the popup with Ctrl + Shift + F

Compact Popup UI — easily enter and submit answers

 Auto-Click Radio Options — automatically selects choices in order

 Console Summary — prints a clickable report for review

 Installation

Install a userscript manager:

Tampermonkey (Chrome / Edge)

Violentmonkey (Firefox / Opera)

Create a new script and paste in the full code from Google Form Manual Filler Toggle Popup
.

Save it — the script will automatically run on any Google Form URL (https://docs.google.com/forms/*).

 Usage

Open a Google Form.

Press Ctrl + Shift + F to open or close the popup.

Enter your answers:

123
1 2 3
1,2,3
ABC
A B C
A,B,C


Click “Fill Form” — the script will:

Click the corresponding option for each question.

Show results in the console (press F12 → Console).

 You must submit the form manually — the script only fills it.

 How It Works

The script looks for all question groups (div[role="radiogroup"]).

Each answer corresponds to the nth option (A=1, B=2, etc.).

It simulates a click for each matched option.

Non-existent answers are logged as ❌ in the console.

 Hotkey
Action	Keys
Toggle popup	Ctrl + Shift + F
Developer Notes

Written in plain JavaScript, no external libraries.

Uses minimal DOM manipulation for lightweight execution.

Tested on the latest Google Forms layout (as of 2025).
                          





cational use.
