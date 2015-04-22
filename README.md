autoform-markdown
========

A simple markdown textarea with preview using perak:markdown


Usage
-----

Add a custom template in your Schema

Example:

```
Schemas.Quest = new SimpleSchema({
  title: {
    type: String
  },
  text: {
    type: String,
    autoform: {
      type: 'markdown'
    }
  }
});
```

Render markdown text using the renderMarkdown helper in your template

```
<template name="quest">
  <h1>{{title}}</h1>
  {{{renderMarkdown text}}}
</template>
```

For more info and usage see: https://github.com/chjj/marked#usage