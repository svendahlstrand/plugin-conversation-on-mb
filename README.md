# 🏕 Conversation on Micro.blog

Link to your post on the Micro.blog timeline from your blog.

![](https://github.com/svendahlstrand/plugin-conversation-on-mb/raw/main/docs/screenshot.png)

> With this convenient plug-in, your blog posts get a **Conversation on Micro.blog** link. When a reader taps that link, they will swiftly end up on the Micro.blog timeline for your blog post. From there, it's easy to engage in the conversation.

To get updates on this plug-in, [follow @sod on Micro.blog](https://micro.blog/sod).

## Do you get value from Conversation on Micro.blog? I'd love your support!

Hey! It's me, Sven. Conversation on Micro.blog and my other plug-ins are passion projects released to the world for free. That said, donations are always welcome if you get value from my work.

[💸 Donate $10](https://dahlstrand.net/donate/) or any amount you're comfortable with. Thanks! 🙏

## Bells and whistles

* 🛠 Customizable via plug-in settings.
* ✴️ Change the link text to whatever you want. Go bananas! Use emojis!
* ⛳️ Flexible placement in your theme using a Hugo partial.
* 🎁 Customize the look and feel using CSS.

## Get started

Hello, fellow microblogger! 👋 Thanks for being here. This plug-in is available in the official directory, so the installation process is quick and easy.

### Install the plug-in

1. Find [Conversation on Micro.blog](https://micro.blog/account/plugins/view/41) in the plug-in directory.
2. Choose the site you want to install the plug-in to.
3. Press *Install*.
4. Congratulations, the plug-in is now installed.

### Include the Conversation on Micro.blog link in your custom theme

For this step, you need a custom theme. Maybe you already have one? If not, [follow Manton's instructions here](https://help.micro.blog/t/custom-themes/59).

1. [Follow this link](https://micro.blog/account/themes) or go to *Design* → *Edit Custom Themes*.

2. Click on your custom theme. (It's probably named Marfa Custom or something like that.)

3. Click on the relevant template. (Often `layouts/post/single.html` but varies from theme to theme.)

4. Paste the following partial call where you see fit. For some themes, a good place might be after the content (look for `{{ .Content }}` in the template).
```
{{ partial "conversation-link.html" . }}
```

5. Press *Update Template* and pat yourself on the back.

### Make sure the Conversation on Micro.blog link shows up

1. Find a post on your blog and make sure you see the *Conversation on Micro.blog* link.

2. Click it, make sure it takes you to the timeline on Micro.blog.

### Configure the plug-in (if you want)

1. Go to *Plug-ins* and press ⚙️ *Settings* (next to the Conversation on Micro.blog plug-in).

2. Make changes as you see fit.

3. Press *Update Settings* and go to the next step.

### Customize the look and feel

The *Conversation on Micro.blog* link is delivered to you with minimal markup and styles. Every Micro.blog theme is individual, and this bare-bones approach keeps it flexible. It's up to you to implement a custom look and feel using HTML and CSS. Here's a couple of examples for your inspiration.

#### Give the link breathing room with a paragraph

There's an easy way to add a space between the *Conversation on Micro.blog* link and content around it. Just wrap the link in a paragraph. Add the partial call to the template in this way:

```html
<p>{{ partial "conversation-link.html" . }}</p>
```

That should result in the same amount of breathing space text paragraphs have between them.

#### Flexible look and hover effect using CSS

If you're comfortable with CSS, there are endless possibilities for styling. And if you're new to CSS, you can still do it! You can learn a lot from [@Miraz](http://micro.blog/miraz)'s excellent tutorials. Start with [What you need to know about CSS to customise your Micro.Blog blog](https://custom.micro.blog/2019/06/04/what-you-need.html).

The *Conversation on Micro.blog* link is just an `a` element with the class `conversation-on-mb`. I experimented with the CSS below to get a nice hover effect. It's not guaranteed to look good on your blog, though. 😉

<img src="https://github.com/svendahlstrand/plugin-conversation-on-mb/raw/main/docs/styling-example.png" alt="" width="304" height="108" />

To add custom CSS to a Micro.blog, navigate to *Design* → *Edit CSS*.

```css
.conversation-on-mb {
  border: solid 0.15rem black;
  border-radius: 0.4rem;
  color: black;
  display: inline-block;
  font-weight: bold;
  padding: 0.3rem 0.6rem 0 0.6rem;
  text-decoration: none;
}

.conversation-on-mb:hover {
  border-color: #011ac5;
  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.5);
  color: #011ac5;
  text-decoration: none;
}
```

### Having troubles?

Feel free to [reach out to @sod on Micro.blog](https://micro.blog/sod) for additional help.
