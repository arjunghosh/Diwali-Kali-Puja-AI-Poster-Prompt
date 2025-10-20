# 📊 Project Context & Details

## 🎯 Project Overview

**Name**: Diwali AI Poster Generator  
**Version**: 2.6 (Ultra-Optimized)  
**Type**: AI Prompt Script for Festival Poster Generation  
**Status**: ✅ Ready for GitHub  
**License**: Attribution License

## 📝 What This Project Does

An ultra-optimized AI script that creates personalized Diwali and Kali Pujo festival posters through an interactive 8-question Q&A flow. The script works on ChatGPT, Gemini, and Copilot, automatically starting the conversation when loaded.

## 🔄 Evolution & Optimization

### Original Version (v1)
- 465 lines
- Basic festival selection
- No immediate start
- Separate scripts for each platform

### Current Version (v2.6)
- **224 lines** (52% reduction)
- **Immediate start** functionality
- **Unified script** structure
- **New Q&A flow**: Platform → Festival → Identity → Colors → Style → Regional → Signature
- **Bug fixes**: Variable naming, preset selection, conditional logic
- **Enhanced features**: Name extraction, input validation, bilingual support

### Key Improvements
1. ✅ Added immediate start system prompt
2. ✅ Restructured Q&A flow (8 questions)
3. ✅ Added identity options (person/company/anonymous)
4. ✅ Fixed variable naming inconsistencies
5. ✅ Added festival preset selection logic
6. ✅ Clarified conditional logic
7. ✅ Added name extraction rules
8. ✅ Optimized all sections

## 📁 File Structure

```
Diwali-AI-Poster-Prompt/
├── .gitignore                          # Excludes old versions
├── Diwali-AI-Poster-Creation-Prompt-v4.md  # Main AI script (224 lines)
├── LICENSE                             # Attribution License
├── README.md                           # Public documentation
├── PROJECT_CONTEXT.md                  # This file (internal details)
└── index.html                          # GitHub Pages website
```

## 🎨 Technical Details

### Script Architecture
- **Global Variables**: Titles, greetings, validation rules
- **Festival Presets**: Diwali, Kali Pujo, Both (with elements, colors, accents)
- **Preset Selection Logic**: IF-THEN logic based on Q2 answer
- **Script A**: ChatGPT/Copilot (auto-generate)
- **Script B**: Gemini (2-step process)

### Key Features
1. **Immediate Start**: System prompt triggers Q&A automatically
2. **Platform Agnostic**: Works on all major AI platforms
3. **Bilingual Support**: Hindi (शुभ दीपावली) and Bengali (শুভ কালী পূজা)
4. **Input Validation**: 50-character limit enforcement
5. **Smart Defaults**: Culturally appropriate color palettes
6. **Conditional Logic**: Dynamic content based on user choices

### Q&A Flow
1. **Q1**: Platform (ChatGPT/Copilot vs Gemini)
2. **Q2**: Festival (Diwali, Kali Pujo, or Both)
3. **Q3**: Identity (Person, Anonymous, or Company/Team)
4. **Q4**: Primary Color (Recommended or custom)
5. **Q5**: Accent Colors (Recommended or custom)
6. **Q6**: Art Style (Traditional, Modern, Watercolor, Mandala, Custom)
7. **Q7**: Regional Style (Optional: Bengali Alpana, Pattachitra, etc.)
8. **Q8**: Signature (Name, message, none, or custom)

## 🔧 Implementation Notes

### For AI Implementers
- Use `{VARIABLE}` format for all substitutions
- Apply PRESET SELECTION LOGIC after Q2
- Enforce 50-character validation strictly
- Update chat titles at specified points
- Use `{IF condition: "text"}` for conditional logic

