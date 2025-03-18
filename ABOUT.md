# Lab 00 Template Readme

The published lab can be found at
[https://eecs281staff.github.io/l00-template](https://eecs281staff.github.io/l00-template).

![QR Code Link](images/lab00.qr.png)


## Changing the Lab Due Date

Edit the "lab-due" variable in the front matter of docs/README.md. This
string is quoted because the time contains a colon (:) which will break YAML
parsing.

## Adding Files or External Links

- **Adding New Page(s):** Include new files (either markdown or HTML) in the
  docs/ directory and link to them from docs/README.md.
- **Adding Downloadable Content:** Include new files (eg. PowerPoint or PDF)
  in the docs/ directory and add them to the "externalLinks" section in
  docs/_config.yml.  

```console
primerSpec:
  sitemap:
    label: ""
    externalLinks:
      - title: "Lab 00 Slides"
        url: l00-slides.pdf 
```
- **Adding External Links:** Edit "externalLinks" as above but include a
  fully qualified URL.
- **Adding Images or Figures:** Include any pictures (eg. JPG or PNG) in the
  docs/ directory and add them to the pages using markdown.  

```console
![Alt Text](images/image.png)
```

  For drawings, use Excalidraw to create the included files. These display
  like standard PNG images, but the source for the drawing is included in the
  file, so it may be edited later if necessary.

## Other Editing Concerns

### Document Structure

Labs have multiple sections that should be labeled with uppercase alpha
descriptors followed by a colon and a short title, beginning with "Part A:
Handwritten Problem (5)". Each of these sections should be
level two headings (##), and together give students a complete high-level
overview of the lab's requirements. Display the number of points each section
is worth in parentheses, after the title. If a section is not worth points
then follow the title with "(UNGRADED)", but each section must display its
contribution the lab grade.

To keep things clean visually, do not include any other level two headers,
and keep any additional level three headers out of the table of contents:  

```console
### Part B Subsection
{: .primer-spec-toc-ignore }
```

### Using Math Formulas

1. Ensure that `latex: true` is included in the front matter of any page with
   formulas.
2. Surround formulas with two dollar signs ($$) to interpret LaTeX
   expressions for typesetting. Kramdown does a good job deciding whether
   to include the formula inline (span) or block (div). To force an inline
   formula, precede it with a backslash (\\).  

```console
    # This will show up as a block element, works but ugly
    1. $$y = mx + b$$

    # This forced inline version looks nicer
    1. \$$y = mx + b$$

    # Here, additional text allows the default to work without forcing inline
    1. $$y = mx + b$$ is a linear equation
```

### Custom Styling or Extensions

To get the question options of the quizes to use capital letters (eg. A., B.)
additional styling was added via a change to the document head. This can be
found in `_includes/custom-head.html`, which loads a stylesheet
(`assets/css/quiz.css`). The questions need to be in an ordered list that is
not inside any other list, and the answers need to be an ordered list inside
of an ordered list.

Any additional custom styling or extensions can be included using this method.
