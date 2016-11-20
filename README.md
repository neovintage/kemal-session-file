# kemal-session-file

File System based session storage for [Kemal](http://github.com/sdogruyo/kemal)

## Installation


Add this to your application's `shard.yml`:

```yaml
dependencies:
  kemal-session-file:
    github: sdogruyol/kemal-session-file
```


## Usage

Be sure that the session path folder is writable by the user.

```crystal
require "kemal"
require "kemal-session-file"

Session.config.engine = Session::FileSystemEngine.new({:sessions_dir => "./your/session/path/"})

Kemal.run
```



## Contributing

1. Fork it ( https://github.com/sdogruyol/kemal-session-file/fork )
2. Create your feature branch (git checkout -b my-new-feature)
3. Commit your changes (git commit -am 'Add some feature')
4. Push to the branch (git push origin my-new-feature)
5. Create a new Pull Request

## Contributors

- [sdogruyol](https://github.com/sdogruyol) Serdar Dogruyol - creator, maintainer
