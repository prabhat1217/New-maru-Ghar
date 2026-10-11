# Maru Ghar — મારું ઘર (Gandhinagar)

આ source bundle માં પસંદ કરેલી premium 3D gold/silver branding, photorealistic property-style homepage, એ જ પસંદ કરેલો app icon, Firebase listing submission અને admin approval page સામેલ છે.

## GitHub repository માં મૂકવા
1. ZIP extract કરો.
2. અંદરના files/folders (`index.html`, `admin.html`, `assets/`, `.github/` વગેરે) repository `prabhat1217/Maru-ghar` ના root માં upload કરીને જૂના project files replace કરો.
3. `main` branch પર commit કરો. GitHub Actions માં **Build Maru Ghar Android APK** workflow ચલાવો અથવા push પછી ચાલે તેની રાહ જુઓ.
4. Workflow run માં **Artifacts → MARU-GHAR-ANDROID-APK** માંથી APK ડાઉનલોડ કરો.

## Firebase / admin
- Firebase project: `maru-ghar-gandhinagar-8dbe4`
- Listings collection: `listings`
- Admin page: `/admin.html`
- Admin panel માં Firebase Authentication નું Email/Password account વાપરો. માત્ર UID `yJYiuaUE3KXVLVuWqLyLRH5owQJ3` ને rules માં admin અધિકાર છે.
- `firestore.rules` source file માં સુધારેલી rules છે. આ ZIP મૂકવાથી Firebase Console ની live rules આપમેળે બદલાતી નથી. Live rules અલગથી publish/deploy કરવી જરૂરી છે.
- Firebase Authentication માં Email/Password અને Anonymous providers સક્રિય હોવા જોઈએ.
- Cloudinary unsigned preset `marughar_images` અને cloud name `t5gd6nts` config માં છે. Unsigned preset માટે upload restrictions લગાવેલી હોવી જોઈએ.

## મહત્વની સ્થિતિ
આ source bundle છે, live deployment અથવા successful APK build નો પુરાવો નથી. GitHub Actions run green થયા પછી જ APK build સફળ ગણવો. Firebase Console માં live rules અને test listing/approval ચકાસ્યા પછી જ production-ready ગણવું.
