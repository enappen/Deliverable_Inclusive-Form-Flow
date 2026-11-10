# Deliverable - Inclusive Form Flow

## Repository URL:  
    https://github.com/enappen/Deliverable_Inclusive-Form-Flow  
  
## Website URL:  
    https://enappen.github.io/Deliverable_Inclusive-Form-Flow/
  
## Fonts:  

  
## Purpose & Expectations:  
      The purpose of the form, titled "Become a Member" is to serve as an application for users that would like to become a member by becoming a writer, researcher, or both. The target audience of this form is for subscribers or those interested in the websites topic and want to become a contributing member. The form collects contact information (name, phone number, and email address), the applicants preferred position as a member, and two optional fields (a section to briefly express why they are interested in becoming a member and another field asking where they heard of the organization). The form identifies required fields in the legend before the form (stating "Sections with (*) are required to complete.") and having "(Optional)" next to optional fields. After submitting, their information would be set via a URL to to organization. The privacy statement at the top of the form urges the applicant not to provide confidential information and that information is not sold to a third party.
  
## Task and Data Plan:  
    - The name input is a required field needed for identifying the applicant. The type is set to text and the name is "name" which matches the for attribute in its label. Autocomplete is set to name which will inform the user-agent to recommend a previously used name. Collecting a first and last name is considered general information and does not require encrypting.
    
    - The phone input is a required field needed for a contact method. Type is set to "tel" for telephone. Autocomplete is set to "tel" to inform the user-agent to recommend a previously used phone number. The input is named "phone", which matches the for attribute in its label. A phone number is considered general information and does not require additional encryption.

    - The email input is a required field needed as a secondary contact method. Type is set to "email", which requires an input that follows proper email formatting. Autocomplete is set to "email" to inform the user-agent to recommend a previously used email. Name is set to "email", which matches its label's for attribute. An email is considered general information and does not require additional encryption.

    - The position preference fieldset is a required field needed to determine which position the applicant is applying for. The legend helps identify that the applicant must select one option. There are three total inputs with the type radio sharing the same name (preferred-preference) restricting only one option to be selected at a time. The value for each radio input reflects the choice (i.e. writing, research, or both). The inputs are nested in the label so the radio button appears on the same line and are naturally programmatically associated. There is no autocomplete as the input is a radio button. The preferred position selection is not confidential and does not require additional encryption.

    - The input named "about-you" is an optional field that allows the applicant to express their interest in becoming a member. The type is textarea with the id "about-you" to match its label's for attribute. Autocomplete is set to "off" because it is not a section the user-agent would have stored information on to prefill. The constraint of maxlength is set to 300 to limit the amount of characters used in the input. This helps keep the users input brief. The character limit is explained in the help paragraph. The textarea selector was used to establish a minimum height of 7.5rem. This is an optional field that provides only surface level information. The top of the form informs the user to not provide any confidential information.

    - The input named "discovery" is an optional field where the user can provide meaningful data that the organization can use to keep track of where users discovered the website. Type is set to text and named "discovery" which matches the labels for attribute for programmatic association. Autocomplete is set to off as it's not a section the user-agent would have stored information on to prefill. A placeholder with the value "ex. social media" is used to help provide an example as to what kind of answer the input is looking for (such as heard from a friend, an organization, etc.). The constraint of maxlength is set to 30 to limit the amount of characters used in the input. The width of the input was set to 34 characters to fully display the maximum amount of characters allowed and indicate the character limit to the user. This information is only of value to a marketing strategy and is not confidential.

    -The input for preferred method of contact is a required field needed to prioritize reaching out to the applicant according to their preference. The type is set to radio and the name for both inputs is set to "preferred-contact" to ensure only one can be selected at a time. There is not autocomplete, but the phone option is selected by default. This data informs of a preference and contains no personal data.

    - The preferred time to be contacted is a required field needed to document what time works best for the applicant to be reached. The type is an input type that uses the select and option elements for a drop-down menu style. The name is time and no autocomplete is used as its not applicable. One option (Morning, Afternoon, or Evening) must be selected. There is no default value, so the first option acts like a placeholder prompting a choice be made by the applicant. A preferred time to contact the applicant isn't personal information, but allows for the organization responding to the applicant to mindful of when is best to be reached.

  
