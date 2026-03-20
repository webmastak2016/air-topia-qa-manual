# Test Plan – Guest Membership Validation

## AIR-362 (Test Guest creation without missing contact information)

## Objective

Verify validation of required fields (Phone Number and Birth Date) during the Guest membership signup and purchase flow.

## Scope

Testing the Guest Membership flow through:

- Guest Explore Memberships page
- Guest Widget
- Guest Profile editing

## Environment

URL: https://staging.airtopiaparks.com/guest/explore/memberships

Environment: Staging

Device:
Mac mini (Apple M4)

OS:
macOS

Browsers:
- Google Chrome
- Safari

Test Card:
4242 4242 4242 4242

## Features to Test

- Phone number validation
- Birth date validation
- Guest account creation
- Membership purchase
- Profile editing validation
- Cross-browser behavior

## Test Data

Valid email address  
Invalid phone numbers (letters, symbols)  
Empty phone field  
Empty birth date field

## Risks

Users may create memberships without valid contact information.

This may cause issues with:

- customer communication
- support requests
- account management
