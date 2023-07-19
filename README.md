```
                     Workbench Incident Template Macros
   https://github.com/deduncan-tesla/eTicketing-Template-Macro/releases/latest/
                              Devan Duncan
                        Rev. 2023.07.18 (v23.07.18.00)
```

NEW IN v23.07.18.00:
-  Script will check for existing Data folder on startup; if not found, user will be prompted to select an install location. Script will then download latest version into that directory and remove downloaded file.

NEW IN v23.07.17.00:
-  If already open, hotkey restores instead of relaunch
-  Menu will remember last position if it reopens (unless closed by user)
-  Hotfix for HTML editor link for Email templates not working
-  Hotfix for Delete confirmation
-  Hotfix for HTML editor using `<em>` instead of `<i>` for italics
-  Hotfix for invisible unicode chars coverting to "???????" in HTML templates

NEW IN v23.07.16.00:
-  Email Templates! You can now create bulk email templates with variables.
-  Text filtering for tabs
-  Smoother menu scrolling (less flickering)
-  More persistent UI elements & less empty space
-  Link to Github repo/releases on Options tab
-  Option to skip SupplierData update (not recommended)
-  On-launch script to condense all TicketLog.csv files & remove duplicates
-  Clicking "Send Response" automatically opens HTML editor
-  General code cleanup

FEATURES:
-  Uses DOM to fill out workbench incidents, can also pull information from them
-  Can send emails and insert HTML and attachments into them
-  Can paste text blocks (including rich text)
-  Can close bulk tickets using iterative loops
-  Can bulk send email templates with dynamic variables

NOTES:
-  Update version whenever making a new release
-  When setting an HTML string as a variable, always use &apos; for apostrophes and escape % with tilde (i.e. ``P2P`%20Portal`%20-`%20Indirect`%20Invoicing.pdf``)
-  Be careful when adjusting Sleep delays; most of them are there for a reason

TODO:
-  MAYBE Add manual variables for templates (i.e. [PrimaryContact] to pull in supplier primary contact) (Already added for bulk email templates)
-  More error handling everywhere
-  Error handling for missing attachments
-  Workbench attachments
-  Detect new Ticketing, switch back to eTicketing
-  Error for PowerBI access missing - localparam to disable supplier search
