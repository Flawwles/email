Email Framework
=====

Simple to use fluid email template

## How does it work?

This template works by following a simple structure of `backgroundTable` `row` `column` and `block`.

## What's what?

### Background Table

Background Table is a 100% width table that wraps around all the content on the template - It's used to hold the rows and allow you to set background colours to the whole template

### Row

A row is also a 100% width table but it used to divide different areas of the email - This will normally be used to crate full width horizontal stripes that divide the email

### Column

By default all columns are set to be 600px wide; This creates the main content area of the email. On this framework there are a number of pre-set columns ready to go such as:
... 1 column
... 2 column
... 3 column
... 4 column

More will be added soon - but this is enough to get started with.

## Code breakdown

`<table align="center" border="0" cellpadding="0" cellspacing="0" class="container" style="width: 600px;">`

The table which is the child of the panel element is given the class of container and the width is set.

Within this table a row is inserted

`<tr data-block-row="one">`
`    <td valign="top" class="container-padding" style="background-color: #fffffe;">`
`       <table border="0" cellpadding="0" cellspacing="0" style="width: 100%;">`

The `TD` is given the call of container-padding which sets the gutter of the template (the space left and right) to stop the content touching the sides - The background colour that is set here will span 600px

Almost all `TABLE`s are given the attributes of `"border="0" cellpadding="0" cellspacing="0" style="width: 100%;"`



