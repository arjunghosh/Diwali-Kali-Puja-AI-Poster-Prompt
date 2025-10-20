# 🪔 Diwali & Kali Pujo AI Image Prompt

> **Production-ready AI prompt script for creating personalized festival posters with advanced LLM orchestration, bilingual support, and cross-platform compatibility**

[![License](https://img.shields.io/badge/license-Attribution-green.svg)](LICENSE)
[![AI Platforms](https://img.shields.io/badge/platforms-ChatGPT%20%7C%20Gemini%20%7C%20Copilot-orange.svg)](https://github.com/arjunghosh/Diwali-Kali-Puja-AI-Poster-Prompt)
[![Version](https://img.shields.io/badge/version-2.10-blue.svg)](https://github.com/arjunghosh/Diwali-Kali-Puja-AI-Poster-Prompt)

## 🎯 What This Is

A sophisticated AI prompt engineering solution that transforms any LLM (ChatGPT, Gemini, Copilot) into a personalized festival poster generator. This project demonstrates advanced prompt engineering techniques including:

- **Conditional Logic Orchestration**: Dynamic Q&A flow with context-aware branching
- **Cross-Platform Compatibility**: Single prompt works across multiple AI platforms
- **Cultural Authenticity**: Bilingual support with culturally appropriate defaults
- **Production-Ready**: Input validation, error handling, and comprehensive testing

## ✨ Key Features

### 🚀 **Advanced Prompt Engineering**
- **Immediate Start**: Auto-executes when loaded (no manual trigger needed)
- **Context-Aware Branching**: Adapts questions based on previous answers
- **Smart Variable Substitution**: Dynamic content generation
- **Conditional Logic**: Platform-specific execution paths

### 🎨 **User Experience**
- **8-Question Flow**: Optimized for clarity and efficiency
- **6 Primary Color Options**: Expanded palette for customization
- **5 Accent Color Options**: Rich visual combinations
- **Regional Art Styles**: Support for traditional Indian art forms
- **Multi-Identity Support**: Personal, corporate, and anonymous options

### 🌏 **Cultural Intelligence**
- **Bilingual Greetings**: Hindi (शुभ दीपावली) and Bengali (শुभ কালী পূজা)
- **Mandatory Visual Elements**: Ensures cultural authenticity
- **Festival-Specific Presets**: Diwali, Kali Pujo, or Both
- **Traditional Art Styles**: Madhubani, Pattachitra, Alpana, Warli, Kalamkari

### 🛡️ **Production Quality**
- **Input Validation**: 50-character limit enforcement
- **Error Handling**: Graceful degradation for invalid inputs
- **Cross-Platform Testing**: Validated on ChatGPT, Gemini, Copilot
- **Comprehensive Test Suite**: 15+ test scenarios included

## 🚀 Quick Start

```bash
# 1. Copy the prompt file
Diwali-AI-Poster-Creation-Prompt-v4.md

# 2. Paste into your preferred AI platform
ChatGPT, Gemini, or Copilot

# 3. Follow the interactive Q&A
8 simple questions → Get personalized poster

# 4. Done!
High-resolution festival poster generated
```

## 📋 How It Works

### Architecture Overview

```
┌─────────────────────────────────────────┐
│  System Prompt (Immediate Start)        │
└──────────────┬──────────────────────────┘
               │
               ▼
┌─────────────────────────────────────────┐
│  Q1: Platform Selection                 │
│  └─→ Branch to Script A or B            │
└──────────────┬──────────────────────────┘
               │
               ▼
┌─────────────────────────────────────────┐
│  Q2: Festival Selection                 │
│  └─→ Load Festival Presets              │
└──────────────┬──────────────────────────┘
               │
               ▼
┌─────────────────────────────────────────┐
│  Q3-Q8: Customization Questions         │
│  └─→ Collect user preferences           │
└──────────────┬──────────────────────────┘
               │
               ▼
┌─────────────────────────────────────────┐
│  Generate Final Prompt/Image            │
│  └─→ Apply all selections               │
└─────────────────────────────────────────┘
```

### Q&A Flow

1. **Platform Selection** → Choose execution path (ChatGPT/Copilot or Gemini)
2. **Festival Choice** → Diwali, Kali Pujo, or Both (loads presets)
3. **Identity** → Person, Anonymous, or Company/Team
4. **Primary Color** → 6 culturally appropriate options + custom
5. **Accent Colors** → 5 complementary combinations + custom
6. **Art Style** → Traditional, Modern, Watercolor, Mandala, or Custom
7. **Regional Style** → Optional traditional art forms
8. **Signature** → Context-aware (adapts to identity choice)

### Festival Presets

#### 🪔 Diwali
- **Greeting**: Happy Diwali (शुभ दीपावली)
- **Elements**: Glowing diyas, kandils, rangoli patterns, festive night sky
- **Mandatory**: People celebrating (families, children, gatherings)
- **Colors**: 6 options (Festive Maroon, Deep Blue, Royal Purple, Rich Orange, Deep Green, Elegant Gold)
- **Accents**: 5 options (Gold/Silver, Orange/Fuchsia, Emerald/Gold, Purple/Magenta, Copper/Bronze)

#### 🌺 Kali Pujo
- **Greeting**: Happy Kali Pujo (শুভ কালী পূজা)
- **Elements**: Red hibiscus flowers, Alpana patterns, divine atmosphere
- **Mandatory**: Ma Kali's face with red tongue (prominent)
- **Colors**: 6 options (Deep Red, Midnight Blue, Jet Black, Crimson, Navy, Charcoal)
- **Accents**: 5 options (Red/White, Gold/Red, Silver/Red, White/Gold, Crimson/Gold)

#### 🎊 Both Festivals
- **Greetings**: Both Diwali and Kali Pujo
- **Elements**: Harmonious blend of both festival elements
- **Mandatory**: People celebrating + Ma Kali (minimum shown)
- **Colors**: Combined palette from both festivals
- **Accents**: Mixed combinations

## 🎨 Use Cases

### Personal Use
- Create personalized Diwali/Kali Pujo greetings
- Share with family and friends
- Customize with names and messages

### Corporate Use
- Company festival greetings
- Team celebrations
- Brand-appropriate designs

### Community Use
- Anonymous festive wishes
- Universal appeal
- No personalization needed

## 🛠️ Technical Specifications

| Specification | Details |
|---------------|---------|
| **Platforms** | ChatGPT (DALL-E 3), Gemini (Imagen 3), Copilot (Designer) |
| **Languages** | English, Hindi (हिंदी), Bengali (বাংলা) |
| **Input Validation** | 50 characters max, alphanumeric + basic punctuation |
| **Image Output** | Ultra-high resolution, 300 DPI |
| **Dependencies** | None (platform native) |
| **Test Coverage** | 15+ scenarios across platforms |
| **Conditional Logic** | 6+ branching points |
| **Variable Substitution** | 20+ dynamic variables |

## 📖 Usage Examples

### ChatGPT/Copilot (Auto-Generate)
```
User: [Pastes script]
AI: Hello! Which AI platform? A. ChatGPT/Copilot B. Gemini
User: A
AI: Great! I'll ask 8 questions to create your poster.
     Which festival(s)? A. Both B. Diwali only C. Kali Pujo only
User: A
AI: Who is this for? A. Person B. Anonymous C. Company/Team
[... continues through 8 questions ...]
AI: Thank you, Priya! Here's your poster.
     [Generates image]
```

### Gemini (2-Step Process)
```
User: [Pastes script]
AI: Hello! Which AI platform? A. ChatGPT/Copilot B. Gemini
User: B
AI: Great! I'll ask 8 questions to build your prompt.
[... continues through 8 questions ...]
AI: Thank you, Priya! Copy this prompt and paste it back:
     [Provides formatted prompt]
User: [Pastes prompt back]
AI: [Generates image]
```

## 🎯 Advanced Features

### Conditional Logic
- **Q8 Signature**: Adapts based on Q3 identity choice
  - Anonymous → Generic festive messages
  - Person/Company → Name display options
- **Festival Presets**: Loads appropriate variables based on Q2
- **Platform Branching**: Different execution paths for ChatGPT vs Gemini

### Input Validation
- **50-Character Limit**: Enforced on all custom inputs
- **Smart Rejection**: Clear error messages
- **Graceful Handling**: No crashes on invalid input

### Cultural Authenticity
- **Mandatory Visual Elements**: 
  - Diwali → People celebrating
  - Kali Pujo → Ma Kali's face with red tongue
  - Both → People + Ma Kali (minimum)
- **Bilingual Support**: Native script greetings
- **Traditional Art Styles**: Regional authenticity

## 📚 Regional Art Styles Supported

- **Bengali Alpana**: Traditional floor art patterns
- **Pattachitra**: Orissa scroll paintings
- **Madhubani**: Bihar folk art
- **Warli**: Maharashtra tribal art
- **Kalamkari**: Andhra Pradesh hand-painted textiles

## 🧪 Testing

Comprehensive test suite included: `SCRIPT_VALIDATION_TEST.md`

**Test Coverage**:
- ✅ Platform selection (ChatGPT vs Gemini)
- ✅ Festival presets (Diwali, Kali Pujo, Both)
- ✅ Identity types (Person, Anonymous, Company)
- ✅ Color options (6 primary, 5 accent)
- ✅ Art styles (5 options)
- ✅ Regional styles (custom input)
- ✅ Conditional Q8 logic
- ✅ Mandatory visual elements
- ✅ Input validation
- ✅ Newline formatting (cross-platform)
- ✅ Final generation (both platforms)

## 🤝 Contributing

Contributions welcome! This project demonstrates:
- Advanced prompt engineering techniques
- Cross-platform AI orchestration
- Cultural sensitivity in AI applications
- Production-ready prompt design

**How to Contribute**:
1. Fork the repository
2. Create feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open Pull Request

## 📄 License

**Attribution License** - Simple and permissive

### Attribution Requirements

If you use this in any way, please:
1. ✅ Acknowledge: **Arjun Ghosh**
2. ✅ Link back: https://github.com/arjunghosh/Diwali-Kali-Puja-AI-Poster-Prompt

**Example**:
```
Created by Arjun Ghosh
Source: https://github.com/arjunghosh/Diwali-Kali-Puja-AI-Poster-Prompt
```

## 👤 Author

**Arjun Ghosh**

🚀 **Founder & CEO** - [Loyla.ai](https://loyla.ai)  
💼 **Director of Sustainability & New Ventures** - Neoenrg  
🎯 **Expertise**: AI/ML, Digital Transformation, Sustainability

**Connect**:
- 📧 Email: [ghosh.arjun@gmail.com](mailto:ghosh.arjun@gmail.com)
- 💼 LinkedIn: [Arjun Ghosh](https://linkedin.com/in/arjunghosh)
- 🌐 Company: [Loyla.ai](https://loyla.ai)

## 🙏 Acknowledgments

- Traditional Indian folk art inspirations
- Bengali Alpana and Hindi Devanagari typography
- Community feedback for optimization
- Cultural authenticity advisors

## 📞 Support & Feedback

- 🐛 **Issues**: [GitHub Issues](https://github.com/arjunghosh/Diwali-Kali-Puja-AI-Poster-Prompt/issues)
- 💬 **Discussions**: [GitHub Discussions](https://github.com/arjunghosh/Diwali-Kali-Puja-AI-Poster-Prompt/discussions)
- 📧 **Email**: [ghosh.arjun@gmail.com](mailto:ghosh.arjun@gmail.com)

---

## 🎓 What This Demonstrates

This project showcases advanced AI/ML engineering capabilities:

### Prompt Engineering Excellence
- ✅ Conditional logic orchestration
- ✅ Cross-platform compatibility
- ✅ Dynamic variable substitution
- ✅ Context-aware branching

### Production-Ready Design
- ✅ Comprehensive testing
- ✅ Input validation
- ✅ Error handling
- ✅ User experience optimization

### Cultural Intelligence
- ✅ Bilingual support
- ✅ Cultural authenticity
- ✅ Regional customization
- ✅ Traditional art integration

### Technical Innovation
- ✅ Platform-agnostic design
- ✅ Zero dependencies
- ✅ Immediate execution
- ✅ Scalable architecture

---

**Made with ❤️ for the Diwali and Kali Pujo community**

*Demonstrating AI excellence through cultural celebration* 🪔✨

---

**Repository**: https://github.com/arjunghosh/Diwali-Kali-Puja-AI-Poster-Prompt  
**Version**: 2.10  
**License**: Attribution License