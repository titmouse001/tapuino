## Tapuino - tweaked version (added support for compressed file loading)

The C64 Tape Emulator using an Arduino pro mini  (ATmega328 2KB version)

### Compression Tool Can be Found Here:
executable: https://github.com/titmouse001/C64TapCompressionTool/releases/tag/v1.0.0.1  
code: https://github.com/titmouse001/C64TapCompressionTool  

----
Changes to [Original Tapuino]:
- Added compression support
  - now loads compressed (packed) tap files
  - tap files can be compressed with the [Tap Compression Tool]
    - compressed files are called .zap files
    - compressed files must keep the .zap filename extension
  - tap files are still supported - you can mix both tap and zap files together
  - Example savings: Zybex.tap (881KB) -> Zybex.zap (89KB)
- Replaced 9x9 font with a smaller 5x7
  - includes a dedicated arrow for indicating off screen text
- Fixed minor scrolling filename bug
- Tweaked display logic

[Original Tapuino]:https://github.com/sweetlilmre/tapuino
[Tap Compression Tool]:https://github.com/titmouse001/Tapuino-C64TapPackerTool
