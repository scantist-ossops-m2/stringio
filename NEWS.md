# News

## 3.0.3 - 2022-12-08

### Improvements

  * Improved documents.
    [[GitHub#33](https://github.com/ruby/stringio/pull/33)]
    [[GitHub#34](https://github.com/ruby/stringio/pull/34)]
    [[GitHub#35](https://github.com/ruby/stringio/pull/35)]
    [[GitHub#36](https://github.com/ruby/stringio/pull/36)]
    [[GitHub#37](https://github.com/ruby/stringio/pull/37)]
    [Patch by Burdette Lamar]

### Fixes

  * Fixed a bug that large `StringIO#ungetc`/`StringIO#ungetbyte`
    break internal buffer.

  * Fixed a bug that `StringIO#each("2+ character", chomp: true)` cause
    infinite loop.
    [[Bug #18769](https://bugs.ruby-lang.org/issues/18769)]

  * Fixed a bug that `StringIO#each(nil, chomp: true)` chomps.
    [[Bug #18770](https://bugs.ruby-lang.org/issues/18770)]

  * Fixed a bug that `StringIO#each("", chomp: true)` isn't compatible
    with `IO#each("", chomp: true)`.
    [[Bug #18768](https://bugs.ruby-lang.org/issues/18768)]

  * Fixed a bug that `StringIO#set_encoding` doesn't accept external
    and internal encodings pairo.
    [[GitHub#16](https://github.com/ruby/stringio/issues/16)]
    [Reported by Kenta Murata]

  * Fixed a bug that `StringIO#truncate` isn't compatible with
    `File#truncate`.

### Thanks

  * Kenta Murata

  * Burdette Lamar
