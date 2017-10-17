# <a name="use-microsoft-graph-to-integrate-with-onenote"></a>使用 Microsoft Graph 与 OneNote 集成

通过将应用与 OneNote 集成，可以为全球数百万用户创建跨多个平台的增强体验。 可以使用 Microsoft Graph 访问 OneNote 中的笔记本、节和页面，从而创建可帮助用户计划和管理想法和信息的解决方案。

## <a name="why-create-onenote-apps"></a>为什么要创建 OneNote 应用？

可以使用 Microsoft Graph 创建和管理 OneNote 笔记本中的笔记、列表、图片、文件等内容。

### <a name="collect-and-organize-notes-and-ideas"></a>收集并管理笔记和想法  
将 OneNote 用作画布，用户可以在其中添加和排列他们的内容。 借助 Microsoft Graph，可以轻松地编写应用，让学生做笔记并进行研究、让家庭分享计划和想法或让购物者分享图片。 应用可以捕获用户所需的信息，将其发送到 OneNote，然后帮助用户管理这些信息。

### <a name="capture-information-in-many-formats"></a>以多种格式捕获信息
捕获 HTML、嵌入的图像（源自本地或公共 URL）、视频、音频、电子邮件和其他常见的文件类型。 OneNote 甚至还能够以快照的形式呈现网页和 PDF 文件。 Microsoft Graph 支持 OneNote 页面布局的一组标准 HTML 和 CSS，因此，用户可以使用表、内嵌图像和基本格式以获取所需的外观。 

### <a name="use-the-onenote-ecosystem-to-enhance-your-core-scenarios"></a>使用 OneNote 生态系统增强核心方案
了解 OneNote 其他强大的功能。 Microsoft Graph 中的 OneNote API 在图像上运行 OCR、支持全文搜索、自动同步客户端、处理图像和提取名片捕获、联机产品以及方法列表。 针对笔记和轻型媒体，在云中将 OneNote 用作数字内存存储，或针对特定于域的数据用作数据馈送。 

### <a name="reach-millions-of-onenote-users-on-all-major-platforms"></a>服务于所有主要平台上的数百万 OneNote 用户
使用 OneNote 提高应用使用率。 在新的 Windows 设备上预安装了 OneNote，可作为 Office 365 的一部分联机用于大部分平台。 发布使用功能丰富的 OneNote 环境的应用时，可以获得广泛的跨平台市场潜力。

<!-- Might be good to show a few examples of Microsoft Graph API calls here, similar to what we have in the featured scenarios topic: https://developer.microsoft.com/en-us/graph/docs/concepts/featured_scenarios. You could have an H2 section called "What can I do with OneNote APIs in Microsoft Graph?"-->

## <a name="what-can-i-do-with-onenote-apis-in-microsoft-graph"></a>可以通过 Microsoft Graph 中的 OneNote API 实现什么功能？

以下是使用 OneNote 资源的一些最热门的请求。

|操作|URL|
|:--------|:--|
|获取我的笔记本|[https://graph.microsoft.com/v1.0/me/onenote/notebooks](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me/onenote/notebooks&version=1.0)|
|获取我的分区|[https://graph.microsoft.com/v1.0/me/onenote/sections](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me/onenote/sections&version=1.0)|
|获取我的页面|[https://graph.microsoft.com/v1.0/me/onenote/pages](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me/onenote/pages&version=1.0)|

## <a name="explore-the-onenote-apis"></a>浏览 OneNote API
使用 [Microsoft Graph 浏览器](https://developer.microsoft.com/en-us/graph/graph-explorer)在你自己的 OneNote 笔记本中试用 OneNote API。

若要在 Graph 浏览器中进行 OneNote API 调用，请选择左侧栏中的“显示更多示例”****。 使用菜单将 OneNote 切换至“打开”****。 还需要启用相应的权限。 在左侧菜单中的帐户名称中，选择“修改权限”****。 有关 OneNote 权限的详细信息，请参阅[笔记权限](permissions_reference.md#notes-permissions)。

若要开始在 Microsoft Graph 中使用 OneNote API，请参阅 [OneNote 参考内容](../api-reference/v1.0/resources/onenote.md)。

## <a name="see-also"></a>另请参阅

* [品牌准则](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-branding)
* [获取 OneNote 内容和结构](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-get-content)
* [添加图像、视频和文件](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files)
* [创建绝对定位的元素](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos)
* [提取数据](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data)
* [使用笔记标记](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags)

