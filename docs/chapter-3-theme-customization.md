# Chapter 3: Theme Customization in Docusaurus

Docusaurus allows you to customize the look and feel of your documentation website using themes, CSS, and React components. This chapter will guide you through theme options and customization techniques to create a visually appealing book.

## Docusaurus Themes

By default, Docusaurus uses the **classic theme**, which provides a clean layout with a navbar, sidebar, footer, and responsive design. You can customize it or even create your own theme.

### Changing Colors and Fonts

You can modify colors and fonts by updating your `docusaurus.config.js` file under `themeConfig`:

```javascript
themeConfig: {
  colorMode: {
    defaultMode: 'light',
    disableSwitch: false,
  },
  navbar: {
    title: 'My AI Book',
    logo: { src: 'img/logo.svg', alt: 'Logo' },
  },
  prism: {
    theme: require('prism-react-renderer/themes/dracula'),
  },
}
