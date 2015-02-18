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
⋅⋅⋅ 1 column
⋅⋅⋅ 2 column
⋅⋅⋅ 3 column
⋅⋅⋅ 4 column

More will be added soon - but this is enough to get started with.

## Code breakdown

This is an example of a panel that contains a row followed by a two column layout

`<tr data-block-panel="basic">
  <td>
    <table align="center" border="0" cellpadding="0" cellspacing="0" class="container" style="width: 600px;">
      <tr data-block-row="two">
        <td class="container-padding" valign="top">
          <table border="0" cellpadding="0" cellspacing="0" style="width: 100%;">
            <tr>
              <td class="w100p" valign="top" width="560">
                <table border="0" cellpadding="0" cellspacing="0" class="w100p" align="left" width="270">
                  <tr>
                    <td>1/2</td>
                  </tr>
                </table>
                <table border="0" cellpadding="0" cellspacing="0" align="right" class="w100p" width="270">
                  <tr>
                    <td>2/2</td>
                  </tr>
                </table>
              </td>
            </tr>
          </table>
        </td>
      </tr>
    </table>
  </td>
</tr>`

Currently the data-block-* do nothing, so they can be removed, they might act as a reference point however.

`<table align="center" border="0" cellpadding="0" cellspacing="0" class="container" style="width: 600px;">`

The table which is the child of the panel element is given the class of container 
