---
title: 创建 OneNote 页
description: " Microsoft 365 中的企业笔记本"
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: 4bfd49759e7503992592492b17775e1d7ffb54015434dcca4a628afc0779550b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54165572"
---
# <a name="create-onenote-pages"></a>创建 OneNote 页

**适用于**：OneDrive 上的消费者笔记本 | Microsoft 365 上的企业级笔记本

若要创建 OneNote 页面，请向 *pages* 终结点发送一个 POST 请求。 例如：

`POST ../notes/sections/{id}/pages`

<br/>

发送在邮件正文中定义页面的 HTML。 如果请求成功，Microsoft Graph 将返回 201 HTTP 状态代码。


> **注意：** 若要了解有关可以发送以创建节、节组和笔记本的 POST 请求，请参阅我们的 [交互式 REST 参考](https://dev.onenote.com/docs)。


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a>构建请求 URI

若要构建 POST 请求 URI，请从服务根 URL 开始：

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

然后追加 *页面* 终结点：

- **在任何节中创建页面（由节名称指定）**<br/><br/>`.../pages?sectionName=DefaultSection`

- **在任何节中创建页面（由 ID 指定）**<br/><br/>`.../sections/{section-id}/pages` 

如果要在用户的个人笔记本中创建页面，Microsoft Graph 还提供了可用于在默认笔记本中创建页面的终结点：

- **在默认笔记本的默认节中创建页面**<br/><br/>`../pages` 



完整的请求 URI 类似于以下示例之一：

- `https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?sectionName=Homework`

了解有关[服务根 URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url) 的详细信息。

<a name="post-pages-section-name"></a>

### <a name="using-the-sectionname-url-parameter"></a>使用 *sectionName* URL 参数

使用 *sectionName* 参数在默认笔记本的命名节中创建页面时，适用以下规则：

- 仅顶级节可以引用（不是节组中的节）。

- 如果默认笔记本中不存在带指定名称的节，API 将自动创建该节。 这些字符不允许出现在节名称中：`? * \ / : < > | & # " % ~`

- 出于匹配原因，节名称不区分大小写，但创建节时要保留大小写。 因此，“My New Section”将以此方式显示，但“my new section”也会在后面的文章中匹配。

- 节名称必须为 URL 编码。 例如，空格必须编码为 *%20*。

- *SectionName* 参数仅对`../notes/pages`路由（不是 `../notes/sections/{id}/pages`）有效。

由于如果不存在节便会进行创建，因此在应用创建的每一个页面上使用此调用都是安全的。 用户可以重命名节，但 API 将创建一个使用你所提供的 sectionName 的新分区。 

> **注意：** API 针对重命名节中的页面返回的链接仍然会到达那些旧页面。 


<a name="message-body"></a>

## <a name="construct-the-message-body"></a>构造邮件正文

定义页面内容的 HTML 被称为 *输入 HTML*。 输入 HTML 支持[标准 HTML 和 CSS 子集](#supported-html-and-css-for-onenote-pages)，并增添了自定义属性。 （**data-id** 和 **data-render-src** 等自定义属性在 [输入和输出 HTML](onenote-input-output-html.md) 中进行了说明。） 

在 POST 请求的邮件正文中发送输入 HTML。 你可以使用 `application/xhtml+xml` 或 `text/html` 内容类型直接在邮件正文中发送输入 HTML，也可以在多部分请求的“演示文稿”部件中发送它。 

以下示例直接在邮件正文中发送输入 HTML。

```html
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Authorization: Bearer {token}
Content-Type: application/xhtml+xml

<!DOCTYPE html>
<html>
  <head>
    <title>A page with a block of HTML</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>This page contains some <i>formatted</i> <b>text</b> and an image.</p>
    <img src="https://..." alt="an image on the page" width="500" />
  </body>
</html>
```

<br/>

如果要发送二进制数据，则必须使用[多部分请求](#example-request)。 

> **注意：** 为简化编程和应用的一致性，可以使用多部分请求来创建所有页面。 最好使用库来构造多部分邮件。 这样可减少创建格式不正确的有效负载的风险。


<a name="input-html-rules"></a>

### <a name="requirements-and-limitations-for-input-html-in-post-pages-requests"></a>POST 页面请求中有关输入 HTML 的要求和限制

发送输入 HTML 时，请注意这些常规要求和限制：  

- 输入 HTML 应为 UTF-8 编码且格式标准的 XHTML。 所有容器开始标记都要求匹配结束标记。 所有属性值必须使用双引号或单引号引住。  <!--docs say MUST be encoded-->

- JavaScript 代码、包含的文件和 CSS 会被删除。 

- HTML 表单将全部删除。  

- Microsoft Graph 支持 [HTML 元素的子集](#supported-html-and-css-for-onenote-pages)。 

- Microsoft Graph 支持常见 HTML 属性的子集和一组自定义属性，如用于更新页面的 **data-id** 属性。 有关受支持的属性，请参阅[输入和输出 HTML](onenote-input-output-html.md)。


<a name="supported-html"></a>

### <a name="supported-html-and-css-for-onenote-pages"></a>OneNote 页面受支持的 HTML 和 CSS

并非所有元素、特性和属性都受支持（在 HTML4、XHTML、CSS、HTML5 等中）。 相反，Microsoft Graph 接受一组有限的 HTML，以更好地适应用户使用 OneNote 的方式。 有关详细信息，请参阅 [HTML 标记对页面的支持](https://dev.onenote.com/docs#/introduction/html-tag-support-for-pages)。 如果其中未列出标记，则可能被忽略。

<!--Microsoft Graph only accepts UTF-8 data. Be sure that all requests are encoded that way, and your content-type headers indicate that as well. xx our examples don't show this-->

以下列表显示 Microsoft Graph 支持的基本元素类型：

- `<head>` 和 `<body>`</p>
- `<title>` 和 `<meta>`，用于设置页面标题和创建日期</p>
- `<h1>` 至 `<h6>`，用于节标题</p>
- `<p>` 用于段落</p>
- `<ul>`、`<ol>` 和 `<li>`，用于列表和列表项</p>
- `<table>`、`<tr>` 和 `<td>`，包括嵌套表</p>
- `<pre>` 用于预设格式的文本（会保留空格和换行符）</p>
- `<b>` 和 `<i>`，用于粗体和斜体字符样式</p>

Microsoft Graph 在创建页面时会保留输入 HTML 的语义内容和基本结构，但会转换输入 HTML 以使用一组受支持的 HTML 和 CSS。 OneNote 中不存在的功能没有任何内容可以转换，因此，它们可能无法在源 HTML 中识别。 


<a name="example"></a>

## <a name="example-request"></a>示例请求

这个多部分请求示例创建了一个包含图像和嵌入式文件的页面。 必需的 **演示** 部分包含定义页面的输入 HTML。 **ImageBlock1** 部分包含二进制图像数据，**fileBlock1** 包含二进制文件数据。 数据部分也可包含 HTML，其中 Microsoft Graph 在 OneNote 页面上[将 HTML 呈现为一个图像](onenote-images-files.md#add-an-image-using-binary-data)。 

```html
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Authorization: Bearer {token}
Content-Type: multipart/form-data; boundary=MyPartBoundary198374

--MyPartBoundary198374
Content-Disposition:form-data; name="Presentation"
Content-Type:text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with rendered images and an attached file</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>Here's an image from an <i>online source</i>:</p>
    <img src="https://..." alt="an image on the page" width="500" />
    <p>Here's an image uploaded as <b>binary data</b>:</p>
    <img src="name:imageBlock1" alt="an image on the page" width="300" />
    <p>Here's a file attachment:</p>
    <object data-attachment="FileName.pdf" data="name:fileBlock1" type="application/pdf" />
  </body>
</html>

--MyPartBoundary198374
Content-Disposition:form-data; name="imageBlock1"
Content-Type:image/jpeg

... binary image data ...

--MyPartBoundary198374
Content-Disposition:form-data; name="fileBlock1"
Content-Type:application/pdf

... binary file data ...

--MyPartBoundary198374--
```

有关介绍如何创建包含图像和其他文件的页面的更多示例，请参阅[添加图像和文件](onenote-images-files.md)、我们的[教程](/previous-versions/office/office-365-api/how-to/onenote-tutorial)及[示例](https://github.com/onenotedev)。 此外，了解如何针对名片捕获、线上食谱和产品列表[创建绝对定位元素](onenote-abs-pos.md)、[使用笔记标记](onenote-note-tags.md)和[提取数据](onenote-extract-data.md)。

Microsoft Graph 对某些格式非常严格，如多部分邮件正文中的 CRLF 换行符。 为降低创造格式不正确的有效负载的风险，应使用库来构造多部分消息。 

如果收到格式不正确有效负载的 400 状态，请检查换行符和空格的格式，并检查编码问题。 例如，请尝试使用 `charset=utf-8`（示例：`Content-Type: text/html; charset=utf-8`）。

请参阅[输入 HTML 的要求和限制](#requirements-and-limitations-for-input-html-in-post-pages-requests)，以及 [POST 请求的大小限制](onenote-images-files.md#size-limitations-for-post-pages-requests)。


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-post-pages-requests"></a>*POST 页面* 请求的请求和响应信息

| 请求数据 | 说明 |  
|------|------|  
| 协议 | 所有请求均使用 SSL/TLS HTTPS 协议。 |  
| 授权标头 | <p>`Bearer {token}`，其中 `{token}` 是已注册应用的一个有效 OAuth 2.0 访问令牌。</p><p>如果缺少或无效，则请求失败，并显示 401 状态代码。 请参阅[身份验证和权限](permissions-reference.md)。</p> |  
| Content-Type 标头 | <p>HTML 内容的 `text/html` 或 `application/xhtml+xml`，确定是直接在邮件正文中发送还是在多部分请求的“演示”部分中发送。</p><p>发送二进制数据时，多部分请求是必需的，并使用 `multipart/form-data; boundary=part-boundary` 内容类型，其中 `{part-boundary}` 是一个字符串，表示每个数据部件的开始和结束。</p> |  
| 接受标头 | `application/json` | 

<br/>

| 响应数据 | 说明 |  
|------|------|  
| 成功代码 | 201 HTTP 状态代码。 |  
| 响应正文 | 采用 JSON 格式的新页的 OData 表示形式。 |  
| 错误 | 如果请求失败，API 将在响应正文的 **\@api.diagnostics** 对象中返回错误。 |  
| 位置标头 | 新页的资源 URL。 |  
| X-CorrelationId 标头 | 唯一标识请求的 GUID。在与 Microsoft 支持部门协作来解决问题时，可以使用此值和日期标头值。 |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a>构建 Microsoft Graph 服务根 URL

Microsoft Graph 服务根 URL 为 Microsoft Graph 的所有调用使用以下格式：

`https://graph.microsoft.com/{version}/me/onenote/`  

URL 中的 `version` 段表示想要使用的 Microsoft Graph 的版本。 `v1.0` 用于稳定的生产代码。 `beta` 用于试用正在开发的功能。 Beta 版中的特性和功能可能会有所更改，因此，不应将其用于生产代码。 

为当前用户可以访问的 OneNote 内容（拥有和共享）使用 `me`。 为指定用户已与当前用户共享的 OneNote 内容（此 URL 中）使用 `users/{id}`。 使用 [Microsoft Graph](https://graph.microsoft.com/v1.0/users) 获取用户 ID。 

<a name="limitations"></a>

## <a name="onenote-section-size-limitations"></a>OneNote 分区大小限制
对可使用 OneNote API 添加到分区的页面数量有一些限制。 当某个分区达到此限制并尝试在该分区中创建新页面时，你将看到 HTTP 状态代码为 `507` 的响应，并显示消息“已超出每个分区允许的最大页面数”。 有关此错误代码的详细信息，请参阅 [OneNote 错误代码](onenote-error-codes.md)。

可以使用下列解决办法之一：
- 创建新分区并从中添加新页面。
- 删除已达到页面限制的现有分区的未使用页面。

<a name="permissions"></a>

## <a name="permissions"></a>权限

若要创建 OneNote 页面，需要请求相应的权限。 选择应用运行所需的最低级别的权限。

从以下项中进行选择：

- Notes.Create
- Notes.ReadWrite
- Notes.ReadWrite.All

有关权限范围及其工作方式的详细信息，请参阅 [Microsoft Graph 权限引用](permissions-reference.md)。




<a name="see-also"></a>

## <a name="see-also"></a>另请参阅

- [添加图像和文件](onenote-images-files.md)
- [创建绝对定位的元素](onenote-abs-pos.md)  
- [提取数据](onenote-extract-data.md)
- [使用笔记标记](onenote-note-tags.md)
- [与 OneNote 集成](integrate-with-onenote.md)
- [OneNote 开发者博客](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Microsoft Q&A 上的 OneNote 开发问题](/answers/topics/microsoft-graph-notes.html)
- [OneNote GitHub 存储库](https://go.microsoft.com/fwlink/?LinkID=390178)