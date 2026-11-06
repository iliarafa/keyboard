# Type a Tune

A typing game for kids in 3rd grade and up. It teaches typing with a steady,
even rhythm instead of racing for speed.

Every correct key plays the next note of "Twinkle, Twinkle, Little Star" and
puts a star in the night sky. When the beat is steady, the stars are evenly
spaced and the song sounds right. When the typing stops and starts, the song
stumbles and the gaps show up in the sky.

## Play it

Open `index.html` in any modern browser (Chrome, Edge, Firefox or Safari).
There is no install, build step or account. It needs a physical keyboard and
works well on Chromebooks.

## How it teaches

- **Six lessons on the home row**, one finger pair at a time: F J, D K, S L,
  A ;, G H, then real home-row words. Each lesson is 48 keys, one key for each
  note of the song.
- **The flow score measures rhythm directly.** The game times the gap between
  keys and compares each gap with the player's own recent beat (the median of
  their last 8 gaps). Being on the beat scores 1.0. Being 50% late scores about
  0.57. Speed doesn't matter, only evenness.
- **The music gets fuller as flow improves.** At 50% flow a bass line joins
  in, and at 75% sparkles are added.
- **A ghost star shows when the next note is due**, based on the player's own
  pace, so there is no fixed metronome to fall behind.
- **Mistakes don't stop the song.** A wrong key makes a soft thunk and the
  letter is marked. The player can keep going or retype the missed letter right
  away to fix it.
- **Pauses tell the game something.** A long hesitation before a key, or a miss,
  flags that key, and the results screen lists up to three keys to practice.
  A pause longer than 5 seconds counts as a break and isn't penalized.
- **An on-screen keyboard and hands** are colored by finger, and they light up
  the finger to use for the next key.

## Stars

| Stars | Needs |
| --- | --- |
| ★ | Finish the song |
| ★★ | Flow 60%+ and accuracy 85%+ |
| ★★★ | Flow 75%+ and accuracy 93%+ |

The best stars for each lesson are saved in the browser's local storage, on
that device only. No data leaves the computer.
