# AI Onboarding Automation (Summary): Business Data Extraction & JSON Structuring

This case study summarizes an AI-powered tool I developed during my internship at StatStak to automate the onboarding of new sports facilities onto the platform. The system used OpenAI’s GPT-4 to extract structured information from public business data and generate a complete onboarding JSON config — reducing manual setup time from hours to minutes.

## 🧠 Problem

Onboarding new clients required manually collecting and inputting:
- Branding info (logos, colors, descriptions)
- Lesson, facility, and team structure
- Fees, discounts, policies, and media links

This process was repetitive and error-prone.

## ⚙️ My Role

- Designed a system that queried OpenAI’s API with tailored prompts
- Parsed business websites and social media to find relevant data
- Engineered a multi-step prompt chain that:
  - Extracted business info
  - Formatted it as a structured JSON block
  - Validated key fields for platform ingestion
- Built a testing workflow using Postman and integrated into Flowise
- Collaborated with the product team to align outputs with real onboarding needs

## 🔧 Tech Stack

- OpenAI GPT-4 (Playground + API)
- Flowise (no-code agent framework)
- Postman (workflow testing)
- JSON structuring + parsing
- Prompt engineering and validation

## 🧪 Sample Output (Simplified)

```json
{
  "business_name": "Southtown Soccer",
  "description": "Elite soccer training for all ages",
  "brand_colors": ["#0055A5", "#FFFFFF"],
  "facilities": [
    {
      "name": "Main Field",
      "sports": ["Soccer"],
      "lessons": ["Private", "Group", "Camps"]
    }
  ],
  "contact_email": "info@southtownsoccer.com"
}
```
## 📈 Outcome

- Enabled one-click onboarding for internal use  
- Standardized data input and reduced manual errors  
- Created a base for future auto-scraping and prefill flows

## 🔒 Note

This is a high-level, anonymized summary of a proprietary internal tool. No sensitive business data is shared here.
