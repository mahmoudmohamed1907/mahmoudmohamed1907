- 👋 Hi, I’m @mahmoudmohamed1907


<!---
mahmoudmohamed1907/mahmoudmohamed1907 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

fix: prevent racing of requests
Introduce a request id and a reference to latest request. Dismiss
incoming responses other than from latest request.
Remove timeouts which were used to mitigate the racing issue but are
obsolete now.
