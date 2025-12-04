# RCA003 – Dashboard Display Bug Escaped in DEV

## 📝 Summary
Dashboard charts and metrics were incorrectly displayed in DEV due to untested code deployment.

## 🔍 Root Cause
- Developers did not verify UI rendering on multiple screen sizes
- CSS and JS conflicts were not caught
- No automated UI test for this dashboard

## ⚡ Impact
- Users saw incorrect metrics
- Sprint review screenshots were inaccurate
- QA time spent troubleshooting instead of testing new features

## 🛠 Actions Taken
- Fixed UI rendering issues
- Added automated visual regression test for the dashboard
- Shared RCA findings with Dev team to reinforce post-development testing

## ✅ Lessons Learned
- Always verify UI across screen sizes
- Automated visual tests reduce escapes to DEV
- RCA should be used to educate and prevent repeated mistakes
