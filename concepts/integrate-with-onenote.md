---
title: OneNote API 概述
description: 使用 Microsoft Graph 中的 OneNote API 访问 OneNote 笔记本、分区和页面，以创建可帮助用户规划和组织想法和信息的解决方案。
author: Jewan-microsoft
ms.localizationpriority: high
ms.prod: onenote
ms.custom: scenarios:getting-started
ms.openlocfilehash: b8f8c01955d0ede7bfad843cebb783eb5f9f268f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444899"
---
# <a name="onenote-api-overview"></a>OneNote API 概述

OneNote 是一个数字笔记本，可让客户通过在 Web、手机、平板电脑或桌面上键入、草绘或语音来跟踪家庭、学校或工作方面的想法和笔记。 用户可以随意整理笔记、切换设备、接续之前的工作，以及通过与他人实时交互笔记展开协作。

> [!VIDEO https://www.youtube-nocookie.com/embed/VXd4OeQU1ek]

## <a name="why-integrate-with-onenote"></a>为什么与 OneNote 集成？

通过将应用与 OneNote 集成，可以在服务于全球数百万用户的多个平台中创建强大的体验。 可以使用 Microsoft Graph 访问 OneNote 中的笔记本、节和页面，从而创建可帮助用户计划和管理想法和信息的解决方案。

### <a name="collect-and-organize-notes-and-ideas"></a>收集并整理笔记和想法  

将 OneNote 用作画布，用户可以在其中添加和排列他们的内容。 借助 Microsoft Graph，可以轻松地编写应用，让学生做笔记并进行研究、让家庭分享计划和想法或让购物者分享图片。 应用可以捕获用户所需的信息，将其发送到 OneNote，然后帮助用户管理这些信息。

### <a name="capture-information-in-many-formats"></a>以多种格式捕获信息

捕获 HTML、嵌入的图像（源自本地或公共 URL）、视频、音频、电子邮件和其他常见的文件类型。 OneNote 甚至还能够以快照的形式呈现网页和 PDF 文件。 Microsoft Graph 支持 OneNote 页面布局的一组标准 HTML 和 CSS，因此，用户可以使用表、内嵌图像和基本格式以获取所需的外观。 

### <a name="use-the-onenote-ecosystem-to-enhance-your-core-scenarios"></a>使用 OneNote 生态系统增强核心方案

了解 OneNote 其他强大的功能。 Microsoft Graph 中的 OneNote API 在图像上运行 OCR、支持全文搜索、自动同步客户端、处理图像和提取名片捕获、联机产品以及方法列表。 针对笔记和轻型媒体，在云中将 OneNote 用作数字内存存储，或针对特定于域的数据用作数据馈送。 

### <a name="reach-millions-of-onenote-users-on-all-major-platforms"></a>服务于所有主要平台上的数百万 OneNote 用户

使用 OneNote 提高应用使用率。 在新的 Windows 设备上预安装了 OneNote，可作为 Microsoft 365 的一部分联机用于大部分平台。 发布使用功能丰富的 OneNote 环境的应用时，可以获得广泛的跨平台市场潜力。

<!-- Might be good to show a few examples of Microsoft Graph API calls here, similar to what we have in the featured scenarios topic: featured_scenarios..md You could have an H2 section called "What can I do with OneNote APIs in Microsoft Graph?"-->

## <a name="what-can-i-do-with-onenote-apis-in-microsoft-graph"></a>可以通过 Microsoft Graph 中的 OneNote API 实现什么功能？

以下是使用 OneNote 资源的一些最热门的请求。

|操作|URL|
|:--------|:--|
|获取我的笔记本|[https://graph.microsoft.com/v1.0/me/onenote/notebooks](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/notebooks&version=v1.0)|
|获取我的部分|[https://graph.microsoft.com/v1.0/me/onenote/sections](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/sections&version=v1.0)|
|获取我的页面|[https://graph.microsoft.com/v1.0/me/onenote/pages](https://developer.microsoft.com/graph/graph-explorer?request=me/onenote/pages&version=v1.0)|

## <a name="learn-more-about-onenote-apis"></a>详细了解 OneNote API

深入探索 Microsoft Graph API 以了解 OneNote 内容更新功能。 以下列表中的主题说明如何创建新的 OneNote 页并用新内容更新现有页。 此外，还将了解使用 Microsoft Graph 更新 OneNote 笔记本的最佳做法。

### <a name="work-with-onenote"></a>使用 OneNote

* [使用 OneNote REST API](/graph/api/resources/onenote-api-overview)
* [最佳做法](onenote-best-practices.md)
* [品牌塑造准则](onenote-branding.md)
* [打开 OneNote 客户端](open-onenote-client.md)
* [在 OneNote 页中使用笔记标记](onenote-note-tags.md)
* [Microsoft Graph 中的 OneNote API 错误代码](onenote-error-codes.md)

### <a name="work-with-onenote-pages"></a>使用 OneNote 页

* [OneNote 页中的输入和输出 HTML](onenote-input-output-html.md)
* [使用 Microsoft Graph 获取 OneNote 内容和结构](onenote-get-content.md)
* [创建 OneNote 页](onenote-create-page.md)
* [更新 OneNote 页内容](onenote-update-page.md)

### <a name="work-with-onenote-page-content"></a>使用 OneNote 页内容

* [在 OneNote 页中创建绝对定位的元素](onenote-abs-pos.md)
* [将图像、视频和文件添加到 OneNote 页](onenote-images-files.md)
* [使用 OneNote API div 标记从捕获内容中提取数据](onenote-extract-data.md)

## <a name="api-reference"></a>API 参考

在查找此服务的 API 参考？

- [Microsoft Graph v1.0 中的 OneNote API](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0&preserve-view=true)
- [Microsoft Graph beta 中的 OneNote API](/graph/api/resources/onenote-api-overview?view=graph-rest-beta&preserve-view=true)

## <a name="see-also"></a>另请参阅

了解仅对 OneNote 服务专用 REST 终结点公开的其他一些 OneNote 功能。

- [OneNote 开发](/previous-versions/office/office-365-api/how-to/onenote-landing)
- [处理课堂笔记本](/previous-versions/office/office-365-api/how-to/onenote-classnotebook)
- [使用异步课堂笔记本](/previous-versions/office/office-365-api/how-to/onenote-classnotebook-asynchronous)
- [使用教职员工笔记本](/previous-versions/office/office-365-api/how-to/onenote-staffnotebook)
- [复制笔记本、节和页面](/previous-versions/office/office-365-api/how-to/onenote-copy)
- [管理 OneNote 实体的权限](/previous-versions/office/office-365-api/how-to/onenote-manage-perms)
- [使用网页上的 OneNote 保存对话框](/previous-versions/office/office-365-api/how-to/onenote-save-dialog)
- [订阅 Webhook](/previous-versions/office/office-365-api/how-to/onenote-sync)

## <a name="next-steps"></a>后续步骤

- 使用 [Microsoft Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)在你自己的 OneNote 笔记本中试用 OneNote API。

- 若要在 Graph 浏览器中进行 OneNote API 调用，请选择左侧栏中的“显示更多示例”。 使用菜单将 OneNote 切换至“打开”。 还需要启用相应的权限。 在左侧菜单中的帐户名称中，选择“修改权限”。 有关 OneNote 权限的详细信息，请参阅[笔记权限](permissions-reference.md#notes-permissions)。
