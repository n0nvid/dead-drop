# dead-drop

    quod tegitur, aperitur.

Two sealed messages.

**`videtur.txt`** — a `gpg` symmetric message. You already hold the passphrase:
it's my fingerprint (40 hex characters, no spaces). Decrypt it:

    gpg -d videtur.txt

Inside is where we talk when it has to be quiet. Say hello there.
Ask, and the way forward will find you.

**`final.txt`** — also sealed, but the fingerprint won't open this one.
Its word only travels through the quiet channel above. Come back when you have it:

    gpg -d final.txt
