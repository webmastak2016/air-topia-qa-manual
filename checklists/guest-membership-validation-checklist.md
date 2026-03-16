# Checklist – Guest Membership Validation

## AIR-362 (Test Guest creation without missing contact information)

## Registration Validation

- [ ] User cannot continue without phone number
- [ ] User cannot continue without birth date
- [ ] Phone field accepts only numeric characters
- [ ] Phone number length validation works
- [ ] Invalid characters are rejected

## Membership Purchase

- [ ] Membership cannot be purchased without required fields
- [ ] Checkout validates user contact data
- [ ] Payment flow works with valid information

## Profile Editing

- [ ] Phone number cannot be removed if required
- [ ] Birth date cannot be removed if required
- [ ] System validates required fields during checkout

## Cross-Browser Testing

- [ ] Chrome behavior verified
- [ ] Safari behavior verified
