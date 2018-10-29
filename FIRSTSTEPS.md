# Hyde

Hyde is a brazen two-column [hugo](https://gohugo.io) theme based on the [Jekyll](http://jekyllrb.com) theme of the same name. It pairs a prominent sidebar with uncomplicated content.

![Hyde screenshot](https://f.cloud.github.com/assets/98681/1831228/42af6c6a-7384-11e3-98fb-e0b923ee0468.png)

## First Steps

You've now successfully installed your Hyde Theme in a Hugo project.

There's a few more settings we need to customize before you can get started.

### 1. Deployment

Currently your site is only visible to you but there's a few options to quickly make your site available to the world.

The easiest option in our opinion is Netlify. It's quick to setup and relatively easy to maintain.

1. Go to <a href="https://app.netlify.com/start" target="_blank">https://app.netlify.com/start</a>
2. Connect your Git provider and provide Netlify access to your repository (e.g. username/hyde)
3. Select and Click on your repository
4. Enter your build settings.
   * Build Command: `hugo`
   * Publish Directory: `public`
5. Add advanced build settings as a new variable.
   * Key: `HUGO_VERSION` Value: `0.42`
6. Click on `Deploy Site`

![](https://forestry.io/img/theme/netlify-step-4.gif)

7. Lastly copy your URL (e.g. https://something-something-123456.netlify.com/) and add it as your URL in your [`Site Configuration`](#/pages/config-toml).

The more powerful option is deployment to AWS and makes sense if you have experience with S3 and Cloudformation. You can find detailed documentation and a deployment template [here](https://forestry.io/docs/hosting/s3-cloudfront-stack/).

For other deployment options please check out our list [here](https://forestry.io/docs/hosting/) (including Webhooks, FTP/SFTP and Github Pages).

### 2. Advanced Settings

#### Themes

Hyde ships with eight optional themes based on the [base16 color scheme](https://github.com/chriskempson/base16). Apply a theme to change the color scheme (mostly applies to sidebar and links).

![Hyde in red](https://f.cloud.github.com/assets/98681/1831229/42b0b354-7384-11e3-8462-31b8df193fe5.png)

There are eight themes available at this time.

![Hyde theme classes](https://f.cloud.github.com/assets/98681/1817044/e5b0ec06-6f68-11e3-83d7-acd1942797a1.png)

To use a theme, go to `Site Configuration` -> `Additional Settings` -> `Theme` -> Add one of the theme names above.

![](https://forestry.io/img/theme/theme-settings-hyde.png)

To create your own theme, look to the Themes section of [included CSS file](https://github.com/poole/hyde/blob/master/public/css/hyde.css). Copy any existing theme (they're only a few lines of CSS), rename it, and change the provided colors.

#### Reverse layout

![Hyde with reverse layout](https://f.cloud.github.com/assets/98681/1831230/42b0d3ac-7384-11e3-8d54-2065afd03f9e.png)

To reverse page orientation activate `Reverse Layout` in `Site Configuration` -> `Additional Settings`.

#### Commentary with Disqus

You can optionally enable a comment system powered by Disqus for your posts. Simply add your Disqus Shortname in `Site Configuration` -> `Additional Settings` -> `Disqus Shortname`.

If you don't have a Disqus Account you can sign up for an account [here](https://disqus.com/).

#### Google Analytics

Google Analytics can be enabled by assigning your tracking code to `Site Configuration` -> `Additional Settings` -> `Google Analytics Tracking Code`.

If you don't have a Google Analytics Account you can sign up for an account [here](https://marketingplatform.google.com/about/analytics/).

### 3. Editing in Forestry

Your site is completely editable in Forestry. The Hyde theme is a simple responsive blog completely based on posts and a sidebar menu.

#### Creating and Editing A New Page/Post

Pages and Posts are separated into two different categories.

To create a new page or post click on *Create New* and select *Post* (or *Page* depending what section you are in). Enter a title and click *Create* to proceed to the editor. 

![](https://forestry.io/img/theme/create-new.png)

On the left side you'll find general settings (e.g. title, subtitle, date etc.) and on the other side you have access to the Forestry Editor. The toolbar at the bottom of the editor will help you format and more easily navigate the editor.

![](https://forestry.io/img/theme/toolbar.png)

#### Add and Edit the Sidebar

To add new links and edit existing ones navigate to [Menus](#/menus/main) and click on `add link` or click on the settings wheel to edit existing links.

You are also able to reorder or remove existing links.

#### Preview

You can preview any post or page to see what it looks like before you publish your changes. Simply click on <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" viewBox="0 0 24 24"><g fill="none" fill-rule="evenodd" stroke="currentcolor" stroke-width="1.2"><path d="M12 18c6 0 10-6 10-6s-4-6-10-6-10 6-10 6 4 6 10 6z"></path><circle cx="12" cy="12" r="2"></circle></g></svg> in the top-right corner of your editor.

#### Publish

All new posts/pages start out as draft. To publish a post/page you'll have to turn **Draft** to **OFF** and click on **Save**. If you've set up the site as outlined in the **Deployment** section, Forestry will no build your site and your hosting provider (Netlify, AWS, etc.) is going to update your website shortly.

![](https://forestry.io/img/theme/publish.png)

*More Information on Editing with Forestry [here](https://forestry.io/docs/editing/markdown-editor/)*  
*The full documentation for Developers using Forestry can be found [here](https://forestry.io/docs/)*

***

### Author

**Mark Otto**

* [https://github.com/mdo](https://github.com/mdo "https://github.com/mdo")
* [https://twitter.com/mdo](https://twitter.com/mdo "https://twitter.com/mdo")

### Ported By

**Steve Francia**

* [https://github.com/spf13](https://github.com/spf13 "https://github.com/spf13")
* [https://twitter.com/spf13](https://twitter.com/spf13 "https://twitter.com/spf13")

### License

Open sourced under the [MIT license](LICENSE.md).

<3
