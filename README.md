# doc-server

doc-server provides gem rdoc, filtered to only the gems installed by your gemfile.

It's inspired by https://github.com/rubygems/rubygems-server and the now-defunct `godoc -http`.

##  Installation & usage

```
echo "gem 'doc-server'" >> Gemfile
bundle
bundle exec doc-server
```

This will create a directory (default='rdoc') to store the per-bundle documentation.

Whenever you install or update gems, delete this directory, and restart doc-server.

## Configuration

DOCSERVER_OUTPUT_PATH: Where to store the per-bundle documentation. Default is "rdoc".
DOCSERVER_PORT: Which port to listen on. Default is 8088.

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/danielheath/doc-server.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
