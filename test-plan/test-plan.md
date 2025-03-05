Test Plan: Klassisches Bausparen (Spartarif)

1. Objectives  
- Verify the functionality of the online calculator for the Klassisches Bausparen.  
- Validate calculated values for accuracy.  
- Ensure correct input validation (min/max values, negative numbers, invalid characters).  
- Check UI behavior under different input conditions.
- Confirm PDF download functionality works correctly.
- Check “Kontakt Aufnehmen” contact form

2. Scope  
- In-scope:  
  - Monthly contribution input (manual and slider).  
  - Dynamic contribution option (+5% annual increase).  
  - PDF download functionality. 
  - Contact form 
- Out-of-scope:  
  - Backend processing and API validation.
  - Mobile responsivness.   

3. Test Items  
- Input field (Sparbeitrag).  
- Slider for contribution selection.  
- "Berechnung als PDF herunterladen" button.  
- "Dynamische Sparvariante" checkbox.  

4. Test Approach  
- Manual testing for all features.  
- Positive tests: 
  • Valid inputs: 40–13.888 EUR (monthly contribution), 480–166,666 EUR (yearly contribution), 2.880–1,000,000 EUR (one-time contribution)
  • Using the slider vs. manual input entry
  • Checking calculations with and without the dynamic savings option enabled.  
- Negative tests: 
  • Out-of-range values (below 40 EUR, above 13,888 EUR)
  • Negative numbers (-100 EUR input)
  • Invalid characters (letters, symbols, spaces)
  • Zero input (should be rejected)
  • Rapid input changes (checking UI glitches or lag) 

5. Environment:
- Browser: Chrome v133
- OS: Windows 10

6. Risks & Assumptions  
- Risks: 
  • Slow PDF generation. 
  • UI inconsistencies on rapid input changes. 
- Assumptions: 
  • Tested primarily on Chrome v133, but should also be checked on Firefox and Edge.
  • Mobile responsiveness is not in scope unless explicitly requested.
