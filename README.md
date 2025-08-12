# Anki_Bulk_Package_Importer
Bulk imports regular .apkg/.colpkg package files.

Does not modify the structure of your decks inside in any way. This may or may not be desireable for your use case. See similar projects below if you prefer deck structure to be based off of a folder structure.

For my use case, I designed decks/subdecks (based on `Deck(name=)`) with their own structures via [genanki](https://github.com/kerrickstaley/genanki/tree/main) and didn't want them altered by the importing program.

## Usage

1. Clone or download repository.

   `git clone https://github.com/shford/Anki_Bulk_Package_Importer.git`
2. Open `bulk_import_anki_packages.py`
	- Ensure `PROFILE` is set as desired.
		- Profiles can be seen by opening Anki and going to Anki->File->Switch Profile. Ensure `PROFILE` matches your profile. This is case sensitive.
	- Move your packages to the project folder `put_packages_here` or set `PACKAGE_PATH` to the path containing your packages.
3. Ensure the Anki app is closed.

4. Run `bulk_import_anki_packages.py`.

5. Reopen Anki. Enjoy!

## Similar projects
AnkiMultiImporter by [@KasperGam](https://github.com/KasperGam/AnkiMultiImporter)
- Appears to be abandoned 5 years ago. Based deck hierarchy on folder structure. I couldn't get it to work.

[@Shigeyuki](https://github.com/shigeyukey?page=1&tab=repositories) Appears to have revived the above project. I think it works. I could not find Shigeyuki's source code on Github.


## Limitations
PRs are welcome for all of these. Feel free to submit issues. I'll probably take a look but I make no promises on solutions, especially if an issue is platform specific.


This project does not currently support flatpak installations of Anki.

This program was tested with a modern version of Anki (v25.07.5) on Linux. I referenced the documentation but did actually test run to verify the correct anki2 collection file location for antiquated versions of Anki or other distros (Windows/Mac). If it's wrong it won't break anything, so give it a shot and drop an issue report.

## Disclaimer
This project is a pebble that relies on boulders like Anki that relies on mountains like Qt6 that relies on planets of OS's. At any point one of these things could change and this project may no longer work.

This software is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and noninfringement. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability, whether in an action of contract, tort, or otherwise, arising from, out of, or in connection with the software or the use or other dealings in the software.

## License
This project is provided under the GNU General Public License v2.0 license. In claims of tort or liability, the disclaimer above will take precedence over the license.