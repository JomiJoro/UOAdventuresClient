# Ultima Adventures 3.2 — Elves & Gargoyles Patch

Heyo! This is a small patch for [Ultima Adventures 3.2](https://github.com/FinalTwist/Ultima-Adventures/tree/main) that adds **Elf and Gargoyle buttons to character creation**.

## What's Included?

- **Elves:** Button for Elves
- **Gargoyles:** Button for gargoyles, but you'll need to make major changes to your server to have them work (they just become human).
- **Client files:** Includes the modified Gumpart & Gumpidx needed for the new character creation buttons.

## Client Installation

If you already have the server and client, good news, you can keep all your saves and just modify 3 files.

You have two options:

**Option 1 — Replace the Data Files folder**
- Replace your client's existing `Data Files` folder with the one included in this patch.

**Option 2 — Replace only the required files**
- Replace `Gumpart.mul` and `Gumpidx.mul` with the versions included in this patch.

Choose whatever.

## Server Setup — Enabling Races

To enable other races you do need to make a small change to the server code.

1. Open `CharacterCreation.cs` in your Ultima Adventures server folder.
2. Find the character creation code around line 132.
3. Change the race assignment to:

   ```csharp
   newchar.Race = args.Race;
   ```

4. Rebuild if linux (no idea if required I did anyways) and restart your server.

## Never played the client yet?

You can download and use the client included in this repository, but if you have a client rip your macros. I only included Tazuo because I hate razor.

## 📝 Additional Notes
- No I probably won't fix gargoyles, this was just a 2 second patch I figured out.
- The Elves appear to function like humans (no night vision) other passives are untested.
- So basically Elves might just be cosmetic, but this is an rpg so of course I want it still.
