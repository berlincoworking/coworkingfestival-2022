## Requirements

### for Mac
* You need a version of the Ruby programming language on your computer to run this website locally. It’s installed on every Mac by default.
* You will need to install the xcode command line tools with `xcode-select --install`
* The site is generated with a static site generator. To install it, type `gem install bundler jekyll`.

### for Windows
* Read instructions here: https://jekyllrb.com/docs/windows/


## Development

To run the site locally and view it in your browser:
* Open Terminal.app (Mac).
* Clone this repository into your projects folder: `git clone <URL>`
* Go into the new directory: `cd coworkingfestival.github.io`
* Start the site generator with `jekyll serve --live`.

This will start a web server. Now you can view the site in your browser at http://127.0.0.1:4000.

See how to work with files at https://jekyllrb.com/docs/pages/.

### Adding a participating space

Each participating space has a `.md` file in the `/spaces` directory. To edit name, link, logo… of a space, edit the file.
To add a new space, create a new file `<spacename>.md`.
Keep in mind that filename, identifier, image filenames must always be lowercase and can not contain special characters, spaces or Umlaute.

Each space should also have a logo (`logo-<spacename>.svg`) and a photo (`photo-<spacename>.jpg`) in the corresponding folders.

Logo dimensions: 500x310px

Photo dimensions: 100x750px

### Editing Schedule (not there yet)

In order to edit the schedule, open the .csv file called e.g. `monday-events.csv` for the program day under `data` in a spreadsheet application and make the changes. Save the changes and commit them with `git commit -am 'schedule update' & git push`.
