# dead-drop

    quod tegitur, aperitur.

Two sealed messages.

**`videtur.txt`** — a `gpg` symmetric message. You already hold the passphrase:
it's my fingerprint (40 hex characters, no spaces). Decrypt it:

    gpg -d videtur.txt

Inside is a pointer to the next drop. Follow it.

**`final.txt`** — also sealed, but the fingerprint won't open this one.
Its passphrase waits at the drop above. Come back when you have it:

    gpg -d final.txt
