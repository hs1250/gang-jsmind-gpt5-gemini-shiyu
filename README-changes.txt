Changes made (2025-10-23):
1) Symmetric left-right expansion like XMind for root children.
   - Implemented applySymmetricLayout(root): first half of Level-1 topics go to the RIGHT (top→bottom order), 
     remaining topics go to the LEFT (order reversed) so the overall order is CLOCKWISE by Markdown order.
2) Direction inheritance for deeper levels: children follow the side (left/right) of their parent branch.
   - This keeps entire branches on one side like XMind.
3) No UI changes required; works when importing Markdown via parseMarkdown().

How to revert: use mindmap.js.bak in the same folder.


4) Robust auto-wrap (2025-10-23 v3):
   - Added `enforceNodeWrapping()` and `setupWrapObserver()` in JS.
   - Observer will re-apply wrapping and trigger relayout whenever nodes change.
   - Avoids injecting code inside any template strings; fixes prior v2 load issue.


5)請Gemini Pro將【下載HTML】產生的網頁 節點文字過多時會斷字，是否可以改成【下載 HTML】將js及html一起封裝起來
   -https://gemini.google.com/app/048f331b93309995
