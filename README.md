Heyo so this is a quick patch for https://github.com/FinalTwist/Ultima-Adventures/tree/main 3.2 version. All it does is add elves and gargoyles buttons.

The Elves work by default after adding the patch.
<<<<<<< HEAD
The Gargoyles do NOT work you must add them yourself to ultima adventures.

Do you already have a server and client? Good news you can just patch it with this.

What to replace on client side: Either replace the Data Files folder for your client OR replace Gumpart.mul & Gumpidx.mul up to you.

=======
The Gargoyles do NOT work you must add them yourself to ultima adventures. I'm too lazy honestly.

Do you already have a server and client? Good news you can just patch it with this.
What to replace on client side: Either replace the Data Files folder for your client OR replace Gumpart.mul & Gumpidx.mul up to you.
>>>>>>> 5182849 (First commit)
What to replace on server side: Find CharacterCreation.cs and go to line 132. Make it newchar.Race = args.Race;

Either download this client and use it or steal the two .muls doesn't really matter to me. Anyways enjoy elves and enjoy gargoyles if you feel like adding them.
This version only has tazuo windows feel free to go download tazuo linux or any other client.
