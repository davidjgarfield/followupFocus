# followupFocus
Megalayer GPL Project
http://www.megalayer.com

A FREE GPL auto-reply follouwp CRM script project (usually charged for by many 'email services') -- can be set up as a daily chron or fired off manuallly, updates a leads list with days old and sends promotions to leads based on when they are acquired.  


Desired Roadmap: 

v1.5 Updates lead data if certain emails are opened [pixel driven]

v1.6 Display quantification of email campains 

v1.7 Cookie tracking data for which page lead came from and which form version lead filled out

v1.8 Ability to set up more than one campaign for same lead list sent 50/50 for simple A/B testing

v2.0 Create rules to modify future email campaign versions based on a leads previous actions



Upon a specified days age FollowupFocus sends desired auto-replies (editor required to create email files: text only at first, Rich Text and Graphic HTML options --compatible with most Outlook and email client versions later-- ) 

Sets up to connect to MySQL DB Followup_Focus table (v1.0 sends up to 5 different emails on 5 future days) 

For example, Lead: A (John Smith) enters a website and fills out a form and becomes a lead.  That lead is added to a Followup_Focus table along with datetime, and a 'days_old' field.  This script adds +1 day each day to each row in the table.  When lead A is 3 days old, send email followup Ver 1.  On 4 days old send followup email ver 2 and so on.  

Marketing reason: This example email campaign creates calls to action with 4 followup emails. When automated, each lead is processed based on each days old they exist, instead of sending emails to lead lists on certain day(s) each week.  

Sample campaign that converts leads to an offer: 
Day 2:  Email subject:  Nme, Thank you!
Day 3:  Email subject:  Confirmation is now required (asks for a signup with paid subscription)
Day 4:  Email subject:  Last Chance! (discount only lasts for dynamic date on web page based on cookie)
Day 5:  Email subject:  FINAL NOTICE! (Firm call to action subject sounds like a due bill, gets most response)




