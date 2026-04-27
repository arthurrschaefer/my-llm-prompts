# Task: Audit X followers and remove inactive users, requiring my confirmation first, while strictly simulating human behavior.
# Start state: Browser open on X.com "Followers" page.

# CRITICAL ANTI-BOT RULES:

- You must simulate human pacing to avoid triggering X's bot detection.
- Wait a random amount of time (between 3 and 8 seconds) after opening a new tab before reading its contents.
- Wait a random amount of time (between 2 and 5 seconds) before clicking any menus or buttons.
- Do not rush. Execute all actions deliberately and erratically like a human.

## PHASE 1: SCANNING (Do not remove anyone yet)

Execute this loop for a batch of the next 50 followers on the list:
1. Middle-click (or Ctrl+Click) to open the follower's profile in a new tab.
2. Switch to the new tab and WAIT 3 to 8 seconds.
3. Check for a verification badge (a blue, gold, or grey checkmark) next to their display name. Note if it exists.
4. Check the date of their most recent post.
5. IF the last post is >3 months old OR there are no posts: 
   a. Add their @handle to a "Pending Removal List".
   b. IF you noted a verification badge in step 3, append the tag "[VERIFIED]" next to their handle on the list.
6. WAIT 2 seconds, then close the profile tab.

## PHASE 2: CONFIRMATION
1. Print the full "Pending Removal List" to me. 
2. Ask me exactly this: "Please confirm this list. Are there any accounts here I should NOT remove? (Note: I have tagged verified accounts for your review)."
3. PAUSE AND WAIT for my reply. Do not proceed until I approve.

## PHASE 3: EXECUTION

After I reply with the approved list:
1. Navigate to the first approved profile and WAIT 3 to 5 seconds.
2. Click the 3 dots menu -> WAIT 2 to 4 seconds -> Click "Remover seguidor" -> WAIT 2 seconds -> Click confirm (if a modal appears).
3. Keep a running list of what you have successfully removed.
4. Repeat for the next approved profile, ensuring you pause randomly between profiles.
5. Output the final "Removed List" when finished.