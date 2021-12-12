# [GitHub Desktop 文档](https://docs.github.com/cn/desktop)
设置和使用 GitHub Desktop 管理项目工作的分步指南。

## 安装和配置 GitHub Desktop
获取 GitHub Desktop 设置以管理项目工作。 向 GitHub.com 或 GitHub Enterprise 验证，保持应用程序的更新，并检查您的首选设置。

### 概览
了解 GitHub Desktop 并快速创建您的第一个仓库。

#### GitHub Desktop 使用入门
了解如何设置、验证和配置 GitHub Desktop，以便直接从您的计算机直接参与项目。

GitHub Desktop 是一个可让您使用 GUI 而非命令行或网络浏览器与 GitHub 交互的应用程序。 GitHub Desktop 鼓励您和您的团队使用最佳实践协作处理 Git 和 GitHub。 您可以使用 GitHub Desktop，通过视觉确认更改从桌面完成大部分 Git 命令。 您可以使用 GitHub Desktop 推送到、从中拉取和克隆远程仓库，以及使用协作工具，如归因提交和创建拉取请求。

### 配置和自定义

#### 配置默认编辑器
您可以配置 GitHub Desktop 在项目中使用您首选的文本编辑器或集成开发环境 (IDE) 打开文件。

##### 支持的编辑器
GitHub Desktop 支持以下编辑器。

Atom
Visual Studio Code
Visual Studio Codium
Sublime Text
ColdFusion Builder
Typora
SlickEdit
JetBrains WebStorm
JetBrains PhpStorm
JetBrains Rider
Notepad++

##### 配置默认编辑器
File（文件）菜单，然后单击 Options（选项），在 Options（选项）窗口中，选择 Integrations（集成）。使用“External Editor（外部编辑器）”下拉菜单，选择要设为默认的编辑器。单击 Save（保存）。

## 参与和协作

### 从 GitHub Desktop 克隆和复刻仓库
您可以使用 GitHub Desktop 克隆和复刻 GitHub 上的仓库。

GitHub 上的仓库是远程仓库。 您可以通过 GitHub Desktop 克隆或复刻仓库以在计算机上创建本地仓库。

您可以通过克隆仓库创建 GitHub 上您可以访问的任何仓库的本地副本。如果您拥有一个仓库或拥有写入权限，您可以在本地和远程位置之间进行同步。当您克隆仓库时，您推送到 GitHub 的任何更改都将影响原始仓库。 要在不影响原始项目的情况下进行更改，您可以通过复刻仓库来创建单独的副本。您可以创建拉取请求来提议维护员将您的复刻中的更改加入原始上游仓库。

### 为本地仓库创建别名
您可以为本地仓库创建一个别名，以帮助在 GitHub Desktop 中区分同名的仓库。 创建别名不影响在 GitHub 上的仓库名称。 在仓库列表中，别名以斜体显示。

### 管理分支
您可以在仓库的默认分支之外创建分支，以便安全地试验更改。

如果您对仓库具有读取权限，可随时在 GitHub Desktop 中创建分支， 但如果您对仓库具有写入权限，则只能将分支推送到 GitHub。

仓库管理员可对分支启用保护。 如果您处理的是受保护分支，将无法删除或强制推送到该分支。 在分支可以合并之前，仓库管理员可以另外启用其他受保护分支设置来实施特定的工作流程。 

# [开始使用Git](https://docs.github.com/cn/get-started/getting-started-with-git)
设置 Git（一个分布式版本控制系统）以从计算机管理您的 GitHub 仓库。

## 忽略文件
您可以配置 Git 忽略您不想检入 GitHub 的文件。

### 为单个仓库配置忽略的文件
您可以在仓库的根目录中创建 .gitignore 文件，指示 Git 在您进行提交时要忽略哪些文件和目录。 要与克隆仓库的其他用户共享忽略规则，请提交 .gitignore 文件到您的仓库。

GitHub 在 github/gitignore 公共仓库中维护建议用于许多常用操作系统、环境及语言的 .gitignore 文件正式列表。 您也可以使用 gitignore.io 创建 .gitignore 文件，以用于操作系统、编程语言或 IDE。 

### 为计算机上的所有存储库配置忽略的文件
您也可以创建全局 .gitignore 文件，以定义忽略计算机上每个 Git 仓库中文件的规则列表。

### 排除本地文件而不创建 .gitignore 文件
如果不想创建 .gitignore 文件与其他人共享，可以创建不随仓库提交的规则。 您可以对不希望其他用户生成的本地生成文件使用此方法，例如编辑者创建的文件。

使用您常用的文本编辑器打开 Git 仓库根目录中的文件 .git/info/exclude。 您在此处添加的任何规则都不会检入，并且只会对您的本地仓库忽略文件。

# [使用Git](https://docs.github.com/cn/get-started/using-git)
##About Git
了解版本控制系统Git，以及它如何与GitHub配合使用。

### 关于存储库
存储库或Git项目包含与项目关联的文件和文件夹的整个集合，以及每个文件的修订历史记录。文件历史记录在时间上显示为快照，称为提交。提交可以组织成多个开发行，称为分支。因为Git是一个DVCS（Distributed Version Control System，分布式版本控制系统），所以存储库是自包含的单元，任何拥有存储库副本的人都可以访问整个代码库及其历史记录。使用命令行或其他易于使用的界面，Git存储库还允许：与历史交互、克隆存储库、创建分支、提交、合并、跨代码版本比较更改，等等。

通过GitHub这样的平台，Git还为项目透明度和协作提供了更多机会。公共存储库帮助团队协作构建尽可能最好的最终产品。

### GitHub的工作原理
GitHub托管Git存储库，并为开发人员提供工具，通过命令行功能、问题（线程化讨论）、拉取请求、代码审阅或使用GitHub市场上的免费和可供购买的应用程序集合来发布更好的代码。GitHub拥有协作层，如GitHub flow、1500万开发人员社区和数百个集成的生态系统，GitHub改变了软件的构建方式。

GitHub将协作直接构建到开发过程中。工作被组织到存储库中，开发人员可以在其中概述需求或方向，并为团队成员设定期望。然后，使用GitHub流，开发人员只需创建一个分支来处理更新，提交更改以保存它们，打开请求来提议和讨论更改，并在每个人都在同一页面上时合并请求。

### 协作开发模型
人们在GitHub上协作的主要方式有两种：

Shared repository(共享存储库)

Fork and pull

通过共享存储库，个人和团队被明确指定为具有读、写或管理员访问权限的参与者。这种简单的权限结构与受保护的分支等功能相结合，有助于团队在采用GitHub时快速进步。

对于开源项目，或者任何人都可以参与的项目，管理个人权限可能是一项挑战，但是fork-and-pull模型允许任何可以查看项目的人参与。fork是开发人员个人帐户下项目的副本。每个开发人员都可以完全控制他们的fork，并且可以自由地实现修复或新功能。在forks中完成的工作要么单独保存，要么通过pull请求返回到原始项目。在那里，维护人员可以在合并建议的更改之前查看这些更改。

# [了解 GitHub](https://docs.github.com/cn/get-started/learning-about-github)
