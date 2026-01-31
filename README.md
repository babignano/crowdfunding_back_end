# Crowdfunding Back End
Caterina Lopez

## Planning:
### Concept/Name
Dance-fanstatic-raise (for now) will be a crowdfunding website to support performaners and sporting groups with their specific goals..

### Intended Audience/User Stories
Performaners and sporting groups.....

- As a user I can see a list of fundraisers on the homepage?
- As a user I can login to the website and see my profile
- As a user I can see an individual fundrasiers
- As a user I can see photos and/or videos of the fundrasier
- As a user I can comment on a fundraiser

### Front End Pages/Functionality
- Homepage
    - User Details
    - List Fundraisers
        - Individual Fundraiser

### API Spec

| URL | HTTP Method | Purpose | Request Body | Success Response Code | Authentication/Authorisation |
| --- | ----------- | ------- | ------------ | --------------------- | ---------------------------- |
| /fundraisers/ | GET |Return all fundraisers| N/A |200|N/A|
| /fundraisers/ | POST |Create a new fundraiser|Fundraiser object|201|Must be logged in|
| /fundraisers/:id | GET |Return fundraiser by ID|N/A|200|N/A|
| /fundraisers/:id | PUT |Update a fundraiser|Fundraiser object|20|Must be logged in and the owner|

### DB Schema
![]( {{ ./relative/path/to/your/schema/image.png }} )