# Caroline Padon Site Guide

## Structure

Every project on the site is a self-contained folder. Each folder requires an `index.html` file. All media or other assets specific to that project can live in that folder for simple organization/linking. 

The TEMPLATE folder has a basic `index.html` for duplicating into new projects. 

## Homepage

The homepage colors can be customized using the `:root` CSS block.

The `accent` and `accent-transition` variable sets the gradient behind the pegboard. 

```css
:root {
--primary: #007618;
--hover: #e9f4ea;
--background: #fafffb;
--accent: #C2F90B;
--accent-transition: #afe1a8;
scroll-behavior: smooth;
}
```

### Works

The cells in each table must be wrapped in an `<a>` tag. 

```html
<tr>
	<td><a href="SITE_URL">WORK_TITLE</a></td>
	<td><a href="SITE_URL">YEAR</a></td>
</tr>
```

### Talks

The cells in each table must be wrapped in an `<a>` tag. 

```html
<tr>
	<td><a href="SITE_URL">TALK_TITLE</a></td>
	<td><a href="SITE_URL">LOCATION</a></td>
	<td><a href="SITE_URL">YEAR</a></td>
</tr>
```

## Project Template

Every project template includes an "Information Card" that serves as the header.

```html
<header>
<a href="/">
<table>
  <thead>
    <th colspan="3">Caroline Padon</th>
  </thead>
  <tbody>
    <tr class="info">
      <td>Project Name</td>
      <td>Role</td>
      <td>Year</td>
    </tr>
    <tr>
      <td>TEMPLATE_TITLE</td>
      <td>TEMPLATE_ROLE</td>
      <td>TEMPLATE_YEAR</td>
    </tr>
  </tbody>
</table>
</a>
</header>
```

Each card has several variables to fill:

- Page Title: `TEMPLATE_TITLE`
- Your role/skills used on the project: `TEMPLATE_ROLE`
- Year Completed/Started: `TEMPLATE_ROLE`


### Customizing the page

To edit the colors for the project, find the `:root` CSS block and edit the colors:

```css
:root {
--primary: black;
--hover: rgb(250 255 251);
--background: rgb(250 255 251);
--accent: rgb(0 118 24);
scroll-behavior: smooth;
}
```

To include custom HTML/styling, it is possible to remove all CSS except the `header` CSS block. This allows embedding bespoke project HTML/CSS. 

### SEO Variables

For SEO, there are several variables to fill for each page:

- Page Title: `TEMPLATE_TITLE`
- Page Description ~(150 character): `TEMPLATE_DESCRIPTION`
- Folder Name (will be the URL): `TEMPLATE_FOLDERNAME`

```html
<!-- Info -->
<meta name="description" content="TEMPLATE_DESCRIPTION">
<!-- Open Graph / Facebook -->
<meta property="og:type" content="website">
<meta property="og:url" content="https://caropadon.com/TEMPLATE_FOLDERNAME">
<meta property="og:title" content="Caroline Padon / TEMPLATE_TITLE">
<meta property="og:description" content="TEMPLATE_DESCRIPTION">
<!-- Twitter -->
<meta property="twitter:url" content="https://caropadon.com/TEMPLATE_FOLDERNAME">
<meta property="twitter:title" content="Caroline Padon / TEMPLATE_TITLE">
<meta property="twitter:description" content="TEMPLATE_DESCRIPTION">
<title>Caroline Padon / TEMPLATE_TITLE</title>
```

