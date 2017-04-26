# <a name="contribute-to-microsoft-graph-documentation"></a>参与 Microsoft Graph 文档

感谢你对 Microsoft Graph 文档的关注！ 

* [参与方法](#ways-to-contribute)
* [我们可以接受拉取请求的先决条件](#before-we-can-accept-your-pull-request)
* [存储库结构](#repository-organization)
* [使用 GitHub、Git 和此存储库](#use-github-git-and-this-repository)
* [如何使用 Markdown 设置主题格式](#how-to-use-markdown-to-format-your-topic)
* [标准 Markdown](#standard-markdown)
* [更多资源](#more-resources)

## <a name="ways-to-contribute"></a>参与方法

可以通过下面这些方法参与 [Microsoft Graph 文档](http://developer.microsoft.com/en-us/graph/docs)：

* 通过 [Microsoft Graph 开发者文档公共存储库](https://github.com/microsoftgraph/microsoft-graph-docs)提交文章
* 通过 [GitHub 问题](https://github.com/microsoftgraph/microsoft-graph-docs/issues)举报文档缺陷
* 向 [Office 开发者平台 UserVoice](http://officespdev.uservoice.com) 添加文档请求

## <a name="before-we-can-accept-your-pull-request"></a>我们可以接受拉取请求的先决条件

### <a name="minor-corrections"></a>次要更正

针对此存储库中的文档和代码示例提交次要更正或说明时，无需发送参与许可协议 (CLA)。提交形式为拉取请求。我们会尽力在 10 个工作日内评审拉取请求。


### <a name="larger-submissions"></a>大型提交

如果提交的是文档和代码示例的新更改或重大更改，需要先向我们发送已签名的参与许可协议 (CLA)，然后我们才能接受你的拉取请求（如果你属于以下任意一组的话）：

* Microsoft Open Technologies 组成员
* 不在 Microsoft 供职的参与者

作为社区成员，**必须先签署参与许可协议 (CLA)，然后才能向此项目提交大量内容**，但只需要填写和提交一次此协议。请仔细阅读此协议；可能还需要让你的雇主签署此协议。

签署参与许可协议 (CLA) 并未授予向主存储库提交内容的权利，但确实表示 Office 开发者和 Office 开发者内容发布团队可以查看并考虑你提交的内容；如果被我们采纳，你将获得相应的奖励。

可以单击[此处](https://github.com/microsoftgraph/microsoft-graph-docs/raw/master/Contribution%20License%20Agreement.pdf)下载参与许可协议 (CLA)。请填写此表单，然后通过电子邮件的方式将它发送到 [officedev@microsoft.com](mailto:officedev@microsoft.com)。

收到和处理你的 CLA 后，我们便会尽力在 10 个工作日内评审你的拉取请求。

## <a name="repository-organization"></a>存储库结构

microsoft-graph-docs 存储库中的内容先按文章语言进行分组，然后再按主题进行分组。每个主题目录的根中的 README.md 文件指定了本主题内文件的结构。

每个主题内的文章是以 MADN GUID 命名，而不是以标题命名。这是我们的文档管理流程的一个弊端，目前还无法更改。我们强烈建议使用每个主题目录内的目录转到要查看或编辑的文件。有关详细信息，请参阅 [README.md](https://github.com/microsoftgraph/microsoft-graph-docs/blob/master/README.md)。

## <a name="use-github-git-and-this-repository"></a>使用 GitHub、Git 和此存储库

**注意：** 此部分中的大多数信息收录在 [GitHub 帮助] []文章中。如果已熟悉 Git 和 GitHub，请跳至“**参与和编辑内容**”部分，查看此存储库中代码/内容流的详细信息。

### <a name="setting-up-your-fork-of-the-repository"></a>设置存储库分叉

1.    创建一个用于参与此项目的 GitHub 帐户。如果尚未创建，请转到 [GitHub 主页] []立即创建。
2.    在计算机上安装 Git。请按[安装 Git 教程] [Set Up Git]中的说明操作。
3.    创建你自己的此存储库分叉。为此，请单击页面顶部的“**分叉**”按钮。
4.    将自己的分叉复制到本地计算机上。为此，请打开 GitBash。在命令提示符处输入以下命令：

        git clone https://github.com/{your user name}/microsoft-graph-docs.git

    然后，输入以下命令，创建对根存储库的引用：

        cd microsoft-graph-docs   git remote add upstream https://github.com/microsoftgraph/microsoft-graph-docs.git   git fetch upstream

恭喜你！现已设置好存储库。无需再次重复上述步骤。

### <a name="contribute-and-edit-content"></a>参与和编辑内容

若要尽可能顺利地参与其中，请按以下过程操作。

1. 新建分支。
2. 添加新内容或编辑现有内容。
3. 向主存储库提交拉取请求。
4. 删除分支。

将每个分支限制为只包含一个概念/文章，以简化工作流并降低合并冲突发生的概率。新分支支持以下参与类型：

* 新增文章（及相关图像）
* 编辑文章中的单词拼写和语法
* 跨大量文章应用一个格式更改（例如，应用新的版权页脚）。

#### <a name="create-a-new-branch"></a>新建分支

1.    打开 GitBash。
2.    在提示符处键入 `git pull upstream master:<new branch name>`。此命令在本地新建分支，该分支是从最新的 microsoftgraph master 分支复制而来。**注意：** 对于内部参与者，将命令中的 `master` 替换为要在特定日期发布的分支。
3.    在提示符处键入 `git push origin <new branch name>`。此命令将提醒 GitHub 注意这个新分支。现在，应该可以在 GitHub 存储库的分叉上看到这个新分支。
4.    键入 `git checkout <new branch name>` 切换到新分支。

#### <a name="add-new-content-or-edit-existing-content"></a>添加新内容或编辑现有内容

使用文件资源管理器转到本地计算机上的存储库。存储库文件位于 `C:\Users\<yourusername>\microsoft-graph-docs`。

若要编辑文件，请在所选的编辑器中打开并修改文件。若要新建文件，请使用所选的编辑器，在本地存储库副本中的适当位置上存储新文件。操作期间，请务必经常保存操作。

`C:\Users\<yourusername>\microsoft-graph-docs` 中的文件是你在本地存储库中创建的新分支的工作副本。提交更改前，在此文件夹的任何更改都不会影响本地存储库。若要向本地存储库提交更改，在 GitBash 中键入以下命令：

    git add .
    git commit -v -a -m "<Describe the changes made in this commit>"

`add` 命令将更改添加到临时区域以准备将其提交到存储库。`add` 命令表明你希望将所有已添加或修改的文件暂存后，对子文件夹进行递归查看。（若不希望提交所有更改，可以添加特定的文件）。也可以撤消提交。要请求帮助，请键入 `git add -help` 或 `git status`。）

`commit` 命令将暂存更改提交到存储库中。`-m` 表示要在命令行中提供提交注释。如果你并不希望在某个特定日期进行发布，可以说“尽快发布”。-v 和 -a 开关可以省略。-v 开关用于命令的详细输出，-a 与添加命令的用途相同。 

可以在工作期间多次提交，也可以等待完成，然后一次性提交。

#### <a name="submit-a-pull-request-to-the-main-repository"></a>向主存储库提交拉取请求

如果已完成工作且已准备好将其合并到中央存储库内，请按以下步骤操作。

1.    在 GitBash 中的命令提示符处键入 `git push origin <new branch name>`。在本地存储库中，`origin` 代表从中复制本地存储库的 GitHub 存储库。此命令将新分支的当前状态（包括上述步骤中的所有提交）推送到 GitHub 分叉。
2.    在 GitHub 网站上，在自己的分叉中转到新分支。
3.    单击页面顶部的“**拉取请求**”按钮。
4.    请确保基本分支是 `microsoftgraph/microsoft-graph-docs@master`，且头分支是 `<your username>/microsoft-graph-docs@<branch name>`。
5.    单击“**更新提交范围**”按钮。
6.    为拉取请求添加标题，然后说明要进行的所有更改。如果是 UserVoice 项或 GitHub 问题 bug 修复，请务必在说明中引用相应的问题。
7.    提交拉取请求。

一位网站管理员现在将处理你的拉取请求。你的拉取请求将出现在 microsoftgraph/microsoft-graph-docs 网站上的“问题”下。如果拉取请求被接受，即表示问题已解决。

#### <a name="create-a-new-branch-after-merge"></a>合并后新建分支

在分支成功合并（即拉取请求被接受）后，请勿继续使用已在上游成功合并的本地分支。如果你提交其他拉取请求，这可能会导致合并冲突出现。相反，若要进行其他更新，根据已在上游成功合并的分支新建本地分支。

例如，假设本地分支 X 已成功合并到 microsoftgraph/microsoft-graph-docs master 分支中，且你希望对已合并的内容进行其他更新。根据 microsoftgraph/microsoft-graph-docs master 分支新建本地分支 X2。为此，请打开 GitBash，然后执行以下命令：

    cd microsoft-graph-docs
    git pull upstream master:X2
    git push origin X2

现在已有在分支 X 中提交的工作的本地副本（在新的本地分支中）。由于 X2 分支还包含其他作者合并的所有工作，因此如果你的工作依赖其他人的工作（例如，共享的图像），其他人的工作也包含在新分支中。可以查看新分支并验证内容，验证之前的工作（及其他人的工作）…

    git checkout X2

…是否包含在此分支中。（`checkout` 命令将 `C:\Users\<yourusername>\microsoft-graph-docs` 中的文件更新为 X2 分支的当前状态。）查看新分支后，可以对内容进行更新并以常用方式将其提交。但是为了避免误在已合并的分支 (X) 进行操作，最好将其删除（请参阅下列“**删除分支**”部分）。

#### <a name="delete-a-branch"></a>删除分支

成功将更改合并到中央存储库后，就可以将使用的分支删除，因为不再需要使用这个分支了。必须通过新分支完成其他任何工作。  

若要删除分支，请按以下步骤操作：

1.    在 GitBash 中的命令提示符处键入 `git checkout master`。这命令可确保你不在要删除的分支中（严禁出现这样的行为）。
2.    接下来，在命令提示符处键入 `git branch -d <branch name>`。只有当分支已成功合并到上游存储库中，此命令才会在本地计算机上删除分支。（可以使用 `???D` 标记替代此行为，但首先请确保你要这么做。）
3.    最后，在命令提示符中键入 `git push origin :<branch name>`（冒号前有一个空格，之后没有空格）。这将删除 github 分叉中的分支。  

恭喜！你已成功参与此项目！

## <a name="how-to-use-markdown-to-format-your-topic"></a>如何使用 Markdown 设置主题格式

### <a name="standard-markdown"></a>标准 Markdown

此存储库中的所有文章都使用 Markdown。我们将介绍所需的基础知识，因为 [Markdown 主页] []中有完整介绍（并列出了所有语法）。

如果要寻找实用的编辑器，请尝试 [Markdown Pad][]。


### <a name="markdown-basics"></a>Markdown 基础知识

下面列出了最常见的 markdown 语法：

*    **换行符与段落：** Markdown 中没有 HTML `<br />` 元素。相反，新段落是通过两个文本块之间的空行进行指定。
*    **斜体：** HTML `<i>some text</i>` 编写为 `*some text*`
*    **粗体：** HTML `<strong>some text</strong>` 元素编写为 `**some text**`
*    **标题：** HTML 标题由行开头的 `#` 字符数指定。`#` 字符数对应于标题的层级（例如，`#` = h1、`##` = h2 和 `###` = h3）。
*    **编号列表：** 若要创建编号（经过排序的）列表，请在代码行的开头添加 `1. `。若要在一个列表元素内添加多个元素，请按如下方式设置列表格式：
        
        1.    Notice that this line is tabbed over after the '.'
        
            Now notice that there is a line break between the two paragraphs in the list element, and that the indentation here matches the indentation of the line above.

*    **点符列表：** 点符（未经排序的）列表几乎与经过排序的列表完全相同，唯一的区别在于 `1. ` 被替换为 `* `、`- ` 或 `+ `。多元素列表的工作方式与它们在经过排序的列表中的工作方式相同。
*    **链接：** 链接的基本语法是 `[visible link text](link url)`。

    链接还可以包含引用，我们将在下面的**链接和图像引用**部分中对此进行介绍。

*    **图像：** 图像的基本语法是 `![alt text for the image](image url)`。

    图像还可以包含引用，我们将在下面的**链接和图像引用**部分中对此进行介绍。

*    **内嵌 HTML：** Markdown 允许内嵌 HTML：Markdown 以<i>斜体</i>形式正确呈现 `<i>italic</i>`。

### <a name="link-and-image-references"></a>链接和图像引用

Markdown 提供一项很实用的功能，即允许用户插入图像和链接引用（而不是 URL）。下面展示了使用此功能的语法：

    The image below is from [Google][googleweb]
    
    ![Google's logo][logo]
    
    [googleweb]: http://www.google.com
    [logo]: https://www.google.com/images/srpr/logo3w.png

使用文件底部分组的引用，可以轻松地查找、编辑和重复使用链接和图像 URL。 


## <a name="more-resources"></a>更多资源

* 有关 Markdown 的详细信息，请转到 [Markdown 网站][Markdown 主页]。
* 若要详细了解如何使用 Git 和 GitHub，请先查看 [GitHub 帮助部分] [GitHub 帮助]。如有必要，请联系网站管理员。

[GitHub 主页]: http://github.com
[GitHub 帮助]: http://help.github.com/
[Set Up Git]: http://help.github.com/win-set-up-git/
[Markdown 主页]: http://daringfireball.net/projects/markdown/
[Markdown Pad]: http://markdownpad.com/
[microsoftgraph/microsoft-graph-docs issues]: https://github.com/microsoftgraph/microsoft-graph-docs/issues
