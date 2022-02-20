<h1 align=center>Hugo PaperMod2.0</h1>

> Hugo PaperMod2.0 is a Hugo theme based on [Hugo PaperMod](https://github.com/adityatelange/hugo-PaperMod), itself based on [hugo-paper](https://github.com/nanxiaobei/hugo-paper).
> The goal of this project is to add native internet payment features, such as Bitcoin and Lightning capabilities, to the og theme.

This theme is very close Hugo PaperMod. Hence, most things stated in PaperMod's documentation should be applicable to PaperMod2.0, with minor refactor (for example, links might not be the same). I therefore choose to keep a copy of the [original PaperMod README file](https://github.com/fanismichalakis/hugo-PaperMod2.0/PARENT.README.md) on this repo as well.

## Additional features of PaperMod2.0 (with respect to PaperMod)

- Lightning Address in `meta` tag (detected by browser extensions such as [Alby](https://getalby.com/))
- `paybutton` shortcode (seamlessly create donation buttons in your posts)
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

### Lightning Meta Tag

Add the following line in the `params` section of your `config.yml` file:

```yml
lightningAddress: "your@lightning.address"
```

Some browser extensions will catch it and allow their users to directly send tips to this address.

### paybutton shortcode

Instead of having to write some HTML every time you want to put a donation button in your page, you can use the `paybutton` shortcode to do the same thing in one line. This is a 2 steps process:

1. Add the destination url (BTCPay Server invoice page, Tippin page, etc.) to the page's params:

```md
---
title: "my blog post"
<...>
paybuttonlink: "your donation link"

---
```

2. Add the button where you want, as many times as you want:

```md
{{<paybutton text=" 🎩⚡ Give Value Back " color="#1da1f2">}}
```

As you can see, you can customize the text displayed in the button, as well the color of the button. Putting the link in the page's params allows you to use a different link for each post (can be useful to see which posts people found value in, for example).

## Acknowledgments

Huge shoutout to the Hugo devs, and to [@adityatelange](https://github.com/adityatelange) for PaperMod.

Thanks to [@dergigi](https://twitter.com/dergigi) for paving the way of [Value4Value](https://dergigi.com/2021/12/30/the-freedom-of-value/).