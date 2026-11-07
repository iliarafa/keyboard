# Type a Tune

A touch-typing trainer that scores rhythm instead of raw speed. It is built for
learners from about 3rd grade up.

Every correct key plays the next note of a song. When the pace is even, the
melody sounds right and the timing chart shows evenly spaced bars. When the
typing stops and starts, the song stumbles and the chart shows the gaps.

## Run it

Open `index.html` in any modern browser (Chrome, Edge, Firefox or Safari).
There is no install, build step or account. It needs a physical keyboard and
works on Chromebooks.

## Lessons

18 lessons cover the three letter rows of the keyboard, plus a custom word list.

| Row | Lessons |
| --- | --- |
| Home row | F J, D K, S L, A ;, G H, home row words |
| Top row | E I, R U, T Y, W O, Q P, top row words |
| Bottom row | V M, B N, C and comma, X and period, Z and slash, all letters |
| Custom | My words: paste a spelling list or any words |

- The first home-row lessons use letter drills.
- Lessons that add new keys mix "reach and return" drills (`ded`, `kik`, `frf`)
  with real words. The words use only the keys learned so far.
- The next-key label names the finger and the direction of the reach, for
  example "left middle finger · reach up".

## Songs

All the songs are in the public domain. A song's length sets how many keys a
lesson has.

| Song | Notes |
| --- | --- |
| Ode to Joy (Beethoven) | 32 |
| Für Elise (Beethoven) | 35 |
| In the Hall of the Mountain King (Grieg) | 30 |
| Twinkle, Twinkle, Little Star (traditional) | 48 |

Every key is one beat. Long notes are struck again on each beat they last.

## How it scores flow

- The game times the gap between keys and compares each gap with the typist's
  own recent beat, which is the median of their last 8 gaps. Being on the beat
  scores 1.0, being 50% late scores about 0.57, and a gap twice as long scores
  about 0.38. Speed is not part of the score.
- The timing chart plots every keystroke by time and pitch. A key within 15% of
  the beat is "on beat". Otherwise it is "early" or "late", and missed keys are
  marked separately.
- A dashed marker shows when the next key is due, based on the typist's own
  pace.
- The music fills out as flow improves. A bass line joins at 50% flow and an
  octave layer at 75%.
- A wrong key makes a soft thunk, the letter is marked, and the song keeps
  going. Retyping the missed letter right away counts as a fix.
- A pause longer than about 5 seconds counts as a break and isn't penalized.

## Levels

| Level | Needs |
| --- | --- |
| Completed | Finish the lesson |
| Steady | Flow 60%+ and accuracy 85%+ |
| Mastered | Flow 75%+ and accuracy 93%+ |

The results screen shows flow, accuracy, words per minute, time and the
early / on-beat / late split. It also lists up to three keys that caused misses
or long hesitations. **Practice these keys** builds a short round from just
those keys.

## Custom word lists

Choose **My words** and paste any list. Capital letters become lowercase, and
numbers and other symbols are removed. When the page is hosted, a link like
`index.html?words=friend,happy,garden` opens with that list already loaded, so
a teacher can share one link with a class.

Progress, the chosen song and the word list are saved in the browser's local
storage, on that device only. No data leaves the computer.
