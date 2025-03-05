Bug Reports

Bug 1: Incorrect Default Value  
- Steps to Reproduce:  
  1. Open the calculator for Klassisches Bausparen.  
  2. Observe the default value in "Sparbeitrag"  
- Expected: Default = 40 EUR (minimum)
- Actual: Default = 100 EUR 
- Severity: Medium (mislead users and affect correct usage of the calculator)
- Environment: Chrome 133, Windows 10 
- Screenshot: Screenshot-1, Screenshot-2, Screenshot-3 

Bug 2: Negative Input Allowed  
- Steps:  
  1. Open the calculator for Klassisches Bausparen. 
  2. Enter "-100" in the "Sparbeitrag" field.  
- Expected: Negative values should be immediately blocked.
- Actual: System accepts negative values with an error message.  
- Severity: High (Even with an error message, allowing negative input can lead to unintended errors)
- Environment: Chrome 133, Windows 10 
- Screenshot: Screenshot-5

Bug 3: Negative Postal Code
- Steps:  
  1. Open the calculator for Klassisches Bausparen. 
  2. Click on Kontakt Aufnehmen
  3. Click on "Andern".  
  4. Enter "-1234" in the "Postleitzahl" field.  
  5. Attempt to submit.  
- Expected: Error: "Postal code must be positive." The input field should immediately prevent invalid values.
- Actual: System loads negative values without at least an error message.
- Severity: High (the system does not provide any feedback)
- Environment: Chrome 133, Windows 10 
- Screenshot: Screenshot-4

Bug 4: UI Glitch on Input Change  
- Steps to Reproduce:  
  1. Open the calculator for Klassisches Bausparen.  
  2. Enter a valid value (e.g., 100) in the "Sparbeitrag" field.  
  3. Immediately change it to another valid value (e.g., 200).  
- Expected:  
  - Smooth transition to the new value without intermediate resets.  
- Actual:  
  - UI briefly resets all values to 0 before displaying the updated calculation.  
  - Example: "Summe der Einzahlungen" flashes 0.00 EUR before showing 14,400.00 EUR.  
- Severity: Medium (does not impact functionality, but can reduce trust in the tool).  
- Environment: Chrome 133, Windows 10  
- Screenshot: Video-1  