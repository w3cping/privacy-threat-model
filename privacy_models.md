# Summary

This document serves to outline the main camps of thought regarding what privacy entails, and identify privacy threats to some or all such privacy models.  It can advise on what is accepted by the entire web community and W3 as a privacy threat, and what is only considered a threat to some groups.

If a privacy model does not represent an editor's ideal model, they may consider adding a new one rather than editing the existing one if the change is not additive.

This is meant to be more a general guide rather than a proposal-by-proposal definition of privacy listing.

## Privacy Models

### The No Tracking Theory of Privacy
This theory is the idea that user data should not be tracked at all, and should be made impossible to track. No user should be identifiable in anything that touches the client.

All forms of individual tracking should be prevented entirely and made impossible. It is acceptable if this comes at the cost of loss of customization or functionality.

All forms of profiling should be prevented.

**Benefits:**

100% guarantee a user cannot be tracked.

**Issues:**

Potentially not feasible to lock out every tracking method, esp tracking by the browser or OS.

Potentially not feasible to lock out every profiling method, esp ‘form profiling’. 

Concerns above infeasibilities could lead to profiling monopolization by companies whose tracking methods cannot be locked out, leading to a worse privacy state and less web competition.

Breaks current technologies.

Concerns users will not have transparency/control over their data when they are tracked under the assumption it should not exist.

Leads to subscription and walled garden web solutions.

Preventing fingerprinting requires entropy management that restricts abilities of the internet.


### The Control Theory of Privacy via ID
This theory is the idea that a user should have total control over their online data, and profiling may exist while this is the case.

A user’s profile must be linked to an id stored on device that can be passed in place of Personal Information.

Personal Information is restricted or forbidden to be passed/sold.

The id can be removed from the device by the user to thwart all existing profiles.

Every tracking method and profiling method should be auditable.

A user should have the ability to be forgotten, or a user’s ability to delete their profile.

A user should have the ability to opt (in or out whichever is deemed more appropriate) to tracking

Legal arrangements used to punish detractors

**Benefits:**

Does not break current technologies

Keeps open web, prevents walled garden dominance

Custom experiences can still exist


**Issues:**

Reliance on audits to detect cheaters may be impractical

Data Sales and Sharing may obscure what data is where

When PI serves a legal business need (your name must be recorded in an ecommerce transaction) some data cannot be deleted

When PI is associated, revoking the id may not thwart existing profiles for a cheating operator or under some implementations


## Potential* Threats

"Potential" is due to differences in privacy definitions. A certain definitions may deem something a threat to be eliminated, others a threat to be watched, others not a threat.

### Individual Identification

This refers to being able to identify a user on a user agent/browser. This is a broad category. The sub categories will be listed separately below. Some privacy models consider them threats to be prevented, others consider them acceptable but requiring safeguards and increased user control. All should be considered by any privacy model at minimum for the purposes of safeguards.

**Sync Tracking**: Any type of cross device syncing involving browser data. Examples include Chrome Sync. This allows for cross domain data to be tracked by the browser company. This also allows for user profile data and customization to be built from this data.

**OS Snooping**: Examples: Safari-ios or Google-Android integrations that enable the operating system to gain insight into user data in the browser when it appears as an app, or in some cases even in the classic PC browser. These browser-side integrations allow tracking prevention safeguards to be bypassed by the browser and/or OS companies. This allows a user’s web data to be tracked and users to be profiled on the web through the user agent through a back door.

**Stack ID**: The operating system or any program higher on the stack assigns a device id that can be correlated to the web user, and passes it through with some or all client calls.

**Browser Login Tracking**: The ability for a user to log in to their browser by some means that exists across domain, enabling the browser or affiliate to individually track them. Examples include gmail/chrome login.

**First and Third Party Cookie Tracking**: a cookie can be used to identify an individual web user. The cookie can be cross domain, or a synced first party domain cookie. Either performs the same function, despite the misnomer that only third party cookies can track.

**Storage Tracking**: Tracking using a storage system other than cookies to store an id to track a user,

**Browser Snooping**: This refers to the ability of a browser to send user data signals to a home server by its own accord. It also includes taking data from signals not meant to be related to user tracking, profiling, or data collection, and using them for that purpose as part of a microservice architecture system.

**Fingerprinting**: The use of multiple data points of a device’s user agent to identify it as close to unique, theryby identifying a user. Fingerprinting can be performed by a third party, first party, or even the browser client itself which has access to the most entropy data.

### Profiling

This section details situations in which a profile of user data can be built, or problems relating to profiling.

**Form Profiling**: This refers to the practice of building a user profile based on form information filled out on a web page, often for the purpose of signing up for a product. In some cases this is legally required, as in ecommerce. The threat also refers to taking legally required information and then using it for other purposes.

**Choice Profiling**: This refers to creating a user profile based on choices a user makes such a purchases on an ecommerce platform, or shows watched on a streaming platform. This profile is used for customization options and the data can also be sold for numerous uses (product decisions, data science, advertising).

**Hidden Profiles**: Refers to a user being unable to access a web system’s profile on their user data. This could be because it is impossible or impractical. It is of particular concern because a user can be misled as to what data of theirs is being captured where this threat exists.

**Untouchable Profiles**: Refers to a user profile that a user is unable to request deletion of. Includes cases where it is impractical for a user to verify or have confidence their data has truly been deleted upon request.

**Aggregate Link Profiling**: Linking an aggregate system (like floc) to an individual user through various individual tracking, coop, or machine learning methods.
