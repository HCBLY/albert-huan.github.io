学术页面
页面构建部署

Academic Pages 是用于学术网站的 Github Pages 模板。

开始
如果您没有 GitHub 帐户，请注册一个 GitHub 帐户并确认您的电子邮件（必填！
单击右上角的“使用此模板”按钮。
在“新建仓库”页面上，输入仓库名称为“[您的 GitHub 用户名].github.io”，这也是您网站的 URL。
设置站点范围的配置并添加内容。
将任何文件（如 PDF、.zip 文件等）上传到目录。它们将显示在 https://[您的 GitHub 用户名].github.io/files/example.pdf。files/
通过转到“GitHub 页面”部分中的存储库设置来检查状态
（可选）使用文件夹中的 Jupyter 笔记本或 python 脚本从 TSV 文件生成发布和谈话的 Markdown 文件。markdown_generator
更多信息请访问 https://academicpages.github.io/

在本地运行
当您最初使用您的网站时，在将更改推送到 GitHub 之前能够在本地预览更改非常有用。要在本地工作，您需要：

克隆存储库并进行更新，如上所述。

确保你已经安装了 ruby-dev、bundler 和 nodejs

在大多数 Linux 发行版和 Windows 子系统 Linux 上，命令为：

sudo apt install ruby-dev ruby-bundler nodejs
在 MacOS 上，命令包括：

brew install ruby
brew install node
gem install bundler
运行以安装 ruby 依赖项。如果遇到错误，请删除 Gemfile.lock，然后重试。bundle install

运行以生成 HTML 并从本地服务器提供它，将在更改时自动重建和刷新页面。jekyll serve -l -H localhostlocalhost:4000

如果您在 Linux 上运行，则可能需要先安装一些额外的依赖项，然后才能在本地运行：sudo apt install build-essential gcc make

保养
模板的 bug 报告和功能请求应通过 GitHub 提交。有关如何设置模板样式的问题，请随时在 GitHub 上开始新的讨论。

这个存储库是由Stuart Geiger从Minimal Mistakes Jekyll主题中分叉出来的（然后分离），该主题是© 2016年的Michael Rose，并在MIT许可证下发布（见 LICENSE.md）。它目前由 Robert Zupko 维护，欢迎其他维护者。

Bug 修复和增强功能
如果您有要作为拉取请求提交的错误修复和增强功能，则需要分叉此存储库，而不是将其用作模板。这也将允许您将模板副本同步到您的分支。

不幸的是，像学术页面这样的模板主题存在一个后勤问题，这使得对核心主题进行错误修复和更新变得有点棘手。如果使用此模板并对其进行自定义，则在尝试同步时可能会遇到合并冲突。如果要保存各种.yml配置文件和 Markdown 文件，可以删除存储库并重新分叉。或者您可以手动修补。
