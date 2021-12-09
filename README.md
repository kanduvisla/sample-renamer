# sample-renamer

A Small CLI tool to quickly rename WAV-samples on MacOS

## Installation

Clone this repository and add the following alias (replacing the path with the actual path ofcourse):

    alias sr="[PATH TO REPOSITORY]/sr"

## Usage

Just enter a folder with a lot of WAV-files and type `sr`.
The script will play each sample and ask for input. The input can be:

- _(blank)_ : The file will not be renamed
- `r` : Replay the sample
- _(anything)_ : The file will be renamed to `(anything).wav`.

## Notes

- This script only works on MacOS, because it was quickly made on the fly and uses
MacOS's built-in `afplay` command. However, it would be possible to simply replace 
this line in the script with another player to make the script applicable for more
Unix-based platforms (please make sure to send a Pull Request if you do).
- There is no way to stop playing the sample. So if you have a folder with all kind
of samples that are 10s of seconds to minutes, this might not be the best tool for you.
I used it to rename all kind of short samples (kicks, snares, hihats, etc.)
