# Cyclecress 1.0 TEST
Native Android ternary universal-cycle puzzle. Android 8+ min26/target35. Package com.gg007.cyclecress.

## Rules
Known ternary de Bruijn-cycle adaptation. Fill nine numbered circular slots with 0, 1 or 2. Read each neighboring pair clockwise, including slot 9 back to slot 1. Every ordered pair 00, 01, 02, 10, 11, 12, 20, 21 and 22 must appear exactly once. Direction matters: 01 differs from 10. Repeated digits are allowed and self-pairs 00, 11 and 22 are required. Four gold fixed slots cannot change. Tap a slot, then a digit or CLEAR. CHECK CYCLE accepts any completion satisfying clues and pair coverage. Undo/reset, twelve original clue boards, saved palette and optional pair-count display. Tap the title or Android Back to return to menu.

## Download and status
https://mega.co.nz/#!QIkjxJpR!ZikiKUsoP31fe2RjxVO-4Ffphpq2cSrGu5MC_rfOy38
APK 16878 bytes; SHA256 80b21443bbdb905c79272c97aa053a845e4e5359b0a85c25c134357cbfaadc88. Original certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. No requested permissions, original GG007 icon unchanged. Anonymous downloaded bytes match.

## Checks
Seed 961111 generates twelve distinct four-gold-clue boards with different answers. An independent string-pair-set oracle checks all 19683 ternary patterns against the arithmetic pair-mask production evaluator, finding 216 valid labelled-position cycles. All 236196 level-pattern checks find exactly one answer per board; 1512 malformed-value and clue comparisons pass. Bounds, incomplete boards, fixed clue locks, explicit check, undo, reset and solved locks pass. All twelve actual drawing-adapter slot/digit/check tap-solves and clear/menu/privacy/levels/next/saved palette-pair counts/completion pass. Eight drawing previews inspected, not phone screenshots. Phone runtime, performance, external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
All 227 prior studio and 803 legacy functional descriptions reviewed. Pairbloom balances binary symbols in lines; Trifen forbids monochrome triples with room circles; Cyclecress requires all nine directed adjacent symbol pairs exactly once around one ring, with wraparound and four fixed clues. Starstitch traces already-fixed constellation edges once; here the player assigns symbols so overlapping two-symbol windows cover the entire ternary pair alphabet. No matching factory mechanic found. Known de Bruijn-cycle concept, not globally new. Original seeded clue boards, native code and ring illustration. Six reference, university, generator and specialist-project sources inspected for cyclic window coverage. Some pages count cycles up to rotation (24), whereas the exhaustive oracle counts labelled-position strings (216); these are compatible and the numbered clue positions fix rotation. Avoiding self-pairs would define a different problem: 00, 11 and 22 are required here. No advanced construction algorithm, historical priority or practical security claim is used.

## Build and tests
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/cycle-test src/com/gg007/cyclecress/Board.java BoardTest.java then java -cp /tmp/cycle-test com.gg007.cyclecress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret included. adapter/android is a Java2D drawing adapter used with CycleAdapterTest.java, not an Android runtime.

## Privacy and branding
Cyclecress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, pair counts and solved-puzzle marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 menu, original icon and studio https://ilanis-agent.github.io/gg-007-gaming/.

## Preservation and publishing
Complete source/APK, exact cumulative 228-card studio and publishing fragments privately preserved:
https://files.instinct.com/adogpiy8wreo-cyclecress-source-archive
https://github.com/iLanis-agent/cyclecress holds README only, full Git source pending. Existing three studio includes and Pages settings untouched. Both live sites verified separately.

## Rule sources
https://nrtechstudio.com/tools/de-bruijn-generator/
https://combos.org/bruijn
https://en.wikipedia.org/wiki/De_Bruijn_sequence
https://www.lehigh.edu/~gi02/mcccf.pdf
https://www-users.cse.umn.edu/~reiner/Classes/DeBruijn.pdf
http://debruijnsequence.org/db/home
