---
title: Check the verification code
description: Check that the code that the user entered is the same one that was sent
---

# Check the verification code

To verify the code submitted by the user you make a call to the [Verify check endpoint](/api/verify#verifyCheck). You pass in the `request_id` (which was returned by the call to the Verify request endpoint in the previous step).

The response tells you if the user entered the correct code. If the status is zero then the code they entered is the same one that they were sent. In that case, create a user session object.

After checking the code, return your user to the home page.

Enter the following code in the `/check-code` route handler to achieve this:

```python
# Some Python code here
```