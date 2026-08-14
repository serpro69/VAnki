# VAnki

VAnki is an AnkiConnect client at heart.

You open a video, it transcribes with Whisper if there aren't subtitles, and every word in the subtitle becomes clickable. Click one, dictionary popup. Hit enter and the card lands in Anki with the audio of that sentence cut out by ffmpeg, a screenshot of the frame, the sentence, and a translation.

If Anki is closed the cards queue up locally and send themselves the next time it sees Anki running, so forgetting to open it first doesn't cost you anything.

It reads intervals back the other way too. A word you've matured in Anki stops being highlighted in the video, so what's on screen tracks what you actually know instead of drifting into a separate list.

The distinctive part is deciding which words to suggest at all. Highlighting every sentence with exactly one unknown word sounds correct and is useless in practice. It also has to clear a frequency floor tied to your vocabulary size and not be a proper noun.

Other stuff: condensed audio (an MP3 of only the dialogue, about 20 minutes out of a 50 minute episode), seeding known words from a deck you already study without overwriting anything you set yourself, and it handles podcasts and radio.

VAnki is free, ELv2 licensed, and entirely local. No account, no API keys (possibly optional in future for better models and different providers, if that need arises). Catalan/Spanish, French, English, German, European Portuguese, Italian, and Norwegian support initially (with possible extension of the supported languages in the future).

## Acknowledgements

VAnki is inspired by [lingua-miner](./lingua-miner) but aims to bring many improvements and additional features on top of the original project.

## Contributing

Contributions are welcome! See the [Contributing guide](https://serpro69.github.io/vanki/latest/contributing/) for guidelines, [Architecture](https://serpro69.github.io/vanki/latest/contributing/architecture/) for how components fit together, and [Testing](https://serpro69.github.io/vanki/latest/contributing/testing/) for test conventions.

## License

Copyright &copy; 2026 - present, [serpro69](https://github.com/serpro69)

Distributed under the ELv2 License.

See [`LICENSE.md`](https://github.com/serpro69/vanki/blob/master/LICENSE.md) file for more information.
