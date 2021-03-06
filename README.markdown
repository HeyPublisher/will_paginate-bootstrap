# will_paginate-bootstrap

---

__Minimal Updates__

The original author of this gem is no longer maintaining it.  This version of the gem is being maintained solely for the use within the HeyPublisher appliction.  If you have feature requests, it may take us a while to get to them.

---

![Bootstrap Pagination Component](https://raw.github.com/HeyPublisher/will_paginate-bootstrap/master/pagination.png)

This gem integrates the [Twitter Bootstrap](http://getbootstrap.com/) [pagination component](http://getbootstrap.com/components/#pagination) with the [will_paginate](https://github.com/mislav/will_paginate) pagination gem.

Just like will_paginate, Rails and Sinatra are supported.

## Install

  * `gem install will_paginate-bootstrap`, *or*
  * For projects using Bundler, add `gem 'will_paginate-bootstrap'` to your `Gemfile` (and then run `bundle install`).

## Usage

### Rails

  1. Load the Bootstrap CSS in your template.
  2. In your view, use the `renderer: BootstrapPagination::Rails` option with the `will_paginate` helper, for example:

```ruby
<%= will_paginate @collection, renderer: BootstrapPagination::Rails %>
```

### Sinatra

  1. Load the Bootstrap CSS in your template.
  2. `require "will_paginate-bootstrap"` in your Sinatra app.
  3. In your view, use the `renderer: BootstrapPagination::Sinatra` option with the `will_paginate` helper, for example:

```ruby
<%= will_paginate @collection, renderer: BootstrapPagination::Sinatra %>
```

## Compatibility

Starting at version 1.0, this gem no longer supports Bootstrap 2.

<table>
	<tr>
		<th>Ruby</th>
		<td>>= 1.9.2</td>
	</tr>
	<tr>
		<th>will_paginate</th>
		<td>>= 3.0.3</td>
	</tr>
	<tr>
		<th>Twitter Bootstrap</th>
		<td>>= 3.0.0</td>
	</tr>
</table>

Bootstrap 2 users can use version `0.2.5` of the gem which was the last version to offer Bootstrap 2 support.
