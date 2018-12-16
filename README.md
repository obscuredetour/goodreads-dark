---
title: The Colorado Sun dark theme
---
## Changelog

### **1.3**

- Fixed text & link colors within article emphasis areas with yellow background
- Altered article cards bottom borders to better reflect CO Sun theme
- Themed tag and category buttons

### **1.2**

- Improved contrast for 'opinion' tagged articles
- Changed 'Become A Member' button to dark text
- Enhanced navigation menu hover and focus contast
- Fixed byline author email links to yellow as blue is too hard to read with dark background
- Fixed credibility indicators' color to light on dark

### **1.1**

- Fixed text and link colors on yellow background

### **1.0 - initial release**

- Themed home page and articles
- Article data embed themed best as possible, might revisit

---
This is a blog post from [https://blog.jeffreysummers.me/post/co-sun-dark](https://blog.jeffreysummers.me/post/co-sun-dark).

The Colorado Sun is great and brilliantly designed, but after too much reading the white background can be glaring.

# Dark theme for coloradosun.com

I really like [The Colorado Sun](https://coloradosun.com/), but after a while the white background is too much. Their website design is fantastic, so I don't want to change too much.

The goal is to keep the same minimalistic theme with a touch of color, just darker and easier on the eyes. I am sharing it and the process of creation in hopes that it will help someone else.

So let's get after it! First is color selection and comparison. I use a tool throughout called [Contrast Ratio](https://contrast-ratio.com/) made by the brilliant [Lea Verou](http://lea.verou.me/). It always helps me balance contrast and text for maximum legibility on projects.

Skip to [screenshots](#screenshots).

## Website colors
**Background**

Colorado Sun's background is pure white `#fff`. Since their navigation bar and footer are already black I decided on charcoal `#202326`, for lack of a better name.

**Article headers**

Article headings are almost black `rgba(0,0,0,.85)`. Let's go with almost white `rgba(255,255,255,.85)`, because my goal is to change only a little and keep to their design and theme.

**Main text**

All main article text is pure black `#000` and I want mostly white `#f5f4f5` because the contrast will be plenty high enough with the new dark background color without going full blown pure white.

**Tertiary text**

The tertiary text includes all text on the secondary articles usually. Again with contrast and maximum legibility in mind and only changing what needs to be changed.

The two light greys `#8b8581`, `#7d7373` I swapped out for `#c9c9c9`,`#bcb8b6` respectively and the dark grey `#5a5653` to `#aeaeae`.

**Link text**

The links in the articles are bright blue `#2b56ff` with a bright green `#30e8bd` underline. After some fiddling around I decided to just reverse the colors to optimize contrast and keep the same vibe going.

Article bio and Credibility learn more links are blue too, but thought green looked out of place here. So I decided on CO Sun yellow `#fcd232` here.

**Buttons / Borders**

The buttons around the website are typically all CO Sun yellow `#fcd232` or the bright blue `#2b56ff`. Page and card borders are grey `#c4c2c0`. These I kept all the same except for one button.

Because the new awesome dark background is in place the all blue 'more stories' button on the home page is hard to see so I made it CO Sun yellow instead.

**Odds & Ends**

Some weird items include some data/graph tables and highlighted paragraphs. You can find these items in the following articles [Jared Polis campaign spending...](https://coloradosun.com/2018/09/14/jared-polis-campaign-spending-governor-race-2018/) & [Amid drought...](https://coloradosun.com/2018/09/12/colorado-water-law-drought-climate-change/) respectively.

I imagine these items will be more prevalent as more content is produced. I suspect some will even produce bugs. For example the table/graph is targeted by the following code.

```css
iframe[src*="//datawrapper"] {
	background-color: rgba(255, 255, 255, 0.7);
}
```

As more content is produced this might need to be expanded, fixed and/or tweaked.

### That's all folks

Below you'll find some screenshots as well as the GitHub repository where this theme is stored.

**How to use**

First, you will need the [CO Sun dark CSS file](https://github.com/obscuredetour/dark-co-sun/blob/master/co-sun-dark.css). You can copy/paste it into  the browser extension [Stylus](https://add0n.com/stylus.html) or click the **Raw** button to download. For reference here is the [Colorado Sun Dark theme on GitHub](https://github.com/obscuredetour/dark-co-sun).

You should be using the browser add-on [Stylus](https://add0n.com/stylus.html). Do **not** use Stylish as it has security issues. For reference, [Stylus on GitHub](https://github.com/openstyles/stylus).

[Stylus for Firefox](https://addons.mozilla.org/en-US/firefox/addon/styl-us/)

[Stylus for Chrome](https://chrome.google.com/webstore/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne?hl=en)

 Unfortunately, [Userstyles.org](https://userstyles.org/) will not let me log in no matter how many times I reset my password. What gives? If I decide to create a new account and upload it I will update this post.

### Screenshots

![Home Page view](https://github.com/obscuredetour/dark-co-sun/raw/master/screenshot-homepage.jpg)

![Article view](https://github.com/obscuredetour/dark-co-sun/raw/master/screenshot-article.jpg)
