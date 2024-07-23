**Read this in other languages: [English](README.md), [中文](README_ZH.md).**

# 学术页面

![pages-build-deployment](https://github.com/academicpages/academicpages.github.io/actions/workflows/pages/pages-build-deployment/badge.svg)

Academic Pages是学术网站的Github页面模板。

# 如何开始

1.如果您没有GitHub帐户，请注册一个，并确认您的电子邮件（必填！）
1.点击右上角的“使用此模板”按钮。
1.在“New repository”页面上，输入您的仓库名称“[your GitHub username]. github.io“，这也将是您网站的URL。
1.设置站点范围的配置并添加您的内容。
1.上传任何文件（如PDF、.zip文件等）到`files/`目录。它们将出现在https：//[您的GitHub用户名]. github.io/files/example.pdf。
1.通过转到“GitHub页面”部分中的存储库设置来检查状态
1.（可选）使用`markdown_generator`文件夹中的python notebook或python脚本从TSV文件生成用于出版物和演讲的markdown文件。

更多信息请访问 https://academicpages.github.io/

## 本地运行

当你最初在网站上工作时，在将更改推送到GitHub之前能够在本地预览更改是非常有用的。要在当地工作，您需要：
1.克隆存储库，并按照上面的详细说明进行更新。
1.确保您安装了ruby-dev、python和nodejs
    
    On most Linux distribution and [Windows Subsystem Linux](https://learn.microsoft.com/en-us/windows/wsl/about) the command is:
    ```bash
    sudo apt install ruby-dev ruby-bundler nodejs
    ```
    On MacOS the commands are:
    ```bash
    brew install ruby
    brew install node
    gem install bundler
    ```
1.运行`bundle install`安装ruby依赖。如果你得到错误，删除Gemfile.lock并重试。
1.运行`jekyll serve -l -H localhost`生成HTML并从`localhost：4000`提供，本地服务器将自动重建并刷新更改的页面。
如果您在Linux上运行，则可能需要安装一些额外的依赖项，然后才能在本地运行：“sudo apt install build-essential gcc make”

# 维护

Bug报告和对模板的功能请求应该[通过GitHub提交]（https：//github.com/academicpages/academicpages.github.io/issues/new/choose）。有关如何设置模板样式的问题，请随时开始[在GitHub上的新讨论]（https：//github.com/academicpages/academicpages.github.io/discussions）。

此存储库由[Stuart盖革]（https：//github.com/staeiou）从[Minimal Mistakes Jekyll Theme]（https：//mmistakes.github.io/minimal-mistakes/）中分叉（然后分离），该主题由© 2016 Michael Rose在MIT许可证下发布（参见LICENSE.md）。它目前由[Robert Zupko]（https：//github.com/rjzupkoii）维护，欢迎更多的维护者。

## 错误修复和增强

如果你有bug修复和增强，你想提交一个pull request，你需要[fork]（https：//docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo）这个仓库，而不是使用它作为一个模板。这也将允许您[同步您的副本]（https：//docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork）模板到您的fork。

不幸的是，像学术页面这样的模板主题的一个后勤问题使得修复错误和更新核心主题有点棘手。如果使用此模板并对其进行自定义，则在尝试同步时可能会出现合并冲突。如果你想保存你的各种.yml配置文件和markdown文件，你可以删除仓库并再次分叉。或者你可以手动打补丁。
