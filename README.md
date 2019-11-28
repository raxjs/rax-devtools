# Rax Developer Tools

Rax Developer Tools lets you inspect the Rax component's structure, props and state.

Go to [Chrome extension](https://chrome.google.com/webstore/detail/rax-developer-tools/anpeoinhjjligmgoiepbnigjhmijblff) store to install this extension.

### Pre-packaged

The official extensions represent the current stable release.

- [Chrome extension](https://chrome.google.com/webstore/detail/rax-developer-tools/anpeoinhjjligmgoiepbnigjhmijblff)

## Usage

1. Install the Chrome [Rax Developer Tools](https://chrome.google.com/webstore/detail/rax-developer-tools/anpeoinhjjligmgoiepbnigjhmijblff) extension
2. Import the "rax/lib/devtools" module in your app
  ```js
  import 'rax/lib/devtools';
  ```
3. Set `process.env.NODE_ENV` to 'development'
4. Reload and go to the 'Rax' tab in the browser's development tools


### Tree View

- Arrow keys or hjkl for navigation
- Right click a component to show in elements pane, scroll into view, show
  source, etc.
- Differently-colored collapser means the component has state/context

![](/images/devtools-tree-view.png)

### Side Pane

- Right-click to store as global variable
- Updates are highlighted

![](/images/devtools-side-pane.gif)

### Search Bar

- Use the search bar to find components by name

![](/images/devtools-search-new.gif)

### Handy Tips

#### Finding Component by a DOM Node

If you inspect a Rax element on the page using the regular **Elements** tab, then switch over to the **Rax** tab, that element will be automatically selected in the Rax tree.

#### Finding DOM Node by a Component

You can right-click any Rax element in the **Rax** tab, and choose "Find the DOM node". This will bring you to the corresponding DOM node in the **Elements** tab.
