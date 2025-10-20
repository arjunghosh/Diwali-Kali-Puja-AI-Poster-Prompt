# 🧪 Script Validation Test - Diwali AI Poster Generator v2.10

**Purpose**: Virtual testing of the script to ensure it runs properly in ChatGPT and Gemini AI

**Date**: October 20, 2024  
**Version**: 2.10

---

## ✅ Test 1: System Prompt & Immediate Start

**Expected Behavior**:
- AI should immediately start Q&A when file is loaded
- Should NOT wait for additional user input
- Should greet user and ask platform selection

**Test Query**: "Load and run this script"

**Expected Output**:
```
Hello! Which AI platform? **A. ChatGPT/Copilot** **B. Gemini**
```

**Status**: ⏳ To be tested

---

## ✅ Test 2: Platform Selection (Q1)

### Test 2A: ChatGPT/Copilot Selection
**Input**: "A"

**Expected Behavior**:
- Set title to "Personalized Festival Poster"
- Say: "Great! I'll ask 8 questions to create your poster."
- Ask Q2 (Festival)

**Status**: ⏳ To be tested

### Test 2B: Gemini Selection
**Input**: "B"

**Expected Behavior**:
- Set title to "Festival Poster Design"
- Say: "Great! I'll ask 8 questions to build your prompt."
- Ask Q2 (Festival)

**Status**: ⏳ To be tested

---

## ✅ Test 3: Festival Selection (Q2)

### Test 3A: Both Festivals
**Input**: "A"

**Expected Behavior**:
- Load BOTH presets
- Set {SELECTED_GREETING_1} = "Happy Diwali (शुभ दीपावली)"
- Set {SELECTED_GREETING_2} = "Happy Kali Pujo (শুভ কালী পূজा)"
- Set {SELECTED_ELEMENTS} = BOTH_ELEMENTS
- Set {SUG_COLOR} = "Festive Maroon/Deep Red"
- Set {OPT_COLOR_B} = "Deep Midnight Blue"
- Set {OPT_COLOR_C} = "Royal Purple"
- Set {OPT_COLOR_D} = "Rich Orange"
- Set {OPT_COLOR_E} = "Deep Green"
- Set {OPT_COLOR_F} = "Elegant Gold"
- Set {SUG_ACCENT} = "Glittering Gold/Silver"
- Set {OPT_ACCENT_B} = "Bright Orange/Red"
- Set {OPT_ACCENT_C} = "Emerald Green/Gold"
- Set {OPT_ACCENT_D} = "Purple/Magenta"
- Set {OPT_ACCENT_E} = "Copper/Bronze"
- Ask Q3 (Identity)

**Status**: ⏳ To be tested

### Test 3B: Diwali Only
**Input**: "B"

**Expected Behavior**:
- Load DIWALI presets
- Set {SELECTED_GREETING_1} = "Happy Diwali (शुभ दीपावली)"
- Set {SELECTED_ELEMENTS} = DIWALI_ELEMENTS (with people)
- Ask Q3 (Identity)

**Status**: ⏳ To be tested

### Test 3C: Kali Puja Only
**Input**: "C"

**Expected Behavior**:
- Load KALI_PUJA presets
- Set {SELECTED_GREETING_1} = "Happy Kali Pujo (শুভ কালী পূজা)"
- Set {SELECTED_ELEMENTS} = KALI_PUJA_ELEMENTS (with Ma Kali)
- Ask Q3 (Identity)

**Status**: ⏳ To be tested

---

## ✅ Test 4: Identity Selection (Q3)

### Test 4A: Person Name
**Input**: "A" then "Priya"

**Expected Behavior**:
- Set {NAME} = "Priya"
- Ask Q4 (Primary Color)

**Status**: ⏳ To be tested

### Test 4B: Anonymous
**Input**: "B"

**Expected Behavior**:
- Set {NAME} = "Anonymous"
- Ask Q4 (Primary Color)

**Status**: ⏳ To be tested

### Test 4C: Company/Team
**Input**: "C" then "ABC Corp"

**Expected Behavior**:
- Set {NAME} = "ABC Corp"
- Ask Q4 (Primary Color)

**Status**: ⏳ To be tested

---

## ✅ Test 5: Primary Color (Q4)

**Input**: "A" (Recommended color)

**Expected Behavior**:
- Should show the recommended color from preset
- Should show all 6 color options + Custom
- Each option on separate line (for Gemini compatibility)
- Ask Q5 (Accent Colors)

