## My Journey Developing a Script with GitHub Copilot

### Phase 1: Diligent Manual Booking—Early Mornings and Multi-Device Sync

At first, I relied on hard work, waking up early every day to try to book courts as soon as reservations opened. I would synchronize my attempts on both my phone and computer, hoping to improve my chances.

### Phase 2: The Phone’s Advantage

Soon, I discovered that booking via my phone was consistently faster than on my computer. The culprit seemed to be the computer’s need to navigate through date and time selectors, slowing the process down significantly.

### Phase 3: The Rise of Scripts and New Motivation

As summer arrived, the demand for air-conditioned courts at the West Gym soared, and scripts became popular among players. Suddenly, it became almost impossible to secure a spot manually. I realized that some people around me were already using scripts, but out of pride, I hesitated to ask them for help. Still, the idea of developing my own script began to take root.

### Phase 4: Starting from Scratch (With a Little Python)

With no background in Java and not being a computer science major, I only had a bit of basic Python knowledge from my undergraduate days. My only real ally was the latest AI technologies being developed abroad.

### Phase 5: Gaining Access to GitHub Copilot

I applied for GitHub’s student program to get access to GitHub Copilot. (There are detailed tutorials on Bilibili about the application process.)

### Phase 6: My First AI-Powered Script

When I started using AI to write scripts, I had no real plan—just hoping for a lucky break. I provided the AI with website screenshots and URLs, asking it to generate a script. Amazingly, it produced a working script (version 1.0) that could be run in the browser console (F12).

### Phase 7: Script 1.0—The Click Simulator

Script 1.0 used a simple approach: simulating mouse clicks to repeatedly look for and press the “Book Now” button at scheduled times. But the button recognition was too slow, and navigating through pages after entering the website was still a major hurdle.

### Phase 8: Manual Button Clicks and Page Redirection—Script 2.0

To address this, I decided to handle the “Book Now” button manually and let the script automate the subsequent page redirection steps (Script 2.0). All I had to do was provide the AI with the reservation and target page links, and it would generate a redirection script—a simple and effective solution.

### Phase 9: Limitations of Redirection and the Power of Tampermonkey

Redirection worked, but I still couldn’t bypass the initial “Book Now” button. Running scripts in the browser console was also problematic, since the console clears on page refresh, interrupting the script. I discovered that using a browser extension like Tampermonkey could solve this, and at this point, my script began to take real shape.

### Phase 10: Early Success, But Not Guaranteed

The script was functional and allowed me to occasionally secure a spot, though not always—there was still an element of luck. Fortunately, script use hadn’t become rampant yet, so I could still get a court from time to time.

### Phase 11: First Optimization—Closing the Reservation Notice Popup

My first optimization attempt was to handle the reservation notice popup, which was an image that loaded slowly. I tried scripting the popup’s closure, but it was too slow. Eventually, I realized it wasn’t necessary to click “Confirm”—just closing the popup was enough, so I dropped this optimization.

### Phase 12: Second Optimization—Streamlining Partner Selection

The next optimization was much simpler: automating the selection of playing partners. This took just a few dozen lines of code.

### Phase 13: Third Optimization—Auto-Selecting Courts (And Its Limits)

I tried to automate court selection by identifying available slots or always booking the same court. However, these solutions were slower than manual clicking. Even after selecting a court, the script’s click on the “Book” button lagged, so I abandoned this approach.

### Phase 14: A New Approach—Form Submission, Then System Roadblocks

Changing tactics, I asked AI to analyze the “Book” button, discovering it submitted a form. I wrote a script to simulate form submission, but the system blocked it—apparently, anti-script mechanisms had been added to prevent automated bookings. I had to stop pursuing this line of development.

### Phase 15: The Final Version—A Race Against Ever-Improving Defenses

With my final version complete, the university updated the booking system in response to student complaints, strengthening its anti-script monitoring. More advanced scripts emerged, making it even harder for mine to stand out. Sometimes, booking manually on a phone was actually faster than using my script. At this point, I could only rely on luck—occasionally securing a spot, but generally getting in once or twice a week at best.

---

Looking back, using AI and GitHub Copilot to develop my script was a journey full of learning, trial and error, and adapting to ever-changing challenges.
