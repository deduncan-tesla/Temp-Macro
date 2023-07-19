```
                     Workbench Incident Template Macros
   https://github.com/deduncan-tesla/eTicketing-Template-Macro/releases/latest/
                              Devan Duncan
                        Rev. 2023.07.18 (v1.0.1.8)
```

NEW IN 1.0.1.8:
-  If already open, hotkey restores instead of relaunch
-  Menu will remember last position if it reopens (unless closed by user)
-  Hotfix for HTML editor link for Email templates not working
-  Hotfix for Delete confirmation
-  Hotfix for HTML editor using `<em>` instead of `<i>` for italics
-  Hotfix for invisible unicode chars coverting to "???????" in HTML templates

NEW IN 1.0.1.7:
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
-  First-run installer (check for Data folder, if not present prompt for install location, then download newest version into target directory and run)
