## How to Use
1. Fork this repository.
2. Go to [LeetCode](https://leetcode.com) and log in to your account
3. Open Developer Tools (F12 or right-click -> Inspect)
4. Go to the Application tab and refresh the page
5. In the Cookies section, find:
   - `LEETCODE_SESSION`
   - `csrftoken`
6. In your repository's Settings → Secrets and Variables → Actions, add:
   - `LEETCODE_SESSION` (from cookies)
   - `LEETCODE_CSRF_TOKEN` (from cookies)
7. In Settings → Actions → General, enable 'Read and write permissions'
8. The workflow runs daily at 15:00 UTC to update your stats. Go to the actins tab and ensure the workflows are not `disabled`
9. If you want to run it manually, to see your stats and solutions organized quickly, then go to the `Actions` section and run the #1 successfully twice. Then run #2 and #3 and it will work. 

## Credits
This project uses [LeetCode Sync](https://github.com/marketplace/actions/leetcode-sync) to fetch solutions, runtime, and memory usage data from LeetCode.
