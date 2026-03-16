# Upon the Matter of Why This Fork Was Necessitated: A Grievance Most Foul

I beseech thee, dear reader, to lend me thine ear, for I have suffered an injustice so profound, so utterly unconscionable, that it would move even the most hardened of souls to weep.

I am employed at a grocery establishment. Each and every day, it falls upon my wretched person to conduct what is known in the common tongue as a "gapscan", that is to say, I must traverse the aisles with scanning apparatus in hand, cataloguing the barren voids upon the shelves where product ought to reside. A task of no great complexity, one would think. One would be CATASTROPHICALLY MISTAKEN.

For you see, within the entirety of our establishment, there exist but THREE Honeywell PDE scanning devices. Three! For an ENTIRE STORE! And each morning a most undignified scramble ensues, not unlike the Hunger Games but with significantly less glamour and considerably more passive aggression. The scoundrel from produce has already absconded with one unit before dawn. The night-fill brigand has secreted another away in some forsaken cage in the back dock. And the third? Its battery has perished at approximately 6am because NOT A SINGLE SOUL saw fit to place it upon its charging cradle. These wretched devices run Android 4, I shall have you know. ANDROID 4. They crash with such regularity that one begins to suspect they are doing it deliberately out of spite.

And so I am left standing there, scannerless, a man most bereft, whilst gaps accumulate upon the shelves like dust upon a neglected mantelpiece. And then, oh THEN, the customers descend upon me with their accusations. "WHERE IS MY ITEM" they bellow, as though I have personally consumed it, as though I am hoarding tins of baked beans beneath my vest for my own nefarious purposes. And apparently, APPARENTLY, it is ALL MY FAULT that the shelves are bare. Not the fault of there being three functioning scanners for an entire commercial operation, oh no.

And what of Metcash, you ask? Metcash, who are almost certainly EVIL, for they have steadfastly, resolutely, and with great prejudice REFUSED to furnish us with new PDE units. "Simply share them" they proclaim from their ivory towers. "Coordinate more effectively" they suggest, as though Dave from dairy did not literally take the last scanner home in his trouser pocket last Tuesday.

And so, driven to the very precipice of madness, I took matters into my own hands. I purchased, WITH MY OWN COIN, a Google Pixel telephone. I then proceeded to flash upon it my own custom ROM, because naturally the stock configuration was entirely insufficient for the task at hand. I then, through considerable tribulation, managed to configure Microsoft's BC Live PDE client upon the device, which was an odyssey unto itself. And THEN, upon discovering that the BC Live interface possesses absolutely NO capability for camera-based barcode scanning whatsoever, I was compelled to locate this keyboard wedge application, only to discover that it employed an ancient, abandoned barcode library with acquisition so abysmal that one would achieve superior results simply typing the numbers in by hand.

Thus I was left with no recourse but to gut the entire application like a fish. I ripped out ZXing and replaced it with Google ML Kit. I integrated CameraX. I configured it to scan ONLY actual product barcodes, lest it go absolutely feral upon every QR code in sight (the Honeywell guns, in their infinite wisdom, open a BROWSER WINDOW each time one accidentally scans a QR code, which adorns literally every product manufactured in the modern era, truly INSPIRED engineering choices there Honeywell, BRAVO). I implemented a volume-down trigger mechanism so the scanner does not read every barcode within a two metre radius as I merely walk past. And I added auditory and haptic confirmation so that I might actually know when something has been successfully scanned.

All of this. Every last bit of it. Simply so that I might perform the duties of my employment. You are most welcome, customers of my store. Your items shall be stocked henceforth.

---

# Android Barcode Keyboard

This Android app registers an input method that you can use like any other Android keyboard.
However, instead of keys it shows a camera window. Whenever a barcode (1D codes, QR, DataMatrix, …)
is inside the camera view, the barcode content will be inserted into the current text fields.

Similar apps already exist, but show lots of ads, require in-app purchases to remove ads, and
have the risk of leaking your data. This app is free and open source and does not even request
permission to connect to the internet from the operating system. You can therefore fully trust
this app not to send your QR code data somewhere.

## License

Copyright 2020 Raphael Michel. Apache License 2.0.

Based on dm77/barcodescanner-view and ZXing by Google (both Apache License 2.0).
