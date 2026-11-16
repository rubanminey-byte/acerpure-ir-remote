# Acerpure Cozy F2 (AF773) Android IR Remote

A standalone Android Kotlin app built around `ConsumerIrManager` that duplicates every button on the default **Acerpure Cozy F2 2-in-1** remote:

- **Power** (On / Off)
- **Speed + / Speed -** (1–16 steps)
- **Left / Right Swing** (30° / 60° / 90°)
- **Up / Down Swing** (90° vertical)
- **Mode** (Eco / Sleep / Turbo + 3-second hold for Child Lock via NEC repeat frames)
- **Timer** (1 / 2 / 4 / 8h)

## Built-In Code Finder (No External Hardware Needed)

Because Android phones only have a transmit-only IR blaster and Acerpure Cozy F2's raw NEC hex codes are not published in public IR databases, the app includes an interactive **Code Finder**:

1. Open the project in **Android Studio** and install it on your phone via USB debugging (or **Build > Build APK(s)**).
2. Enter an NEC hex address (start with `00`, `01`, `02`, `04`, `08`, `10`, `20`, `40`, `80`, or `FF`) and tap **Auto Scan** while pointing your phone at the fan.
3. Once the fan responds, select each button in the dropdown (**Power**, **Speed +**, **Speed -**, **Swing L/R**, **Swing U/D**, **Mode**, **Timer**), step through commands with **Next** / **Auto Scan**, and tap **Save Current Code to Selected Button**.
4. Use **Export JSON** to back up your mapped profile.
