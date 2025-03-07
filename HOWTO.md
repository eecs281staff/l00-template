# How to use this Repo Template

This uses Lab 06: Maps, Sets, and Enums as an example.

1. Make a copy with a proper repo title (eg. l06-maps-sets-enums)

2. Create a QR Code for easy link sharing
   ([see below](#create-a-qr-code-for-lab-url)) and save it in `images/` with
   a filename like `lab06.qr.png`.

3. Update the following settings
    - In `README.md`
        1. Change the title (H1, #) of the file
        2. Change the published lab link to match repo title from step 1 above
        3. Update the link to the filename for the QR Code from step 2 above
    - Rename `docs/l00-template/` like `docs/l06-maps-sets-enums`
    - In `docs/_config.yml`
        1. Change the title
        2. Change the repository root
        3. Change primerSpec:externalLinks:title
        4. Change primerSpec:externalLinks:url
    - In `docs/files.md`
        - Update "Download all files" link appropriately
    - In `docs/Makefile`
        1. Change PROJECTID to match the one used on the Autograder
        2. Change EXECUTABLE like lab06
        3. Change PROJECTNAME like l06-maps-sets-enums

4. Add content to the following locations

    - In `docs/README.md`
        - Convert content from original pdfs to markdown
        - Change `title` in front matter
        - Change `lab-due` date in front matter
    - Copy/create any needed images linked in `docs/README.md` to
      `docs/images/`
    - Copy slides pdf like `docs/l06-slides.pdf`
    - In `docs/solutions.md`
        - **DO NOT RENAME THE FILE**
        - Add solutions for any relevant sections
        - Change `title` in front matter
    - Add any files students download to `docs/l06-maps-sets-enums/`
    - Add any notes about downloaded files above "Tarball" in `docs/files.md`

5. Copy the original lab pdfs to `original-pdfs/`

## Create a QR Code for lab URL

Create QR Code at [www.qrcode-monkey.com](www.qrcode-monkey.com) with the
following settings:

- Enter Content
    - Your URL: https://eecs281staff.github.io/lab00-template
    - Statistics and Editability: Off
- Set Colors:
    - Foreground Color
        - Single Color
        - Custom Eye Color
        - #0000000
    - Eye Color
        - #00274C
        - #00274C
    - Background Color
        - #FFFFFF
- Add Logo Image
    - Upload Image: https://eecs281staff.github.io/eecs281.org/assets/images/eecs281logo.png
    - Remove Background Behind Logo: Yes

Make sure size is 1000x1000 (default) and "Download PNG".
