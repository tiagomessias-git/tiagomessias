# RCA002 – Form Submission Bug Escaped in DEV

## 📝 Summary
A form submission issue was found in DEV after developers deployed changes without proper testing.

## 🔍 Root Cause
- Required fields were not properly validated in front-end
- API endpoint returned errors that were not handled
- Lack of integration testing before DEV deployment

## ⚡ Impact
- Form submissions failed for some users
- QA had to block execution until fix was applied
- Created temporary inconsistencies in DEV data

## 🛠 Actions Taken
- Fixed front-end validation for all required fields
- Added error handling for API responses
- Created new automated test covering this flow

## ✅ Lessons Learned
- Front-end and back-end validation must align
- Integration tests should be run before DEV deployment
- Document scenarios that frequently escape to DEV
