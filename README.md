# pygments-tokens

A map of the tokens used by the pygments syntax highlighter

[Pygments](http://pygments.org/) is a syntax highlighter that
supports over 300 programming languages.  To use pygments in node,
check out [pygmentize-bundled](https://github.com/rvagg/node-pygmentize-bundled) or
[other options on npm](https://www.npmjs.com/search?q=pygments).

Given this JavaScript string:

```js
var a = "b";
```

pygments will generate this HTML:


```html
<div class="highlight"><pre>
  <span class="kd">var</span>
  <span class="nx">a</span>
  <span class="o">=</span>
  <span class="s2">&quot;b&quot;</span>
  <span class="p">;</span>
</pre></div>
```

See the `kd`, `nx`, `o` classes above? This package exports a map of [all the tokens used by pygments](http://pygments.org/docs/tokens/).

Use it to generate and/or validate pygments CSS stylesheets, or to create
a whitelist of allowable CSS class names.

Here's the whole exported object, for reference:

```js
{
  w: 'Whitespace',
  esc: 'Escape',
  err: 'Error',
  x: 'Other',

  k: 'Keyword',
  kc: 'Keyword.Constant',
  kd: 'Keyword.Declaration',
  kn: 'Keyword.Namespace',
  kp: 'Keyword.Pseudo',
  kr: 'Keyword.Reserved',
  kt: 'Keyword.Type',

  n: 'Name',
  na: 'Name.Attribute',
  nb: 'Name.Builtin',
  bp: 'Name.Builtin.Pseudo',
  nc: 'Name.Class',
  no: 'Name.Constant',
  nd: 'Name.Decorator',
  ni: 'Name.Entity',
  ne: 'Name.Exception',
  nf: 'Name.Function',
  py: 'Name.Property',
  nl: 'Name.Label',
  nn: 'Name.Namespace',
  nx: 'Name.Other',
  nt: 'Name.Tag',
  nv: 'Name.Variable',
  vc: 'Name.Variable.Class',
  vg: 'Name.Variable.Global',
  vi: 'Name.Variable.Instance',

  l: 'Literal',
  ld: 'Literal.Date',

  s: 'String',
  sb: 'String.Backtick',
  sc: 'String.Char',
  sd: 'String.Doc',
  s2: 'String.Double',
  se: 'String.Escape',
  sh: 'String.Heredoc',
  si: 'String.Interpol',
  sx: 'String.Other',
  sr: 'String.Regex',
  s1: 'String.Single',
  ss: 'String.Symbol',

  m: 'Number',
  mb: 'Number.Bin',
  mf: 'Number.Float',
  mh: 'Number.Hex',
  mi: 'Number.Integer',
  il: 'Number.Integer.Long',
  mo: 'Number.Oct',

  o: 'Operator',
  ow: 'Operator.Word',
  p: 'Punctuation',

  c: 'Comment',
  cm: 'Comment.Multiline',
  cp: 'Comment.Preproc',
  c1: 'Comment.Single',
  cs: 'Comment.Special',

  g: 'Generic',
  gd: 'Generic.Deleted',
  ge: 'Generic.Emph',
  gr: 'Generic.Error',
  gh: 'Generic.Heading',
  gi: 'Generic.Inserted',
  go: 'Generic.Output',
  gp: 'Generic.Prompt',
  gs: 'Generic.Strong',
  gu: 'Generic.Subheading',
  gt: 'Generic.Traceback'
}
```
