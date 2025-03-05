Test Cases for Klassisches Bausparen

Field	Description
• Test Case ID: TC-001
• Test Case Name:	Default Value in Sparbeitrag Field
• Description: Ensures that the calculator starts with the correct default savings amount.
• Preconditions: The calculator is open for Klassisches Bausparen.
• Test Data: Default system-generated value.
• Execution Steps:	
  1. Open the calculator.
  2. Observe the default value in the "Sparbeitrag" field..
• Expected Result: The default value should be 40 EUR (minimum required contribution)..
• Actual Result: 100 EUR is set as default instead of 40 EUR.
• Status:	Fail
• Bug Reference: Bug 1: Incorrect Default Value

• Test Case ID: TC-002
• Test Case Name:	Negative Value Entry in "Sparbeitrag"
• Description: Ensures that the input field properly rejects negative values.
• Preconditions: The calculator is open for Klassisches Bausparen.
• Test Data: -100 EUR
• Execution Steps:
  1. Enter -100 in the "Sparbeitrag" field.
  2. Click outside the field.
  3. Observe system response and UI behavior.
• Expected Result: The system should immediately block negative input. The value should either reset to the last valid input or remain empty.
• Actual Result: The system accepts the negative value and shows an error message instead of blocking the input.
• Status: Fail
• Bug Reference: Bug 2: Negative Input Allowed

• Test Case ID: TC-003
• Test Case Name: Negative Postal Code Entry
• Description: Ensures that the postal code field does not accept negative values.
• Preconditions: The user is on the contact page.
• Test Data: -1234
• Execution Steps:
  1. Click "Kontakt Aufnehmen".
  2. Click "Andern".
  3. Enter "-1234" in the "Postleitzahl" field.
  4. Attempt to submit.
• Expected Result: The system should display an error message: "Postal code must be positive." The input field should immediately reject negative values. The system should have feedback after loading state.
• Actual Result: The system allows negative values and does not display any error message. Instead, it shows a loading icon but does nothing.
• Status: Fail
• Bug Reference:	Bug 3: Negative Postal Code

• Test Case ID: TC-004
• Test Case Name: UI Reset Issue on Rapid Input Change
• Description: Ensures that the UI handles rapid input changes correctly without resetting calculations.
• Preconditions: The calculator is open for Klassisches Bausparen.
• Test Data: 100 - 200 EUR (rapid input change)
• Execution Steps: 
  1. Enter 100 in the "Sparbeitrag" field.
  2. Immediately change it to 200.
  3. Observe the displayed calculation results.
• Expected Result: The transition should be smooth, without briefly resetting values to 0.
• Actual Result: The UI briefly resets all values to 0 before displaying the updated calculation.
• Status: Fail
• Bug Reference:	Bug 4: UI Glitch on Input Change

• Test Case ID: TC-005
• Test Case Name: PDF Download Validation
• Description: Ensures that the PDF download functionality works correctly and contains accurate data.
• Preconditions: Calculator has valid input.
• Test Data: 500
• Execution Steps:
  1. Enter 500 in the "Sparbeitrag" field.
  2. Click "Berechnung als PDF herunterladen".
  3. Open the downloaded PDF.
• Expected Result: The PDF contains accurate data.
• Actual Result: The PDF is downloaded and contains accurate data.
• Status: Pass
• Bug Reference: N/A

• Test Case ID: TC-006
• Test Case Name: Slider-Manual Input Synchronization
• Description: Ensures that the slider and manual input field stay synchronized.
• Preconditions: The calculator is open for Klassisches Bausparen.
• Test Data: 500 EUR (slider), 700 EUR (manual input)
• Execution Steps:
  1. Move the slider to 500 EUR.
  2. Verify the value in the "Sparbeitrag" field.
  3. Manually enter 700 in the "Sparbeitrag" field.
  4. Verify the slider position.
• Expected Result: The slider and manual input field stay synchronized.
• Actual Result: The slider and manual input field stay synchronized.
• Status: Pass
• Bug Reference: N/A

• Test Case ID: TC-007
• Test Case Name: Invalid Characters in Sparbeitrag
• Description: Ensures that the "Sparbeitrag" field rejects invalid characters (e.g., letters, symbols).
• Preconditions: The calculator is open for Klassisches Bausparen.
• Test Data: abc!@#
• Execution Steps:
  1. Enter "abc!@#" in the "Sparbeitrag" field.
  2. Click outside the field.
• Expected Result: The system should display an error message: "Dozvoljeni su samo brojevi."
• Actual Result: The system displays an error message: "Dozvoljeni su samo brojevi."
• Status: Pass
• Bug Reference: N/A

