# Active learning: Adding table structure

Let's put these new elements into action.

1. First of all, make a local copy of spending-record.html and minimal-table.css in a new folder.
2. Try opening it in a browser — You'll see that it looks OK, but it could stand to be improved. The "SUM" row that contains a summation of the spent amounts seems to be in the wrong place, and there are some details missing from the code.
3. Put the obvious headers row inside a `<thead>` element, the "SUM" row inside a `<tfoot>` element, and the rest of the content inside a `<tbody>` element.
4. Save and refresh, and you'll see that adding the `<tfoot>` element has caused the "SUM" row to go down to the bottom of the table.
5. Next, add a colspan attribute to make the "SUM" cell span across the first four columns, so the actual number appears at the bottom of the "Cost" column.
6. Let's add some simple extra styling to the table, to give you an idea of how useful these elements are for applying CSS. Inside the head of your HTML document, you'll see an empty `<style>` element. Inside this element, add the following lines of CSS code:

```css
CSS
Copy to Clipboard
tbody {
  font-size: 95%;
  font-style: italic;
}

tfoot {
  font-weight: bold;
}
```

7. Save and refresh, and have a look at the result. If the `<tbody>` and `<tfoot>` elements weren't in place, you'd have to write much more complicated selectors/rules to apply the same styling.