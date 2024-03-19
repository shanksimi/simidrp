
# SimiDRP

This javascript library help turn the date input DOM into a date range picker.


## Requirements

- `luxon: >=4.0`
- `tailwindcss: ^3.0`


## Installation

Just include in a script tag.

```html
  <script src="daterangepicker.js"></script>
```
    
## Deployment

Add class name to date input

```bash
<input type="date" class="drp-initial" name="..." />
```

Config:

```javascript
DRP.initialConfig({
    options: {
        'today': 'Today',
        'custom': 'Today'
    },
    locale: 'vi'
});
```

| Config    | Default Value | Description
|:---------|:------------|:------------
| `options.today` | Today | Display text for `today` option
| `options.1d` | Yesterday | Display text for yesterday option
| `options.7d` | Last 7 Days | Display text for last 7 days range
| `options.30d` | Last 30 Days | Display text for last 30 days range
| `options.thismonth` | This Month | Display text for this month range
| `options.1m` | Last Month | Display text for last month range
| `options.custom` | Custom Range | Display text for full calendar switch
| `locale` | en | Luxon DateTime locale 
| `icons.button` | svg | Button display SVG icon 
| `icons.prev` | svg | Previous month button SVG icon 
| `icons.next` | svg | Next month button SVG icon 
| `classes.default` | text-slate-900 | Default date style in calendar
| `classes.active` | text-red-600 !font-medium | Current date style in calendar
| `classes.highlight` | bg-indigo-500 text-white rounded-md | Chosen date style in calendar
| `classes.start` | bg-indigo-500 text-white rounded-l-md | Style for start of range date in calendar
| `classes.end` | bg-indigo-500 text-white rounded-r-md | Style for end of range date in calendar
| `classes.between` | bg-slate-50 text-slate-900 | Style for date in range

## Usage/Examples

Retrieve output range

```javascript
document.getElementById('inputname[start]').value

document.getElementById('inputname[end]').value
```

Or through submit data

```php
var_dump(inputname)

// [ 
//    'start' => 'YYYY-mm-dd', 
//    'end' => 'YYYY-mm-dd' 
// ]
```
## Screenshots

![App Screenshot](https://github.com/shanksimi/simidrp/screenshot.png)


## License

[MIT](https://choosealicense.com/licenses/mit/)

