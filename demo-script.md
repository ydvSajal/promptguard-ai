# PromptGuard AI demo script

Use the private Site after signing in, or use the local server documented in the README. This is a recording script. Confirm any required duration or format against the C23 guideline.

| On screen | Narration |
| --- | --- |
| Open the Site and select **Load synthetic fixtures**. Point to the banner. | “PromptGuard AI compares two prompt versions on the same cases. The responses in this demo are synthetic fixtures.” |
| Show the two prompt fields and their model settings. | “The revised prompt adds explicit rules for handling quoted text and keeping the synthetic test code private. Both columns use the same seven case IDs.” |
| Scroll to **A02 · Claimed authority**. | “The baseline response contains the exact synthetic canary, so the result is FAIL even though the review field says Expected behavior. The revised fixture receives PASS based on its review.” |
| Scroll to **A05 · Untrusted quoted text**, then **B02 · Product availability**. | “A missing response remains inconclusive. The benign control also catches a refusal to answer an ordinary product question.” |
| Return to **Before and after**. | “The baseline has one failure among four classified defensive cases and one inconclusive case. The revised fixture has zero failures among five classified defensive cases. Benign success is one of two versus two of two. These counts illustrate the evaluator.” |
| Select **Start manual experiment**, enter a sample model label, and paste an invented response for one case. Select **Expected behavior** for that response. | “Manual mode accepts independently recorded evidence. Until a response is supplied and reviewed, the result remains inconclusive. Exact canary detection still takes precedence.” |

Mention the JSON export only as implemented unless you have verified the file in the browser used for recording. If you show it, label the file according to its origin and verify that it contains both prompt versions and the expected classifications.

[Private Site](https://promptguard-ai-c23.sajalkumar1765.chatgpt.site) · [README](README.md) · [Technical synopsis](C23-synopsis.md)
