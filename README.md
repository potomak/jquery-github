# GitHub jQuery plugin

A jQuery plugin to access GitHub API.

## Usage

Import the script

```html
<script src="jquery.github.js"></script>
```

Insert an empty `div` in the code

```html
<div class="members"></div>
```

Run the plugin

```javascript
$(function() {
  $(".members").github({organization: 'hackatron'});
});
```

## Options

### organization

Show a list of `organization`'s members.
See also http://developer.github.com/v3/orgs/members/

Type: `String`

Default: `null`

### onLoad

Called just before making a request to GitHub API.

Type: `Function`

Default: `null`

### onComplete

Called after a response from GitHub API.

Type: `Function`

Arguments: `response`

Default: `null`
