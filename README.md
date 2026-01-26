# Haskell MOOC 简体中文翻译版

本仓库内容由[千代有希](https://github.com/ChiyoYuki)个人翻译。
个人英语水准属实不高，如有翻译不当之处甚是抱歉。
欢迎提 issue 或是 PR 完善翻译，对您的支持与帮助深表感谢。

## 跳转链接

[课程第一部分](http://haskell-mooc.chiyo.uk/part1-zh_cn.html)

[课程第二部分](http://haskell-mooc.chiyo.uk/part2-zh_cn.html)

> 另注：中文翻译版存于本仓库 `cn` 分支，本仓库 `master` 分支为个人练习用，敬请留意。

## 名词对照表

|原文|译文|
|---|---|
|functional|泛函、函数式|
|lazy|惰性的|
|algebraic datatype|代数数据类型|
|list|列表|
|parameterized|参数化的|
|type class|类型类|
|constructor|构造子|
|list comprehension|列表推导式|

以下为原仓库 README.md

---

# Haskell MOOC

<p align="center"><img alt="Course logo" src="img/haskell-mooc-logo.svg" width="400" align="center"></p>

University of Helsinki

[Course page](https://haskell.mooc.fi)

[![License: CC BY-SA 4.0](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-sa/4.0/)

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/).

## About the course

This is an online course on Functional Programming that uses the
Haskell programming language. You can study at your own pace. All the
material and exercises are openly available.

The course is intended to be followed through the [Course
page](https://haskell.mooc.fi), but in case the course page is down or
you want an offline backup, the course material is also available in
this repository ([part1.html](part1.html), [part2.html](part2.html)).

## Exercises

Exercises can be found under `exercises/` directory. All required dependencies
can be downloaded and built with:

```
stack build
```

Exercises are Haskell source code files named `Set1.hs`, `Set2.hs` and so on.
You complete the exercises by editing the file according to the instructions in
the file. You can check your answers by running

```
stack runhaskell SetXTest.hs
```

in the `exercises/` directory. Remember to replace `X` with the number
of the set you are working on.

See [the material](part1.html#working-on-the-exercises) for more info.

## Troubleshooting

Here are some fixes for common problems with `stack build`:

- If you get an error like `While building package zlib-0.6.2.3`, you need to install the zlib library headers. The right command for Ubuntu is `sudo apt install zlib1g-dev`.
- If you get an error like `Downloading lts-18.18 build plan ... RedownloadInvalidResponse`, your version of stack is too old. Run `stack upgrade` to get a newer one.

### Newer GHC version

If you need to use a newer version of GHC, perhaps to get
vscode-haskell to work, try the `ghc-9.6.6` branch of this repository
for GHC 9.6.6. The default for the course is GHC 9.2.8 for now.

Don't forget to run `stack build` again after changing branches.

## Reporting errors

If you notice an error in these materials, you can report it via

- an issue or pull request in this repository (see [CONTRIBUTING.md](CONTRIBUTING.md))
- the course [channel on Telegram](https://t.me/haskell_mooc_fi)
