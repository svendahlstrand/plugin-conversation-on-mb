# ✴️ Conversation on Micro.blog

Link to your post on the Micro.blog timeline.

![](./docs/screenshot.png)

> With this convenient plug-in, your blog posts get a **Conversation on Micro.blog** link. When a reader taps that link, they will swiftly end up on the Micro.blog timeline for your blog post.

To get updates on this plug-in, [follow @sod on Micro.blog](https://micro.blog/sod).

## Bells and whistles

* 🛠 Customizable via plug-in settings.
* ✴️ Change the link text to whatever you want. Go bananas! Use emojis!
* ⛳️ Flexible placement in your theme using a Hugo partial.
* 🎁 Customize the look and feel using CSS.

## Get started

Hello, fellow microblogger! 👋 Thanks for being here. This plug-in is available in the official directory, so the installation process is quick and easy.

### Install the plug-in

1. Find Conversation on Micro.blog in the plug-in directory.
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

### Having troubles?

Feel free to [reach out to @sod on Micro.blog](https://micro.blog/sod) for additional help.