## Semantic Form:  

### List 8-14 purposeful controls - i.e. buttons, label/input control  
    1. Name text entry input
    2. Phone number tel input
    3. Email input 
    4. Time input with select and option elements (drop-down menu) with options morning, afternoon, and evening
    5. Preferred contact input uses radio buttons (x2) with options phone and email
    6. Preferred position input uses radio buttons (x3) with the options writing, research, and both
    7. Tell us about yourself input uses a text area type that limits 300 characters
    8. Where did you hear about us? text input 
    9. The submit button for the form

### Persistent Label Usage:  
    - Each form field has a programmatically connected relationship between label and input using a matching for and id value (name, phone, email, position-preference, about-you, and discovery).  

###  List input/control types
    - The text type input was selected for name to allow to user to enter their name.
    - The tel type input is used to accept an input for a phone number.
    - The email type input is used to accept a written entry that follows the proper email format.
    - The input with elements select and option are used to provide a familiar user interface used when selecting timeframes and present the only 3 possible options and 1 default disabled option. The default disabled options saying "Select an option" prompts the user to select an option. If a new option is not chosen after interacting, it'll turn from gray to red. If an option is selected it'll turn green. 
    - The radio type input for preferred contact method uses radio button that hold the same name to require one selection at a time. The first option (phone) is selected by default. The other possible option is email; both options reflect the two required contact methods above. 
    - The radio type input for preferred position is used for each option to ensure the answer meets one of the 3 potential type selections: writing, researching, or both. Using this method has the benefit of forcing only one radio button be selected at a time using the checked and required attributes, as well as giving each radio button the same name.
    - The text area type for the input named "about-me" allows for a custom text response with a 300 character limit. 
    - The text type for the input named "discovery" with a character limit of 30 to allow the user to enter a custom response but keep the response short on a single line.

###  name/value relationships
    - Name/value relationships would function as follows in the following example:  
        name=Jane+Doe;  
        phone=000-000-0000;  
        email=jdoe@email.com;  
        preferred-preference=Writing;  
        about-you=Words;  
        discovery=Social+Media;  

###  identify the submit button
    - The button at the end of the form was assigned a type of "submit" to explicitly declare it as the submit button for the form.

  
## Requirements and Validation:  
    - The first section of the form informs the applicant that questions with a (*) are required to be completed. For additional clarity, "(Optional)" is added to all optional questions.
    - Native constraints are applied to email due to its assigned type (email) requiring a proper email format be used. 
    - Helpful format examples are visible via placeholders in the fields name (Jane Doe), phone number (123-456-7890), and where did you hear about us (EX: Social Media). No placeholder is provided in tell us about yourself because the help provided already explains what the entry should be if optionally provided. 
    
  
## States and Recovery:  
    - Default is set to background color inherit. Visible focus indicators use the same color and format as previous themes, but the color was slightly darkened to help improve contrast for accessibility. Input required is set to inherit background color as required elements are already accentuated with an asterisk (*) as mentioned in the legend and a heavier border and different color would result in over-styling. User-valid is used to maintain default colors until after the user interacts with the input. When the user does the background turn into a soft pastel green color. Meanwhile, user-invalid makes the background color turn light red after interacting and providing an invalid input. Disabled elements are given a 75% opacity to meet contrast accessibility requirements and provide a muted tone of the button indicating its inability to be used and the cursor is not allowed to interact with the element. For Server-returned error please see example in section F5 on index.html. 

    - Errors produce a light red background color on a field after an incorrect formatted answer or no answer is provided after user interaction to indicate error. Text is also populated next to the form provided information on how to fix the issue depending on the error, and entities are preserved as the document will not fully submit without meeting form requirements. Not submitting prevents the previously entered inputs from resetting.
  
## System and Evidence:  
    - Extended System:  (theme, tokens, responsive layout) have been applied in styles.css
    - Test Record: See index.html at section F6.
    - <a href="field-inventory-template.html">Fictional Test-Data List</a>
    - AI Disclosure: No AI was used in this project.  
