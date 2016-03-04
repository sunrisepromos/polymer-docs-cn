
# Polymer documentation style guide

This extremely brief style guide records some style decisions
we've made in the course of developing these docs.

There are counterexamples for each of these rules in the existing docs.

## Language

Most tech writing style guides discuss these points in more detail.

Use the active voice.

-   Good. Polymer upgrades the element when you add it to the document.
-   Avoid. The element is upgraded when you add it to the document.

Use the present tense whenever possible.

-   Good. Clicking the element starts an animation.
-   Avoid. Clicking the element will start an animation.

Address the user in the second person ("you" not "we").

-   Good. You can use any web server to serve your elements.
-   Avoid. We can use any web server to serve our elements.

-   Good. First, edit the `index.html` file.
-   Avoid. Let's reload the page to see the changes.

In direct instructions and procedures, omit the "you":

-   Good. Click **Save**.
-   Avoid. Next you click **Save**.

## Link text

Use descriptive link text. When cross-referencing sections in the doc, include
the section title, in sentence case.

    See [Observe added and removed children](link).

Avoid unqualified inline links such as:

    In this case, you need to [notify the data binding system](link).

Use unqualified inline links only for links where the linked resource is the
_definitive_ definition of the term (for example, API reference page for a
method).

    To update custom properties dynamically, call
    [updateStyles](/{% polymer_version_dir %}/api/#Polymer.Base:method-updateStyles){:target="api"}).

When linking off-site, it should be clear that the link goes off site. For some
documents (like web standards) this may be clear enough from the title.

-   Good: See the
    [Gold standard checklist for web components](https://github.com/webcomponents/gold-standard/wiki)
    on GitHub.
-   Good. Defined in the
    [Shadow DOM specification](https://www.w3.org/TR/shadow-dom/).
-   Avoid. Use `Polymer.dom(event)` to simulate
    [event retargeting](https://www.w3.org/TR/shadow-dom/#event-retargeting).
-   Avoid. Polymer elements use the
    [mediator pattern](https://en.wikipedia.org/wiki/Mediator_pattern).

### API doc links

When linking to API docs, use `target="api"` so the links always open in the
same tab.

    [`listen`](/{% polymer_version_dir %}/api/#Polymer.Base:method-listen){:target="api"})

### Catalog links

When linking to the element catalog, use `target="catalog"` so links always open
in the same tab.

    See the
    [`iron-flex-layout` guide](https://elements.polymer-project.org/guides/flex-layout){:target="catalog"}
    for details.

## Formatting

Use backticks or `<code>` for inline code.

### Formatting API names

Set API names in code font—this includes JavaScript classes, attributes,
properties, methods, and event names.

For methods, omit the parenthesis unless you're specifying arguments.

-   Good: Call `render` to force a synchronous refresh.
-   Avoid: Call `render()` to force a synchronous refresh.

### Formatting element names

For non-type-extension elements, use code font and angle brackets:

-   Good: The `<iron-icon>` element ...
-   Avoid: The `iron-icon` element ...

For type-extension elements, don't add brackets around the element name.
Instead, use the bare element name:

-   Good: A `custom-style` element ...
-   Avoid: A `<custom-style>` element ...

To be extra clear, show both the base tag name and the `is=""` attribute
enclosed in brackets:

-   Good: A `<style is="custom-style">` element ...


### Formatting lists

Line up list text at a 4 space indent.

    *   This is the first line of
        a multi-line list item.

        This is a second paragraph for a
        list item.

    *   This is the next list item.

            <!-- a code sample is indented 4 more spaces -->

## Titles and headings

Document titles and section headings should be in sentence case.

-   Good: ## Create a new element
-   Avoid: ## Create a New Element

For task sections, use 2nd person imperative verbs, not gerunds.

-   Good: ## Observe DOM changes
-   Avoid: ## Observing DOM changes

For concepts sections, favor noun titles instead of verb titles.

-    Good: ## Data binding
-    Avoid: ## Understanding data binding

## Text wrapping

Please set your text editors to wrap text at 80 characters and trim trailing
whitespace. This makes it easier to review pull requests on GitHub.
