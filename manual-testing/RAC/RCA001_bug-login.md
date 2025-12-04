# RCA001 – Login Bug Escaped in DEV

## 📝 Summary
A login bug was detected in the DEV environment that was not caught by developers before deployment.

## 🔍 Root Cause
- Missing validation for empty password field
- Developers did not perform post-development tests
- Automated tests did not cover this edge case

## ⚡ Impact
- Users could not log in during QA execution
- Delayed sprint testing schedule
- Highlighted gaps in the testing process

## 🛠 Actions Taken
- Added validation for empty password field
- Included this scenario in manual and automated tests
- Communicated the need for Devs to test before pushing

## ✅ Lessons Learned
- Developers must validate critical flows in DEV
- Edge cases should be included in automated tests
- RCA reports prevent repeated mistakes