**Status**: ⏳ To be tested

---

## ✅ Test 6: Accent Colors (Q5)

**Input**: "A" (Recommended accent)

**Expected Behavior**:
- Should show the recommended accent from preset
- Should show all 5 accent options + Custom
- Each option on separate line
- Ask Q6 (Art Style)

**Status**: ⏳ To be tested

---

## ✅ Test 7: Art Style (Q6)

**Input**: "A" (Traditional Indian Folk Art)

**Expected Behavior**:
- Should show all 5 art style options
- Each option on separate line
- Ask Q7 (Regional Style)

**Status**: ⏳ To be tested

---

## ✅ Test 8: Regional Style (Q7)

### Test 8A: Yes with Style
**Input**: "A" then "Bengali Alpana"

**Expected Behavior**:
- Validate input (max 50 chars)
- Store regional style
- Ask Q8 (Signature)

**Status**: ⏳ To be tested

### Test 8B: No
**Input**: "B"

**Expected Behavior**:
- Skip regional style
- Ask Q8 (Signature)

**Status**: ⏳ To be tested

---

## ✅ Test 9: Signature (Q8) - Conditional Logic

### Test 9A: Anonymous User (Q3=B)
**Expected Behavior**:
- Should ask: "Would you like to add a signature to your poster?"
- Options:
  - A. Add a simple festive message (e.g., 'Happy Diwali!')
  - B. Add a personalized message (e.g., 'With love, from all of us')
  - C. No signature

**Input**: "A"

**Status**: ⏳ To be tested

### Test 9B: Person User (Q3=A, NAME="Priya")
**Expected Behavior**:
- Should ask: "How should your name 'Priya' appear on the poster?"
- Options:
  - A. Use name as-is
  - B. Use name with a message (e.g., 'With love, Priya')
  - C. No signature

**Input**: "B"

**Status**: ⏳ To be tested

### Test 9C: Company User (Q3=C, NAME="ABC Corp")
**Expected Behavior**:
- Should ask: "How should your name 'ABC Corp' appear on the poster?"
- Options:
  - A. Use name as-is
  - B. Use name with a message (e.g., 'With love, ABC Corp')
  - C. No signature

**Input**: "A"

**Status**: ⏳ To be tested

---

## ✅ Test 10: Final Generation (ChatGPT/Copilot)

**Platform**: ChatGPT/Copilot  
**Input**: Complete all 8 questions

**Expected Behavior**:
1. Update title to "Creating {SELECTED_GREETING} poster for {NAME}"
2. Say: "Thank you, {NAME}! Here's your poster."
3. Generate image with proper prompt including:
   - Core Theme
   - Visual Elements (with mandatory elements)
   - Color Palette
   - Art Style
   - Signature (conditional based on Q8)
   - Mood

**Status**: ⏳ To be tested

---

## ✅ Test 11: Final Prompt (Gemini)

**Platform**: Gemini  
**Input**: Complete all 8 questions

**Expected Behavior**:
1. Update title to "Final Prompt for {NAME}"
2. Say: "Thank you, {NAME}! Copy this prompt and paste it back:"
3. Provide formatted prompt with:
   - PROMPT START
   - Core Theme
   - Visual Elements (with mandatory elements)
   - Color Palette
   - Art Style
   - Signature (conditional based on Q8)
   - Mood
   - PROMPT END
4. Instructions to paste back

**Status**: ⏳ To be tested

---

## ✅ Test 12: Mandatory Visual Elements

### Test 12A: Diwali Only
**Expected in Elements**:
- People celebrating Diwali (families lighting diyas, children playing, festive gatherings)

**Status**: ⏳ To be tested

### Test 12B: Kali Puja Only
**Expected in Elements**:
- Ma Kali's face with red tongue and divine expression (prominent)

**Status**: ⏳ To be tested

### Test 12C: Both Festivals
**Expected in Elements**:
- People celebrating Diwali
- Ma Kali's face with red tongue (minimum shown)

**Status**: ⏳ To be tested

---

## ✅ Test 13: Input Validation

### Test 13A: Custom Color Too Long
**Input**: "This is a very long custom color name that exceeds fifty characters"

**Expected Behavior**:
- Reject with: "Please keep under 50 characters."
- Ask again

**Status**: ⏳ To be tested

### Test 13B: Custom Color Valid
**Input**: "Deep Crimson"

