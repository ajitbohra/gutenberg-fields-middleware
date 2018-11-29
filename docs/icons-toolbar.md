# icons-toolbar

![image](https://user-images.githubusercontent.com/1138833/39433283-113c0c44-4cb3-11e8-9d56-021306f76132.png)

Generally used in block-controls or inspector. 

## Properties

#### label:

A label for the field. Should not be used when field goes in block-controls.

- Type: `String`
- Required: No

#### help:

Used to add help text below the field. Should not be used when field goes in block-controls.

- Type: `String`
- Required: No

#### placement:

Defines where you want to show the field. By default a field would be added to the block however it can be added to the sidebar settings by using `inspector` or in the block-controls by using `block-controls`.

- Accepts: `block-controls`, `inspector`
- Type: `String`
- Required: No

#### **controls:**

Add icons to be added for selection. 

- Type: `Object`
- Required: Yes

**Example:**

```js
view: {
	type: 'string',
	field: {
		type: 'icons-toolbar',
		placement: 'block-controls',
		controls: [
			{
				icon: 'list-view', // Dashicon.
				title: 'List View',
				value: 'list',
			},
			{
				icon: 'grid-view',
				title: 'Grid View',
				value: 'grid',
			},
		],
	},
},
```



## Return value in `props.attribute`

- Type: `string`




Read more about defining attributes on official Gutenberg [handbook](https://wordpress.org/gutenberg/handbook/designers-developers/developers/block-api/block-attributes/).
