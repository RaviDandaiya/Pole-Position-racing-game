Walkthrough - Level System, Voice & Animation
I have implemented a complete level progression system for the Retro Racer game.

Changes Made
1. Level HUD
Added a new Level panel to the HUD.
The panel updates in real-time as you advance.
2. UI Layout & Mobile Optimization
Compact HUD: Reduced font sizes and panel padding to maximize road visibility.
Mobile Controls: Repositioned joystick buttons to the bottom of the screen with semi-transparency.
Improved Spacing: Fixed overlap between HUD panels and mobile buttons.
3. Level Up Splash Animation
Implemented a premium #level-splash overlay.
Uses a "pop-in" scale animation with cubic-bezier easing for a professional feel.
Appears for 2 seconds when you cross the finish line.
3. Boost Mechanic (Nitro)
Control: Hold SPACE to activate Nitro.
Visuals: Dynamic cyan exhaust flames appear behind the car.
Physics: Speed increases up to 150% of normal MAX_SPEED.
Management: A new Nitro Meter in the HUD tracks your boost level (refills slowly when not in use).
4. Gameplay & UI Enhancements
Smoother Overtaking: Reduced AI car hitboxes by 25%, making it much easier to pass traffic.
Premium HUD: Panels now have glowing borders and a glass-morphism effect.
Dynamic Splash: The Level Up animation is now multi-stage with a "pop and shine" effect.
5. GitHub Integration
Repository: Pole-Position-racing-game
Latest Commit: Included all gameplay, level system, and UI enhancements.
Verification
Overtaking: Passing cars is now fluid and feels less "sticky".
Boost: Verified that holding Space increases speed significantly and depletes the nitro bar.
UI: HUD elements glow on hover and the Level 2+ transition is much more impactful.
Level Transition
When the player crosses the track length, 
levelUp()
 is triggered:

gameState switches to STATE_COUNTDOWN.
The Level Splash is shown.
Voice announces the new level.
Track resets and traffic is re-randomized.
HUD Visuals
The new HUD features custom-styled glass panels with real-time Nitro and Level tracking.

How to Play
Click RACE START.
Hear the voice announce "Level 1".
Reach the end of the track.
Watch the "LEVEL 2" animation and hear the announcement.
Continue racing!