**Expected Behavior**:
- Accept (under 50 chars)
- Continue to next question

**Status**: ⏳ To be tested

---

## ✅ Test 14: Signature Logic

### Test 14A: Anonymous + Simple Message
**Q3**: B (Anonymous)  
**Q8**: A (Simple festive message)

**Expected Signature**:
- "Include 'Happy Diwali!' elegantly at bottom"

**Status**: ⏳ To be tested

### Test 14B: Person + Name with Message
**Q3**: A (Priya)  
**Q8**: B (Name with message)

**Expected Signature**:
- "Include 'With love, Priya' elegantly at bottom"

**Status**: ⏳ To be tested

### Test 14C: Company + Name as-is
**Q3**: C (ABC Corp)  
**Q8**: A (Name as-is)

**Expected Signature**:
- "Include 'ABC Corp' elegantly at bottom"

**Status**: ⏳ To be tested

---

## ✅ Test 15: Newline Formatting

**Platform**: Gemini

**Expected Behavior**:
- All options should be on separate lines
- Blank line between each option
- Example:
  ```
  A. Option 1
  
  B. Option 2
  
  C. Option 3
  ```

**Status**: ⏳ To be tested

---

## 📊 Test Results Summary

| Test # | Test Case | ChatGPT | Gemini | Notes |
|--------|-----------|---------|--------|-------|
| 1 | System Prompt | ⏳ | ⏳ | Immediate start |
| 2A | Platform A | ⏳ | ⏳ | ChatGPT/Copilot |
| 2B | Platform B | ⏳ | ⏳ | Gemini |
| 3A | Festival Both | ⏳ | ⏳ | Preset loading |
| 3B | Festival Diwali | ⏳ | ⏳ | Preset loading |
| 3C | Festival Kali Puja | ⏳ | ⏳ | Preset loading |
| 4A | Identity Person | ⏳ | ⏳ | Name extraction |
| 4B | Identity Anonymous | ⏳ | ⏳ | Anonymous flag |
| 4C | Identity Company | ⏳ | ⏳ | Company name |
| 5 | Primary Color | ⏳ | ⏳ | 6 options |
| 6 | Accent Colors | ⏳ | ⏳ | 5 options |
| 7 | Art Style | ⏳ | ⏳ | 5 options |
| 8A | Regional Yes | ⏳ | ⏳ | Custom style |
| 8B | Regional No | ⏳ | ⏳ | Skip |
| 9A | Q8 Anonymous | ⏳ | ⏳ | Conditional |
| 9B | Q8 Person | ⏳ | ⏳ | Conditional |
| 9C | Q8 Company | ⏳ | ⏳ | Conditional |
| 10 | ChatGPT Generate | ⏳ | ⏳ | Image gen |
| 11 | Gemini Prompt | ⏳ | ⏳ | Prompt output |
| 12A | Mandatory Diwali | ⏳ | ⏳ | People |
| 12B | Mandatory Kali Puja | ⏳ | ⏳ | Ma Kali |
| 12C | Mandatory Both | ⏳ | ⏳ | Both elements |
| 13A | Validation Long | ⏳ | ⏳ | Reject |
| 13B | Validation Valid | ⏳ | ⏳ | Accept |
| 14A | Signature Logic 1 | ⏳ | ⏳ | Anonymous |
| 14B | Signature Logic 2 | ⏳ | ⏳ | Person |
| 14C | Signature Logic 3 | ⏳ | ⏳ | Company |
| 15 | Newline Formatting | ⏳ | ⏳ | Gemini |

---

## 🎯 Testing Instructions

### For ChatGPT Testing:
1. Copy `Diwali-AI-Poster-Creation-Prompt-v4.md`
2. Paste into ChatGPT
3. Say "Load and run this script"
4. Follow through with Test 1-15
5. Mark results in table above

### For Gemini Testing:
1. Copy `Diwali-AI-Poster-Creation-Prompt-v4.md`
2. Paste into Gemini
3. Say "Load and run this script"
4. Follow through with Test 1-15
5. Mark results in table above

---

## 📝 Notes for Testing

- Test both platforms separately
- Document any deviations from expected behavior
- Note any formatting issues
- Check if conditional logic works correctly
- Verify mandatory elements are included
- Confirm newline formatting in Gemini

---

**Test Created**: October 20, 2024  
**Version**: 2.10  
**Status**: Ready for virtual testing
