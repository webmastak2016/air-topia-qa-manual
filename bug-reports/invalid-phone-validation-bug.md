# Bug Report – Invalid Phone Number Accepted in Guest Membership Flow

## AIR-362 (Test Guest creation without missing contact information)

## Environment

URL:
https://staging.airtopiaparks.com/guest/explore/memberships

Device:
Mac mini (Apple M4)

OS:
macOS

Browser:
Google Chrome

## Summary

The phone number field validation appears incorrect. The field accepts up to 16 characters including letters and special characters, and the user can still proceed to the next step with an invalid phone number.

## Steps to Reproduce

1. Open the Guest Explore Memberships page.
2. Start the membership signup flow.
3. Enter an invalid phone number (letters or symbols).
4. Continue to the next step.

## Actual Result

The form allows the user to proceed even with an invalid phone number.

## Expected Result

The system should restrict the phone field to a valid numeric phone format and prevent proceeding until a valid number is entered.

## Potential Impact

Users may be able to complete the membership purchase without a valid contact phone number.

## Attachments

### Step 3 – Invalid phone number entered

![Invalid phone input](../screenshots/phone-validation-guest-membership-step3.png)

### Step 4 – System allows proceeding with invalid phone number

![Form proceeds with invalid phone](../screenshots/phone-validation-guest-membership-step4.png)
