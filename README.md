<div align="right">Language: :us:
<a title="Chinese" href="docs/zh-CN/README.md">:cn:</a>
<a title="Russian" href="docs/ru/README.md">:ru:</a></div>

# <div align="center"><a title="NexT website repository" href="https://github.com/theme-next/theme-next.org"><img align="center" width="56" height="56" src="https://raw.githubusercontent.com/theme-next/hexo-theme-next/master/source/images/logo.svg?sanitize=true"></a> e x T</div>

<p align="center">«NexT» is a high quality elegant <a href="http://hexo.io">Hexo</a> theme. It is crafted from scratch with love.</p>
<p align="center">
  <a href="https://bestpractices.coreinfrastructure.org/projects/2625"><img src="https://bestpractices.coreinfrastructure.org/projects/2625/badge" title="Core Infrastructure Initiative Best Practices"></a>
  <a href="https://www.codacy.com/app/theme-next/hexo-theme-next?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=theme-next/hexo-theme-next&amp;utm_campaign=Badge_Grade"><img src="https://api.codacy.com/project/badge/Grade/72f7fe7609c2438a92069f448e5a341a" title="Project Grade"></a>
  <a href="https://travis-ci.org/theme-next/hexo-theme-next?branch=master"><img src="https://travis-ci.org/theme-next/hexo-theme-next.svg?branch=master" title="Travis CI [Linux]"></a>
  <a href="https://i18n.theme-next.org"><img src="https://d322cqt584bo4o.cloudfront.net/theme-next/localized.svg" title="Add or improve translation in few seconds!"></a>
  <a href="https://github.com/theme-next/hexo-theme-next/releases"><img src="https://badge.fury.io/gh/theme-next%2Fhexo-theme-next.svg"></a>
  <a href="http://hexo.io"><img src="https://img.shields.io/badge/hexo-%3E%3D%203.5.0-blue.svg"></a>
  <a href="https://github.com/theme-next/hexo-theme-next/blob/master/LICENSE.md"><img src="https://img.shields.io/badge/license-%20AGPL-blue.svg"></a>
</p>

## Live Preview

* :heart_decoration: Muse scheme: [LEAFERx](https://leaferx.online) | [Alex LEE](http://saili.science) | [Miaia](https://11.tt)
* :six_pointed_star: Mist scheme: [uchuhimo](http://uchuhimo.me) | [xirong](http://www.ixirong.com)
* :pisces: Pisces scheme: [Vi](http://notes.iissnan.com) | [Acris](https://acris.me) | [Jiaxi He](http://jiaxi.io)
* :gemini: Gemini scheme: [Ivan.Nginx](https://almostover.ru) | [Raincal](https://raincal.com) | [Dandy](https://dandyxu.me)

More «NexT» examples [here](https://github.com/iissnan/hexo-theme-next/issues/119).

## Installation

Simplest way to install is by cloning the entire repository:

   ```sh
   $ cd hexo
   $ git clone git@github.com:hoganbin/hexo-theme-next themes/next
   ```

Or you can see [detailed installation instructions][docs-installation-url] if you want any other variant.

## Plugins

In NexT config now you can find dependencies on each module which was moved to external repositories which can be found by [main organization link](https://github.com/theme-next).

For example, if you want to use `fancybox` in your site, go to NexT config and see:

```yml
# Fancybox
# Dependencies: https://github.com/theme-next/theme-next-fancybox
fancybox: false
```

Then turn on `fancybox` and go to «Dependencies» link with installation instructions of this module.

### Exceptions

If you use cdn for any plugins, you need to replace your cdn link.

For example, if you want to use `fancybox` and you configured a cdn link, go to NexT config and see:

```yml
vendors:
  # ...
  # Some contents...
  # ...
  fancybox: # Set or update fancybox cdn url.
  fancybox_css: # Set or update fancybox cdn url.
```

Instead of defining [main organization link](https://github.com/theme-next) for updates.

## Update

You can update to latest master branch by the following command:

```sh
$ cd themes/next
$ git pull
```

And if you see any error message during update (something like **«Commit your changes or stash them before you can merge»**), recommended to learn [Hexo data files][docs-data-files-url] feature.\
However, you can bypass update errors by using the `Commit`, `Stash` or `Reset` commands for local changes. See [here](https://stackoverflow.com/a/15745424/5861495) how to do it.

**If you want to update from v5.1.x to v6.0.x, read [here][docs-update-5-1-x-url].**

## Known Bugs

For those who also encounter **«[Error: Cannot find module 'hexo-util'](https://github.com/iissnan/hexo-theme-next/issues/1490)»**, please check your NPM version.

* `> 3`: Still not work? Please remove `node_modules` directory and reinstall using `npm install`.
* `< 3`: Please add `hexo-util` explicitly via `npm install --save-dev hexo-util` to you site package deps.