# tiptap-extension-video

<h3 align="center">
    A tiptap extension for inserting video.
</h3>

<br/>

<p align="center">
  <a href="https://www.npmjs.com/package/tiptap-extension-video">
    <img
     alt="NPM URL"
     src="https://img.shields.io/badge/npm-tiptapExtensionVideo?logo=npm">
  </a>
  <img
     alt="version"
     src="https://img.shields.io/badge/version-1.0.1-blue">
</p>

<br>

---

## Install

```shell
npm install tiptap-extension-video -S
```

## Usage

```js
editor
  .chain()
  .focus()
  .setVideo({
    src: videoUrl,
    HTMLAttributes: { "data-id": videoId },
  })
  .run();
```

## Options

You can configure common video HTML attributes via the HTMLAttributes options

```js
import Video from "tiptap-extension-video";

const editor = new Editor({
  element: document.querySelector(".editor"),
  extensions: [
    StarterKit,
    Video.configure({ HTMLAttributes: { class: "tiptap-video" } }),
  ],
});
```

## Relations

**tiptap-appmsg-iframe:** https://github.com/KID-1912/tiptap-extension-iframe

**tiptap-appmsg-editor:** https://github.com/KID-1912/tiptap-appmsg-editor