### Variable Naming Convention
- `{SELECTED_GREETING_1}` - Primary greeting
- `{SELECTED_GREETING_2}` - Secondary greeting (if both festivals)
- `{SELECTED_ELEMENTS}` - Visual elements
- `{SUG_COLOR}` - Suggested primary color
- `{OPT_COLOR_B}` - Alternative color option 1
- `{OPT_COLOR_C}` - Alternative color option 2
- `{SUG_ACCENT}` - Suggested accent colors
- `{OPT_ACCENT_B}` - Alternative accent colors
- `{NAME}` - User's name/identity

### Conditional Logic Format
```
{IF BOTH festivals: "text for both"}
{IF single festival: "text for single"}
{IF Q5≠B: "text if Q5 is not B"}
```

## 📊 Statistics

| Metric | Value |
|--------|-------|
| **Original Lines** | 465 |
| **Current Lines** | 224 |
| **Reduction** | 52% |
| **Questions** | 8 |
| **Festival Options** | 3 (Diwali, Kali Pujo, Both) |
| **Identity Options** | 3 (Person, Anonymous, Company) |
| **Platforms Supported** | 3 (ChatGPT, Gemini, Copilot) |
| **Languages** | 3 (English, Hindi, Bengali) |

## 🐛 Bugs Fixed

1. ✅ Variable naming inconsistency (GREETING_1 → SELECTED_GREETING_1)
2. ✅ Missing festival preset selection logic
3. ✅ Unclear conditional logic syntax
4. ✅ Missing name extraction rules
5. ✅ Placeholder format inconsistency
6. ✅ Duplicate Q&A numbering

## 🚀 Deployment

### Git Repository
- **Commits**: 4
- **Files**: 8
- **Status**: Ready to push

### GitHub Pages
- **Website**: index.html (responsive, modern design)
- **URL**: https://YOUR_USERNAME.github.io/diwali-ai-poster-generator
- **Status**: Ready to deploy

### Next Steps
1. Create GitHub repository
2. Push code to GitHub
3. Enable GitHub Pages
4. Update username in files
5. Share project

## 📝 License Details

**Attribution License** - Simple and permissive:
- ✅ Free to use, modify, distribute
- ✅ Commercial use allowed
- ✅ Must acknowledge: "Arjun Ghosh"
- ✅ Must link back to repository
- ✅ No complex restrictions

**Attribution Format**:
```
This script was created by Arjun Ghosh. 
Original source: https://github.com/arjunghosh/diwali-ai-poster-generator
```

## 🎯 Success Metrics

- ✅ Script optimized by 52%
- ✅ All bugs fixed
- ✅ Documentation complete
- ✅ License compliant
- ✅ Website created
- ✅ Git repository ready
- ✅ Ready for public release

## 🔮 Future Enhancements (Optional)

- Add more festival options (Holi, Dussehra, etc.)
- Support for more languages
- Template gallery
- Custom color picker
- Batch generation
- API integration

## 📚 Related Files

- **Diwali-AI-Poster-Creation-Prompt-v4.md**: Main AI script
- **README.md**: Public documentation
- **LICENSE**: Attribution license
- **index.html**: GitHub Pages website
- **PROJECT_CONTEXT.md**: This file (internal details)

## 👤 Project Author

**Arjun Ghosh**
- LinkedIn: https://linkedin.com/in/arjunghosh
- Role: Director of Sustainability & New Ventures, Neoenrg
- Expertise: Digital Transformation, AI/ML, Sustainability

## 📅 Project Timeline

- **Started**: October 2024
- **Version 2.6**: October 20, 2024
- **Status**: ✅ Ready for GitHub
- **Next**: Public release

## 🎉 Project Highlights

1. **Ultra-Optimized**: 52% size reduction while maintaining 100% functionality
2. **Production Ready**: Complete documentation, license, and website
3. **User Friendly**: Simple attribution requirement, no complex restrictions
4. **Well Documented**: Comprehensive README and internal context
5. **Beautiful Website**: Modern, responsive GitHub Pages site
6. **Git Ready**: All files committed, ready to push

---

**Project Status**: ✅ Complete and ready for GitHub  
**Version**: 2.6 (Ultra-Optimized)  
**Last Updated**: October 20, 2024
