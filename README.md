<h1 align=center>Hugo PaperMod2.0</h1>

> Hugo PaperMod2.0 is a Hugo theme based on [Hugo PaperMod](https://github.com/adityatelange/hugo-PaperMod), itself based on [hugo-paper](https://github.com/nanxiaobei/hugo-paper).
> The goal of this project is to add native internet payment features, such as Bitcoin and Lightning capabilities, to the og theme.

This theme is very close Hugo PaperMod. Hence, most things stated in PaperMod's documentation should be applicable to PaperMod2.0, with minor refactor (for example, links might not be the same). I therefore choose to keep a copy of the [original PaperMod README file](https://github.com/fanismichalakis/hugo-PaperMod2.0/PARENT.README.md) on this repo as well.

## Additional features of PaperMod2.0 (with respect to PaperMod)

- Lightning Address in `meta` tag (detected by browser extensions such as [Alby](https://getalby.com/))
- Tippin.me and Zebedee svg icons (can be used as links to donation pages)

## Installation

1. Install Hugo

```bash
brew install hugo
```

You can check installation with:

```bash
hugo version
```

2. Create a new website

```bash
hugo new site <your-website>
```

3. Get the theme for GitHub

```bash
git clone https://github.com/fanismichalakis/hugo-PaperMod2.0 themes/PaperMod2.0 --depth=1
```

OR

```bash
git submodule add https://github.com/fanismichalakis/hugo-PaperMod2.0 themes/PaperMod2.0 --depth=1
```

4. Add the theme in config

Add the following line in `config.yml`:

```yml
theme: "PaperMod2.0"
```

## Usage

For a usage example, you can see my own website's [repo](https://github.com/fanismichalakis/fanismichalakis.fr).

## Acknowledgments

Huge shoutout to the Hugo devs, and to [@adityatelange](https://github.com/adityatelange) for PaperMod.