# Evil-Portal_Dream-Survey
A non-malicious homage to the Willamette Valley Dream Survey for Flipper Zero Evil-Portal. Tempt people into joining your mysterious AP, and share their dreams.
Some people may know the dream survey from dumb youtuber conspiracy theories surrounding FUTEL, who had nothing to do with it.
Futel is a super cool non-profit keeping payphone and phreak culture alive: https://futel.net/ . they just added it to their directory because it was strange.
I have included a jpg of one of the original posters for reference.

Evil Portal waits for a request with email and password params. In this code we use adventurer and dream, and then reassign before sending the request:
```
                const email = adventurer;
                const password = dream;
                const url = `/get?email=${encodeURIComponent(email)}&password=${encodeURIComponent(password)}`;
```

The default text in the boxes are placeholders in the form. Simply change the placeholder here:
```
            <input type="text" name="adventurer" placeholder="Adventurer">
            <textarea name="dream" placeholder="Describe your dream here..."></textarea>
```

Feel free to brainstorm other non <>< related things to do with evil portal. Think outside the box.
