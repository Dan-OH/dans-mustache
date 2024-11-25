# Dan's Mustache

A custom language profile for Mustache files. **Note:** This extension is not compatible with standard Mustache or Handlebars syntax. It's a unique modification for it and probably won't work for you.

---

## Key Features

### Custom Syntax
- Uses HTML-style comments (`<!-- -->`) instead of Mustache's native commenting syntax.

### Code Snippets
Snippets for common tags and templates. Type a prefix to quickly insert a snippet. Here's the full list of available snippets:

|**Prefix**|**Snippet**|**Description**|
|----------|-----------|---------------|
|`webname`,`web name`|`{{web.name}}`|Web Name Comet Tag|
|`webroot`,`web root`|`{{web.root}}`|Web Root Comet Tag|
|`pagemeta`,`page meta`|`{{page.meta}}`|Page Meta Comet Tag|
|`pageslug`,`page slug`|`{{page.slug}}`|Page Slug Comet Tag|
|`parentslug`,`parent slug`|`{{page.parentSlug}}`|Page Parent Slug Comet Tag|
|`pagepath`,`page path`|`{{page.path}}`|Page Path Comet Tag|
|`pagetitle`,`page title`|`{{page.title}}`|Page Title Comet Tag|
|`parenttitle`,`parent title`|`{{page.parentTitle}}`|Page Parent Title Comet Tag|
|`pagebreadcrumb`,`breadcrumbs`|`{{{page.breadcrumb}}}`|Page Breadcrumb Comet Tag|
|`year`|`{{year}}`|Year Comet Tag|
|`pageincludeshead`|`{{{common.template(page-includes-head)}}}`|Page Includes Head Comet Tag|
|`pageheader`|`{{{common.template(page-header)}}}`|Page Header Comet Tag|
|`pagefooter`|`{{{common.template(page-footer)}}}`|Page Footer Comet Tag|
|`pageincludesbody`|`{{{common.template(page-includes-body)}}}`|Page Includes Body Comet Tag|
|`pagecontent`,`inline content`|`<div id="content-$1">{{{page.content($1)}}}</div>`|Inline Content Area|
|`pagebannerimage`,`bannerimage`|`<img id="content-$1" src="{{{page.content($1)}}}" width="$2" height="$3">`|Inline Banner Image|
|`socialmedialink`,`social media links`|`{{{socialMedia.links}}}`|Social Media Links [OLD]|
|`socialmediadynamiclinks`|`{{{socialMedia.dynamicLinks}}}`|Social Media Dynamic Links|
|`postopengraph`,`post open graph`|`{{{post.openGraph}}}`|Post Open Graph Comet Tag|
|`postheadtitle`,`post head title`|`{{{post.headTitle}}}`|Post Head Title Comet Tag|
|`posttitle`,`post title`|`{{{post.title}}}`|Post Title Comet Tag|
|`postcontent`,`post content`|`{{{post.post}}}`|Post Content Comet Tag|
|`postlisting`,`post listing`|`{{{post.listing}}}`|Posts Listing Comet Tag|
|`posttags`,`post tags`|`{{{post.tags}}}`|Post Tags Comet Tag|
|`posttagname`,`post tag name`|`{{{post.tagName}}}`|Post Tag Name Comet Tag|
|`eventtitle`,`event title`|`{{{event.title}}}`|Event Title Comet Tag|
|`eventitem`,`event item`|`{{{event.item}}}`|Event Item Comet Tag|
|`eventlisting`,`event listing`|`{{{event.listing}}}`|Event Listing Comet Tag|
|`eventhomepagesidebarlisting`|`{{{event.homepageSidebarListing}}}`|Event Homepage Sidebar Listing Comet Tag|
|`featurebanner`,`feature banner`|```<div class="feature-banner" style="background-image: url('{{& page.bannerImage }}');"><div class="feature-banner-inner"><h1 class="page-title">{{page.title}}</h1></div></div>```|Page Extra Image Feature Banner|

---

## Usage Tips
- **Snippets:** Type any snippet prefix to see an autocomplete suggestion. Hit `Tab` to insert.
- **Commenting:** Use `<!-- -->` for comments in `.mustache` files.
