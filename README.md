# Deliverable - Inclusive Form Flow

## Repository URL:  
    https://github.com/enappen/Deliverable_Inclusive-Form-Flow  
  
## Website URL:  

  
## Fonts:  

  
## Purpose & Expectations:  
      The purpose of the form, titled "Become a Member" is to serve as an application for users that would like to become a member by becoming a writer, researcher, or both. The target audience of this form is for subscribers or those interested in the websites topic and want to become a contributing member. The form collects contact information (name, phone number, and email address), the applicants preferred position as a member, and two optional fields (a section to briefly express why they are interested in becoming a member and another field asking where they heard of the organization). The form identifies required fields in the legend before the form (stating "Sections with (*) are required to complete.") and having "(Optional)" next to optional fields. After submitting, their information would be set via a URL to to organization. The privacy statement at the top of the form urges the applicant not to provide confidential information and that information is not sold to a third party.
  
## Task and Data Plan:  
    - The name input is a required field needed for identifying the applicant. The type is set to text and the name is "name" which matches the for attribute in its label. Autocomplete is set to name which will inform the user-agent to recommend a previously used name. [SENSITIVITY HERE]
    
    - The phone input is a required field needed for a contact method. Type is set to "tel" for telephone. Autocomplete is set to "tel" to inform the user-agent to recommend a previously used phone number. The input is named "phone", which matches the for attribute in its label. [SENSITIVITY HERE]

    - The email input is a required field needed as a secondary contact method. Type is set to "email", which requires an input that follows proper email formatting. Autocomplete is set to "email" to inform the user-agent to recommend a previously used email. Name is set to "email", which matches its label's for attribute. [SENSITIVITY HERE]

    - The position preference fieldset is a required field needed to determine which position the applicant is applying for. The legend helps identify that the applicant must select one option. There are three total inputs with the type radio sharing the same name (preferred-preference) restricting only one option to be selected at a time. The value for each radio input reflects the choice (i.e. writing, research, or both). The inputs are nested in the label so the radio button appears on the same line and are naturally programmatically associated. There is no autocomplete as the input is a radio button. [SENSITIVITY HERE]

    - The input named "about-you" is an optional field that allows the applicant to express their interest in becoming a member. The type is textarea with the id "about-you" to match its label's for attribute. Autocomplete is set to "off" because it is not a section the user-agent would have stored information on to prefill. The constraint of maxlength is set to 300 to limit the amount of characters used in the input. This helps keep the users input brief. The character limit is explained in the help paragraph. The textarea selector was used to establish a minimum height of 7.5rem. 

    - The input named "discovery" is an optional field where the user can provide meaningful data that the organization can use to keep track of where users discovered the website. Type is set to text and named "discovery" which matches the labels for attribute for programmatic association. Autocomplete is set to off as it's not a section the user-agent would have stored information on to prefill. A placeholder with the value "ex. social media" is used to help provide an example as to what kind of answer the input is looking for (such as heard from a friend, an organization, etc.). The constraint of maxlength is set to 30 to limit the amount of characters used in the input. The width of the input was set to 34 characters to fully display the maximum amount of characters allowed and indicate the character limit to the user. [SENSITIVITY HERE]

  
## Semantic Form:  

  
## Requirements and Validation:  

  
## States and Recovery:  

  
## System and Evidence:  
    - Extended System:  
    - AI Disclosure: No AI was used in this project.  
    - Test Record:  
