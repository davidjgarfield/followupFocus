![FollowupFocus-long.png](http://www.megalayer.com/media/FollowupFocus-long.png "FollowupFocus-long.png") 

# FollowupFocus
Megalayer GPL Project
http://www.megalayer.com

# About
A FREE GPL auto-reply dynamic autoresponder followup script. 
This automation project (usually charged for by many expensive 'email service suites') is generally pretty easy to code and impliment
but every plugin or emailer creator wants to make a buck.  This script will do the same exact thing, can run on the domain the marketer desires and will automate followup processes keeping it fair in helping our fellow marketing audience.

MySQL table tracking lead (website form signups) acquisition
  - Script updates +1 day to each lead on the list
  - Provided UI Form gives lead list owner abililty to create up to 5 auto-reply emails
  - Each email reply retains how many days old a lead must reach before it can be emailed
  - Script checks #days lead exists and when the days match the rule, script sends desired message


## How It Works
Followup script can be set to run daily as a chron, or run it once a day manually
  -OR, perhaps worth creating a way a sited pageload would fire the script to run once per day so as long
  as a website had any traffic at all that day, the script would run once.
  Folowup Focus sends out multiple time lapsed promotional emails to leads based on when they are acquired.


## Desired Roadmap
Desired Future Features:
   - v1.5x Confirm/track emails viewed/opened [pixel served]
   - v1.6x Display quantification of email campains / graph emails opened and website return visit CTA ratios
    -v1.7x Cookie tracking from website ammends lead detail for first and last page lead came from, which form ver lead used
    -v1.8x Ability to set up more than one campaign for same lead list say 50/50 for simple A/B testing
    -v2.0x Create rules GUI interface for campagins that let you modify what happens next for specific actions performed by lead. 
    
### Description Detail
When a specific number of days later (say it's been 2 days) a new lead's age is now 2.
FollowupFocus generates and emails a desired first "Thank you, Name" reply for each 2 day old lead.
To do so, front end campaign creation and management interfaces are needed to:
1. Connect to their MySQL DB
2. Create Megalayer_DB with: Followup_Focus_Leads table

3. Support option to map:
    -existing lead capture forms
    -exisitng MySQL lead table fields
    -newly created lead capture forms
    -custom fields

##Followup_Focus_Lead Table Starting Fields
    Suggested starting fields are:
    id, 
    uername,
    DATETIME,
    firstname,
    lastname,
    fullname,
    email,
    phone (optional),
    Address (optional),
    City (optional),
    State (optional),
    Zip (optional),
    
    Provide ability to create/add, track, and or insert into dynamic email, approximately 10 or so additional 'custom_fields' 
    onto existing Followup_Focus_Lead's table can be added, i.e.: campaign_type, lead_type, lead_source, lead_source_detail

UI FollowupFocus Campaign Creation Panel
      Campaign Identifier Creation Page:
          - Name Campaign
          - Create/Remove any fields required for lead data
          - Identify total number of responses [Email Replies] the campaign requires
          - Identify total number of days each email response requires to be sent
      Campaign: Email Assett Creation Page:
            1. Provides form interface to create text email reply and creates saved data files
            2, All and additionally created fields are supplied in dropdown selection can be used and referenced IN email replies  
              a. text only at first, Rich Text and Graphic HTML [table Outlook compatible] options --versions later-- ) 
      b. the email itself 

Sets up to connect to MySQL DB Followup_Focus table (v1.0 sends up to 5 different emails on 5 future days) 

For example, Lead: A (John Smith) enters a website and fills out a form and becomes a lead.  That lead is added to a Followup_Focus campaign along with datetime, and a 'days_old' field.  This script adds +1 day each day to each row in the table.  When lead A is 2 days old, send followup email #1a, when 3 days old send followup email #2 and so on.  

###Marketing Case Use
Marketing reason: This example email campaign creates calls to action with 4 followup emails. When automated, each lead is processed based on each days old they exist, instead of sending emails to lead lists on certain day(s) each week.  

Sample promotional tactic campaign used over the years that converts leads to an offer: 
Day 2:  Email subject:  Nme, Thank you!
Day 3:  Email subject:  Confirmation is now required (asks for a signup with paid subscription)
Day 5:  Email subject:  Last Chance! (discount only lasts for dynamic date on web page based on cookie)
Day 6:  Email subject:  FINAL NOTICE! (Firm call to action subject sounds like a due bill, gets most response)


####Project Creator / Moderator

This project is maintained by [David J Garfield](http://www.davidjgarfield.com/ "David Garfield") and [Megalayer Technologies](http://www.megalayer.com "Megalayer Technologies"). 

## Contributing

If you have any ideas for things we should include, please use one of the following methods to submit them:

1. Send us pull requests
2. Create an issue in the project (right side)
3. Send us links through the issues feature, and we'll parse and incorporate them
3. Email dgarfield@megalayer.com with content to add

Significant effort is made to give attribution whenever possible, and if you are, or know who the original author/curator is, please let us know so we can give proper credit.

### Attribution

- David Garfield thanks Cory Reed Smith's content, including all authors from the InMyExperience.co project 



This project stays great because of care and love from the community, and we will never forget that.



