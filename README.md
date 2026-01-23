# Crowdfunding Back End - SIMPLE Example
Biagio Abignano

## Planning:
### Concept/Name
**HelpMeOut** - A simple crowdfunding platform where people can ask for help funding their projects and others can pledge to support them.

### Intended Audience/User Stories
People who need money for projects and people who want to help fund good ideas.

- As a creator, I want to post my project idea and funding goal
- As a supporter, I want to see projects and pledge money to ones I like
- As a user, I want to log in so my pledges and projects are tracked

### Front End Pages/Functionality
- **Home**
    - List all fundraisers
    - Click to view details
- **Fundraiser Details**
    - See full info and all pledges
    - Make a pledge if logged in
- **Create Fundraiser**
    - Form to create new fundraiser (login required)
- **Login/Signup**
    - Create account or login

### API Spec

| URL | HTTP Method | Purpose | Request Body | Success Response Code | Authentication/Authorisation |
| --- | ----------- | ------- | ------------ | --------------------- | ---------------------------- |
| /fundraisers/ | GET | Get all fundraisers | N/A | 200 | None |
| /fundraisers/ | POST | Create fundraiser | Fundraiser object | 201 | Logged in |
| /fundraisers/1/ | GET | Get one fundraiser (with pledges) | N/A | 200 | None |
| /pledges/ | GET | Get all pledges | N/A | 200 | None |
| /pledges/ | POST | Create pledge | Pledge object | 201 | Logged in |

### DB Schema

**Users** → **Fundraisers** (one user owns many fundraisers)
**Users** → **Pledges** (one user makes many pledges)
**Fundraisers** → **Pledges** (one fundraiser has many pledges)