# Case Study: Outbreak: IT Room at a High School Career Talk

**A scan-to-play IT escape room, rebuilt the morning of the talk to match what the class was learning, that students came back to replay the next day**

| | |
|---|---|
| **Event** | Virtual career talk, Firelands High School senior class |
| **Date** | Monday, November 16, 2026 (about 26 minutes, over Google Meet), with student replays on November 17 |
| **My role** | Speaker, game designer and host |
| **Game** | Outbreak: IT Room, Tech+ Edition (now called the Rookie Edition) |
| **Stack** | One static HTML page on GitHub Pages, a Google Form for results, a Google Sheet leaderboard |
| **Source** | [PurpleFlagg/outbreak-escape](https://github.com/PurpleFlagg/outbreak-escape) |

---

## The goal

I was invited to give a short virtual career talk to a high school senior class that was early in its CompTIA Tech+ training. I didn't want 26 minutes of me talking at a screen. I wanted students to actually *do* some IT, have fun with it, and leave thinking "I could do this job."

The plan was a quick, game-style activity that:

- used skills the students had **already learned**, so they could win
- worked over a video call, with no installs and no accounts
- let students play on their own phones **or** together as a class
- recorded results so I could see how it went afterward

## The game

**Outbreak: IT Room** is a zombie-themed escape room. The zombies are breaking through the door of the IT room, and the only way out is through the vents. Each vent section is sealed by a "lock," and each lock is an IT skill check.

The Tech+ Edition the class played has five locks:

| Lock | Skill | What players do |
|---|---|---|
| 1. Computing cycle | Input, processing, output, storage | Sort parts (keyboard, CPU, monitor, SSD, microphone) into the right step |
| 2. Passwords | Account security | Pick the strongest password, the safest way to manage 30 passwords, and name two-factor authentication |
| 3. Privacy and encryption | Data and privacy | What encryption does, app permissions, what the browser lock icon means, what to do when you forget a work password |
| 4. Binary | Networking basics | Decode an IP address sent in binary, with a tap-the-bits decoder |
| 5. Spotting scams | Social engineering | Match situations to phishing, vishing, smishing, tailgating and shoulder surfing |

**How it plays**

- **Scan to play.** A QR code on my slide opened the game in any phone browser.
- **Two modes.** *Solo* (each player on their own phone, answer order shuffled) or *Team* (one game on the big screen for the whole room).
- **A 15-minute clock.** Each wrong answer makes the zombies "surge" and costs 10 seconds. Hints are free, so nobody gets stuck.
- **No dead ends.** If the clock runs out, players can choose "Keep going without the clock" and still finish.
- **Live leaderboard.** When a player or team cracks all five locks, the game sends their time, hints used and zombie surges to a Google Form, which feeds a ranked Google Sheet.
- **Host answer key.** A built-in answer key lets the host steer the room without slowing it down.

## Building it for this class

The original Outbreak game was aligned with **CompTIA A+**. A few days before the talk, the teacher shared what the class had covered so far in Tech+: the computing cycle, computing devices, understanding data, data privacy, encryption basics, password management, privacy settings and resetting a Windows password.

That list didn't match the A+ version, which leans on hardware diagnosis, port numbers and help desk tickets. So the **morning of the talk** I built a separate Tech+ Edition with easier locks matched to those topics, a longer clock and free hints. Shortly after, I added Solo and Team modes.

I also asked the teacher a simple question ahead of time: **solo or as a class?** The teacher recommended playing as a class on the room's big display, so the adults in the room could help and give hints. That became the main plan, with Solo mode still open to anyone who wanted to follow along on their phone.

## How it ran

The talk covered where I work, how I got into IT, and why soft skills matter, plus time for student questions. For the game, I shared my screen and we played Outbreak **together as one class**, on the room's big display. Students who wanted to also scanned the QR code and **played along on their own phones** at the same time.

## Results, day 1: in class (November 16)

> **Read this first:** most of the class played *together* on the shared screen, so the leaderboard does **not** represent the whole class. It shows the students who also played along on their own phones (and any group that finished as a team). The game only logs a result when all five locks are cracked, so runs that were started but not finished aren't counted.

**How I picked the rows:** I kept every leaderboard entry submitted on November 16 between 12:12 and 12:14 PM ET, right as the talk wrapped up (scheduled 11:44 AM to 12:10 PM). All five are tagged as the Tech+ Edition. I left out an entry from about four hours later, logged while I was editing the game that afternoon.

| Metric | Result |
|---|---|
| Finished escapes logged | **5** (4 Team, 1 Solo) |
| Finished within the 15-minute clock | **4 of 5** |
| Finished after the clock ran out ("keep going") | 1 |
| Fastest escape | **9:13** |
| Median escape time | **11:44** |
| Slowest escape | 16:37 |
| Hints used | 5 total (2 runs used none) |
| Zombie surges (wrong answers) | 9 total (2 runs had none; 1 run had 7) |
| Perfect run (no hints, no wrong answers) | 1, in 10:20 |

All five results arrived within about 80 seconds of each other. That fits how the session ran: the students on their phones were following along with the class game, so they finished at about the same time.

*Times include the 10-second penalty for each wrong answer. Player and team names are left out on purpose.*

## Results, day 2: students came back to replay (November 17)

The next day, 10 more runs showed up on the leaderboard between 11:49 AM and 12:02 PM ET, all in Solo mode. I hadn't shared the game link anywhere else, so these were Firelands students going back to play again the day after the talk.

By then the game had been renamed the Rookie Edition, with a refreshed look and a shorter 10-minute clock. The five locks and their questions were the same ones the class played on day 1.

| Metric | Result |
|---|---|
| Solo runs logged | **10**, from 4 player names |
| Players who played more than once | **3 of 4** |
| Finished within the 10-minute clock | **10 of 10** |
| Zombie surges (wrong answers) | **0** in all 10 runs |
| Hints used | 5 total (6 runs used none) |
| Fastest escape | **0:37** |
| Median escape time | **1:19** |

Each player's first run compared with their best run:

| Player | Runs | First run | Best run |
|---|---|---|---|
| Player A | 4 | 6:40 | **0:37** |
| Player B | 3 | 2:53 | **0:57** |
| Player C | 2 | 8:01 | **3:02** |
| Player D | 1 | 1:26 | 1:26 |

Some of that speed comes from knowing the puzzles by the second or third try. Solo mode shuffles the answer order on every run, though, so players still had to recognize the right answer each time, not just tap the same spots. Every player who replayed beat their own first time.

*Players are labeled A to D on purpose. No names are shared.*

## What I learned

- **Meet students where they are.** The best change I made was rebuilding the game around what the class had actually studied. Students could win with what they already knew, and that's what makes a career talk feel like "I could do this."
- **Ask the teacher.** One short question (solo or as a class?) shaped the whole activity. The teacher knows the room better than any plan I can make from the outside.
- **Design for both ways of playing.** Team mode on the big screen kept everyone in it together, and Solo mode gave students who wanted more a way to play on their own phones. The same page handled both.
- **Never leave anyone stuck.** Free hints and "keep going without the clock" meant every group could reach the end. One group finished after the clock ran out, and that still counts as escaping.
- **Replay is great feedback.** Students coming back the next day to play again, and getting faster each time, says the game stuck with them. Keeping it free to replay on a phone, with a leaderboard to chase, made that easy.
- **Know what your data can and can't say.** A finish-only leaderboard is great for a fun ranking, but it can't tell you how many people started, where they got stuck, or how many students were behind one phone.

## Next steps

- [x] Rename the editions to **Rookie** (the Tech+ version) and **Technician** (the A+ version), and add a CompTIA trademark notice
- [x] Shorten the Rookie clock to 10 minutes
- [ ] Log when a run *starts*, not only when it finishes, so I can see how many players finish
- [ ] Add an optional session or class code, so results from different talks don't mix on one leaderboard
- [ ] Record which lock each wrong answer happened on, to see which skills students find hardest

## Built with

HTML, CSS and JavaScript in a single page, hosted on GitHub Pages · Google Forms and Google Sheets for the leaderboard · a QR code for scan-to-play

---

*CompTIA, A+ and Tech+ are trademarks of CompTIA, Inc. Outbreak: IT Room is not affiliated with or endorsed by CompTIA.*
