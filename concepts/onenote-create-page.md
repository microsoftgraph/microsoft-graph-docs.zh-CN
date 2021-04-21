---
title: 创建 OneNote 页
description: " Microsoft 365 中的企业笔记本"
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: 856a266a435bf0fb2146fc786ec72058e38debce
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920192"
---
# <a name="create-onenote-pages"></a><span data-ttu-id="469dc-103">创建 OneNote 页</span><span class="sxs-lookup"><span data-stu-id="469dc-103">Create OneNote pages</span></span>

<span data-ttu-id="469dc-104">**适用于**：OneDrive 上的消费者笔记本 | Microsoft 365 上的企业级笔记本</span><span class="sxs-lookup"><span data-stu-id="469dc-104">**Applies to**: Consumer notebooks on OneDrive | Enterprise notebooks on Microsoft 365</span></span>

<span data-ttu-id="469dc-105">若要创建 OneNote 页面，请向 *pages* 终结点发送一个 POST 请求。</span><span class="sxs-lookup"><span data-stu-id="469dc-105">To create a OneNote page, you send a POST request to a *pages* endpoint.</span></span> <span data-ttu-id="469dc-106">例如：</span><span class="sxs-lookup"><span data-stu-id="469dc-106">For example:</span></span>

`POST ../notes/sections/{id}/pages`

<br/>

<span data-ttu-id="469dc-107">发送在邮件正文中定义页面的 HTML。</span><span class="sxs-lookup"><span data-stu-id="469dc-107">Send the HTML that defines the page in the message body.</span></span> <span data-ttu-id="469dc-108">如果请求成功，Microsoft Graph 将返回 201 HTTP 状态代码。</span><span class="sxs-lookup"><span data-stu-id="469dc-108">If the request is successful, Microsoft Graph returns a 201 HTTP status code.</span></span>


> <span data-ttu-id="469dc-109">**注意：** 若要了解有关可以发送以创建节、节组和笔记本的 POST 请求，请参阅我们的 [交互式 REST 参考](https://dev.onenote.com/docs)。</span><span class="sxs-lookup"><span data-stu-id="469dc-109">**Note:** To learn about the POST requests you can send to create sections, section groups, and notebooks, see our [interactive REST reference](https://dev.onenote.com/docs).</span></span>


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a><span data-ttu-id="469dc-110">构建请求 URI</span><span class="sxs-lookup"><span data-stu-id="469dc-110">Construct the request URI</span></span>

<span data-ttu-id="469dc-111">若要构建 POST 请求 URI，请从服务根 URL 开始：</span><span class="sxs-lookup"><span data-stu-id="469dc-111">To construct the POST request URI, start with the service root URL:</span></span>

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

<span data-ttu-id="469dc-112">然后追加 *页面* 终结点：</span><span class="sxs-lookup"><span data-stu-id="469dc-112">Then append the *pages* endpoint:</span></span>

- <span data-ttu-id="469dc-113">**在任何节中创建页面（由节名称指定）**</span><span class="sxs-lookup"><span data-stu-id="469dc-113">**Create a page in any section (specified by section name)**</span></span><br/><br/>`.../pages?sectionName=DefaultSection`

- <span data-ttu-id="469dc-114">**在任何节中创建页面（由 ID 指定）**</span><span class="sxs-lookup"><span data-stu-id="469dc-114">**Create a page in any section (specified by ID)**</span></span><br/><br/>`.../sections/{section-id}/pages` 

<span data-ttu-id="469dc-115">如果要在用户的个人笔记本中创建页面，Microsoft Graph 还提供了可用于在默认笔记本中创建页面的终结点：</span><span class="sxs-lookup"><span data-stu-id="469dc-115">If you're creating pages in the user's personal notebook, Microsoft Graph also provides endpoints you can use to create pages in the default notebook:</span></span>

- <span data-ttu-id="469dc-116">**在默认笔记本的默认节中创建页面**</span><span class="sxs-lookup"><span data-stu-id="469dc-116">**Create a page in the default section of the default notebook**</span></span><br/><br/>`../pages` 



<span data-ttu-id="469dc-117">完整的请求 URI 类似于以下示例之一：</span><span class="sxs-lookup"><span data-stu-id="469dc-117">Your full request URI will look like one of these examples:</span></span>

- `https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?sectionName=Homework`

<span data-ttu-id="469dc-118">了解有关[服务根 URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url) 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="469dc-118">Learn more about the [service root URL](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).</span></span>

<a name="post-pages-section-name"></a>

### <a name="using-the-sectionname-url-parameter"></a><span data-ttu-id="469dc-119">使用 *sectionName* URL 参数</span><span class="sxs-lookup"><span data-stu-id="469dc-119">Using the *sectionName* URL parameter</span></span>

<span data-ttu-id="469dc-120">使用 *sectionName* 参数在默认笔记本的命名节中创建页面时，适用以下规则：</span><span class="sxs-lookup"><span data-stu-id="469dc-120">The following rules apply when using the *sectionName* parameter to create a page in a named section in the default notebook:</span></span>

- <span data-ttu-id="469dc-121">仅顶级节可以引用（不是节组中的节）。</span><span class="sxs-lookup"><span data-stu-id="469dc-121">Only top-level sections can be referenced (not sections within section groups).</span></span>

- <span data-ttu-id="469dc-122">如果默认笔记本中不存在带指定名称的节，API 将自动创建该节。</span><span class="sxs-lookup"><span data-stu-id="469dc-122">If a section with the specified name doesn't exist in the default notebook, the API creates it.</span></span> <span data-ttu-id="469dc-123">这些字符不允许出现在节名称中：`? * \ / : < > | & # " % ~`</span><span class="sxs-lookup"><span data-stu-id="469dc-123">These characters are not allowed for section names: `? * \ / : < > | & # " % ~`</span></span>

- <span data-ttu-id="469dc-124">出于匹配原因，节名称不区分大小写，但创建节时要保留大小写。</span><span class="sxs-lookup"><span data-stu-id="469dc-124">Section names are case-insensitive for matching, but case is preserved when sections are created.</span></span> <span data-ttu-id="469dc-125">因此，“My New Section”将以此方式显示，但“my new section”也会在后面的文章中匹配。</span><span class="sxs-lookup"><span data-stu-id="469dc-125">So "My New Section" will display like that, but "my new section" would also match on subsequent posts.</span></span>

- <span data-ttu-id="469dc-126">节名称必须为 URL 编码。</span><span class="sxs-lookup"><span data-stu-id="469dc-126">Section names must be URL-encoded.</span></span> <span data-ttu-id="469dc-127">例如，空格必须编码为 *%20*。</span><span class="sxs-lookup"><span data-stu-id="469dc-127">For example, spaces must be encoded as *%20*.</span></span>

- <span data-ttu-id="469dc-128">*SectionName* 参数仅对`../notes/pages`路由（不是 `../notes/sections/{id}/pages`）有效。</span><span class="sxs-lookup"><span data-stu-id="469dc-128">The *sectionName* parameter is valid only with the `../notes/pages` route (not `../notes/sections/{id}/pages`).</span></span>

<span data-ttu-id="469dc-129">由于如果不存在节便会进行创建，因此在应用创建的每一个页面上使用此调用都是安全的。</span><span class="sxs-lookup"><span data-stu-id="469dc-129">Because sections are created if they don't exist, it's safe to use this call with every page your app creates.</span></span> <span data-ttu-id="469dc-130">用户可以重命名节，但 API 将创建一个使用你所提供的 sectionName 的新分区。</span><span class="sxs-lookup"><span data-stu-id="469dc-130">Users might rename sections, but the API will create a new section with the section name that you supply.</span></span> 

> <span data-ttu-id="469dc-131">**注意：** API 针对重命名节中的页面返回的链接仍然会到达那些旧页面。</span><span class="sxs-lookup"><span data-stu-id="469dc-131">**Note:** The links returned by the API for pages in a renamed section will still reach those older pages.</span></span> 


<a name="message-body"></a>

## <a name="construct-the-message-body"></a><span data-ttu-id="469dc-132">构造邮件正文</span><span class="sxs-lookup"><span data-stu-id="469dc-132">Construct the message body</span></span>

<span data-ttu-id="469dc-133">定义页面内容的 HTML 被称为 *输入 HTML*。</span><span class="sxs-lookup"><span data-stu-id="469dc-133">The HTML that defines page content is called *input HTML*.</span></span> <span data-ttu-id="469dc-134">输入 HTML 支持[标准 HTML 和 CSS 子集](#supported-html-and-css-for-onenote-pages)，并增添了自定义属性。</span><span class="sxs-lookup"><span data-stu-id="469dc-134">Input HTML supports a [subset of standard HTML and CSS](#supported-html-and-css-for-onenote-pages), with the addition of custom attributes.</span></span> <span data-ttu-id="469dc-135">（**data-id** 和 **data-render-src** 等自定义属性在 [输入和输出 HTML](onenote-input-output-html.md) 中进行了说明。）</span><span class="sxs-lookup"><span data-stu-id="469dc-135">(Custom attributes, like **data-id** and **data-render-src**, are described in [Input and output HTML](onenote-input-output-html.md).)</span></span> 

<span data-ttu-id="469dc-136">在 POST 请求的邮件正文中发送输入 HTML。</span><span class="sxs-lookup"><span data-stu-id="469dc-136">Send the input HTML in the message body of the POST request.</span></span> <span data-ttu-id="469dc-137">你可以使用 `application/xhtml+xml` 或 `text/html` 内容类型直接在邮件正文中发送输入 HTML，也可以在多部分请求的“演示文稿”部件中发送它。</span><span class="sxs-lookup"><span data-stu-id="469dc-137">You can send the input HTML directly in the message body using the  `application/xhtml+xml` or `text/html` content type, or you can send it in the "Presentation" part of a multipart request.</span></span> 

<span data-ttu-id="469dc-138">以下示例直接在邮件正文中发送输入 HTML。</span><span class="sxs-lookup"><span data-stu-id="469dc-138">The following example sends the input HTML directly in the message body.</span></span>

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

<span data-ttu-id="469dc-139">如果要发送二进制数据，则必须使用[多部分请求](#example-request)。</span><span class="sxs-lookup"><span data-stu-id="469dc-139">If you're sending binary data, you must use a [multipart request](#example-request).</span></span> 

> <span data-ttu-id="469dc-140">**注意：** 为简化编程和应用的一致性，可以使用多部分请求来创建所有页面。</span><span class="sxs-lookup"><span data-stu-id="469dc-140">**Note:** To simplify programming and consistency in your app, you can use multipart requests to create all pages.</span></span> <span data-ttu-id="469dc-141">最好使用库来构造多部分邮件。</span><span class="sxs-lookup"><span data-stu-id="469dc-141">It's a good idea to use a library to construct multipart messages.</span></span> <span data-ttu-id="469dc-142">这样可减少创建格式不正确的有效负载的风险。</span><span class="sxs-lookup"><span data-stu-id="469dc-142">This reduces the risk of creating malformed payloads.</span></span>


<a name="input-html-rules"></a>

### <a name="requirements-and-limitations-for-input-html-in-post-pages-requests"></a><span data-ttu-id="469dc-143">POST 页面请求中有关输入 HTML 的要求和限制</span><span class="sxs-lookup"><span data-stu-id="469dc-143">Requirements and limitations for input HTML in POST pages requests</span></span>

<span data-ttu-id="469dc-144">发送输入 HTML 时，请注意这些常规要求和限制：</span><span class="sxs-lookup"><span data-stu-id="469dc-144">When sending input HTML, be aware of these general requirements and limitations:</span></span>  

- <span data-ttu-id="469dc-145">输入 HTML 应为 UTF-8 编码且格式标准的 XHTML。</span><span class="sxs-lookup"><span data-stu-id="469dc-145">Input HTML should be UTF-8 encoded and well-formed XHTML.</span></span> <span data-ttu-id="469dc-146">所有容器开始标记都要求匹配结束标记。</span><span class="sxs-lookup"><span data-stu-id="469dc-146">All container start tags require matching closing tags.</span></span> <span data-ttu-id="469dc-147">所有属性值必须使用双引号或单引号引住。</span><span class="sxs-lookup"><span data-stu-id="469dc-147">All attribute values must be surrounded by double- or single-quote marks.</span></span>  <!--docs say MUST be encoded-->

- <span data-ttu-id="469dc-148">JavaScript 代码、包含的文件和 CSS 会被删除。</span><span class="sxs-lookup"><span data-stu-id="469dc-148">JavaScript code, included files, and CSS are removed.</span></span> 

- <span data-ttu-id="469dc-149">HTML 表单将全部删除。</span><span class="sxs-lookup"><span data-stu-id="469dc-149">HTML forms are removed in their entirety.</span></span>  

- <span data-ttu-id="469dc-150">Microsoft Graph 支持 [HTML 元素的子集](#supported-html-and-css-for-onenote-pages)。</span><span class="sxs-lookup"><span data-stu-id="469dc-150">Microsoft Graph supports a [subset of HTML elements](#supported-html-and-css-for-onenote-pages).</span></span> 

- <span data-ttu-id="469dc-151">Microsoft Graph 支持常见 HTML 属性的子集和一组自定义属性，如用于更新页面的 **data-id** 属性。</span><span class="sxs-lookup"><span data-stu-id="469dc-151">Microsoft Graph supports a subset of common HTML attributes and a set of custom attributes, such as the **data-id** attribute used for updating pages.</span></span> <span data-ttu-id="469dc-152">有关受支持的属性，请参阅[输入和输出 HTML](onenote-input-output-html.md)。</span><span class="sxs-lookup"><span data-stu-id="469dc-152">For supported attributes, see [Input and output HTML](onenote-input-output-html.md).</span></span>


<a name="supported-html"></a>

### <a name="supported-html-and-css-for-onenote-pages"></a><span data-ttu-id="469dc-153">OneNote 页面受支持的 HTML 和 CSS</span><span class="sxs-lookup"><span data-stu-id="469dc-153">Supported HTML and CSS for OneNote pages</span></span>

<span data-ttu-id="469dc-154">并非所有元素、特性和属性都受支持（在 HTML4、XHTML、CSS、HTML5 等中）。</span><span class="sxs-lookup"><span data-stu-id="469dc-154">Not all elements, attributes, and properties are supported (in HTML4, XHTML, CSS, HTML5, etc.).</span></span> <span data-ttu-id="469dc-155">相反，Microsoft Graph 接受一组有限的 HTML，以更好地适应用户使用 OneNote 的方式。</span><span class="sxs-lookup"><span data-stu-id="469dc-155">Instead, Microsoft Graph accepts a limited set of HTML that better fits how people use OneNote.</span></span> <span data-ttu-id="469dc-156">有关详细信息，请参阅 [HTML 标记对页面的支持](https://dev.onenote.com/docs#/introduction/html-tag-support-for-pages)。</span><span class="sxs-lookup"><span data-stu-id="469dc-156">For more information, see [HTML tag support for pages](https://dev.onenote.com/docs#/introduction/html-tag-support-for-pages).</span></span> <span data-ttu-id="469dc-157">如果其中未列出标记，则可能被忽略。</span><span class="sxs-lookup"><span data-stu-id="469dc-157">If a tag's not listed there, it'll probably be ignored.</span></span>

<!--Microsoft Graph only accepts UTF-8 data. Be sure that all requests are encoded that way, and your content-type headers indicate that as well. xx our examples don't show this-->

<span data-ttu-id="469dc-158">以下列表显示 Microsoft Graph 支持的基本元素类型：</span><span class="sxs-lookup"><span data-stu-id="469dc-158">The following list shows the basic element types that Microsoft Graph supports:</span></span>

- <span data-ttu-id="469dc-159">`<head>` 和 `<body>`</span><span class="sxs-lookup"><span data-stu-id="469dc-159">`<head>` and `<body>`</span></span></p>
- <span data-ttu-id="469dc-160">`<title>` 和 `<meta>`，用于设置页面标题和创建日期</span><span class="sxs-lookup"><span data-stu-id="469dc-160">`<title>` and `<meta>` that set the page title and creation date</span></span></p>
- <span data-ttu-id="469dc-161">`<h1>` 至 `<h6>`，用于节标题</span><span class="sxs-lookup"><span data-stu-id="469dc-161">`<h1>` through `<h6>` for section headings</span></span></p>
- <span data-ttu-id="469dc-162">`<p>` 用于段落</span><span class="sxs-lookup"><span data-stu-id="469dc-162">`<p>` for paragraphs</span></span></p>
- <span data-ttu-id="469dc-163">`<ul>`、`<ol>` 和 `<li>`，用于列表和列表项</span><span class="sxs-lookup"><span data-stu-id="469dc-163">`<ul>`, `<ol>`, and `<li>` for lists and list items</span></span></p>
- <span data-ttu-id="469dc-164">`<table>`、`<tr>` 和 `<td>`，包括嵌套表</span><span class="sxs-lookup"><span data-stu-id="469dc-164">`<table>`, `<tr>` and `<td>`, including nested tables</span></span></p>
- <span data-ttu-id="469dc-165">`<pre>` 用于预设格式的文本（会保留空格和换行符）</span><span class="sxs-lookup"><span data-stu-id="469dc-165">`<pre>` for preformatted text (preserves white space and line breaks)</span></span></p>
- <span data-ttu-id="469dc-166">`<b>` 和 `<i>`，用于粗体和斜体字符样式</span><span class="sxs-lookup"><span data-stu-id="469dc-166">`<b>` and `<i>` for bold and italic character styles</span></span></p>

<span data-ttu-id="469dc-167">Microsoft Graph 在创建页面时会保留输入 HTML 的语义内容和基本结构，但会转换输入 HTML 以使用一组受支持的 HTML 和 CSS。</span><span class="sxs-lookup"><span data-stu-id="469dc-167">Microsoft Graph preserves the semantic content and basic structure of the input HTML when it creates pages, but it converts the input HTML to use the supported set of HTML and CSS.</span></span> <span data-ttu-id="469dc-168">OneNote 中不存在的功能没有任何内容可以转换，因此，它们可能无法在源 HTML 中识别。</span><span class="sxs-lookup"><span data-stu-id="469dc-168">Features that don't exist in OneNote have nothing to be translated to, so they might not be recognized in the source HTML.</span></span> 


<a name="example"></a>

## <a name="example-request"></a><span data-ttu-id="469dc-169">示例请求</span><span class="sxs-lookup"><span data-stu-id="469dc-169">Example request</span></span>

<span data-ttu-id="469dc-170">这个多部分请求示例创建了一个包含图像和嵌入式文件的页面。</span><span class="sxs-lookup"><span data-stu-id="469dc-170">This example multipart request creates a page that contains images and an embedded file.</span></span> <span data-ttu-id="469dc-171">必需的 **演示** 部分包含定义页面的输入 HTML。</span><span class="sxs-lookup"><span data-stu-id="469dc-171">The required **Presentation** part contains the input HTML that defines the page.</span></span> <span data-ttu-id="469dc-172">**ImageBlock1** 部分包含二进制图像数据，**fileBlock1** 包含二进制文件数据。</span><span class="sxs-lookup"><span data-stu-id="469dc-172">The **imageBlock1** part contains the binary image data, and **fileBlock1** contains the binary file data.</span></span> <span data-ttu-id="469dc-173">数据部分也可包含 HTML，其中 Microsoft Graph 在 OneNote 页面上[将 HTML 呈现为一个图像](onenote-images-files.md#add-an-image-using-binary-data)。</span><span class="sxs-lookup"><span data-stu-id="469dc-173">Data parts can also contain HTML, in which case Microsoft Graph [renders the HTML as an image](onenote-images-files.md#add-an-image-using-binary-data) on the OneNote page.</span></span> 

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

<span data-ttu-id="469dc-174">有关介绍如何创建包含图像和其他文件的页面的更多示例，请参阅[添加图像和文件](onenote-images-files.md)、我们的[教程](/previous-versions/office/office-365-api/how-to/onenote-tutorial)及[示例](https://github.com/onenotedev)。</span><span class="sxs-lookup"><span data-stu-id="469dc-174">For more examples that show how to create pages that contain images and other files, see [Add images and files](onenote-images-files.md), our [tutorials](/previous-versions/office/office-365-api/how-to/onenote-tutorial), and our [samples](https://github.com/onenotedev).</span></span> <span data-ttu-id="469dc-175">此外，了解如何针对名片捕获、线上食谱和产品列表[创建绝对定位元素](onenote-abs-pos.md)、[使用笔记标记](onenote-note-tags.md)和[提取数据](onenote-extract-data.md)。</span><span class="sxs-lookup"><span data-stu-id="469dc-175">Also, learn how to [create absolute positioned elements](onenote-abs-pos.md), [use note tags](onenote-note-tags.md), and [extract data](onenote-extract-data.md) for business card captures and online recipe and product listings.</span></span>

<span data-ttu-id="469dc-176">Microsoft Graph 对某些格式非常严格，如多部分邮件正文中的 CRLF 换行符。</span><span class="sxs-lookup"><span data-stu-id="469dc-176">Microsoft Graph is strict about some formats, such as CRLF newlines in a multipart message body.</span></span> <span data-ttu-id="469dc-177">为降低创造格式不正确的有效负载的风险，应使用库来构造多部分消息。</span><span class="sxs-lookup"><span data-stu-id="469dc-177">To reduce the risk of creating malformed payloads, you should use a library to construct multipart messages.</span></span> 

<span data-ttu-id="469dc-178">如果收到格式不正确有效负载的 400 状态，请检查换行符和空格的格式，并检查编码问题。</span><span class="sxs-lookup"><span data-stu-id="469dc-178">If you do receive a 400 status for a malformed payload, check the formatting of newlines and whitespaces, and check for encoding issues.</span></span> <span data-ttu-id="469dc-179">例如，请尝试使用 `charset=utf-8`（示例：`Content-Type: text/html; charset=utf-8`）。</span><span class="sxs-lookup"><span data-stu-id="469dc-179">For example, try using `charset=utf-8` (example: `Content-Type: text/html; charset=utf-8`).</span></span>

<span data-ttu-id="469dc-180">请参阅[输入 HTML 的要求和限制](#requirements-and-limitations-for-input-html-in-post-pages-requests)，以及 [POST 请求的大小限制](onenote-images-files.md#size-limitations-for-post-pages-requests)。</span><span class="sxs-lookup"><span data-stu-id="469dc-180">See [requirements and limitations for input HTML](#requirements-and-limitations-for-input-html-in-post-pages-requests) and [size limits for POST requests](onenote-images-files.md#size-limitations-for-post-pages-requests).</span></span>


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-post-pages-requests"></a><span data-ttu-id="469dc-181">*POST 页面* 请求的请求和响应信息</span><span class="sxs-lookup"><span data-stu-id="469dc-181">Request and response information for *POST pages* requests</span></span>

| <span data-ttu-id="469dc-182">请求数据</span><span class="sxs-lookup"><span data-stu-id="469dc-182">Request data</span></span> | <span data-ttu-id="469dc-183">说明</span><span class="sxs-lookup"><span data-stu-id="469dc-183">Description</span></span> |  
|------|------|  
| <span data-ttu-id="469dc-184">协议</span><span class="sxs-lookup"><span data-stu-id="469dc-184">Protocol</span></span> | <span data-ttu-id="469dc-185">所有请求均使用 SSL/TLS HTTPS 协议。</span><span class="sxs-lookup"><span data-stu-id="469dc-185">All requests use the SSL/TLS HTTPS protocol.</span></span> |  
| <span data-ttu-id="469dc-186">授权标头</span><span class="sxs-lookup"><span data-stu-id="469dc-186">Authorization header</span></span> | <p><span data-ttu-id="469dc-187">`Bearer {token}`，其中 `{token}` 是已注册应用的一个有效 OAuth 2.0 访问令牌。</span><span class="sxs-lookup"><span data-stu-id="469dc-187">`Bearer {token}`, where `{token}` is a valid OAuth 2.0 access token for your registered app.</span></span></p><p><span data-ttu-id="469dc-188">如果缺少或无效，则请求失败，并显示 401 状态代码。</span><span class="sxs-lookup"><span data-stu-id="469dc-188">If missing or invalid, the request fails with a 401 status code.</span></span> <span data-ttu-id="469dc-189">请参阅[身份验证和权限](permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="469dc-189">See [Authentication and permissions](permissions-reference.md).</span></span></p> |  
| <span data-ttu-id="469dc-190">Content-Type 标头</span><span class="sxs-lookup"><span data-stu-id="469dc-190">Content-Type header</span></span> | <p><span data-ttu-id="469dc-191">HTML 内容的 `text/html` 或 `application/xhtml+xml`，确定是直接在邮件正文中发送还是在多部分请求的“演示”部分中发送。</span><span class="sxs-lookup"><span data-stu-id="469dc-191">`text/html` or `application/xhtml+xml` for the HTML content, whether it's sent directly in the message body or in the required "Presentation" part of multipart requests.</span></span></p><p><span data-ttu-id="469dc-192">发送二进制数据时，多部分请求是必需的，并使用 `multipart/form-data; boundary=part-boundary` 内容类型，其中 `{part-boundary}` 是一个字符串，表示每个数据部件的开始和结束。</span><span class="sxs-lookup"><span data-stu-id="469dc-192">Multipart requests are required when sending binary data, and use the `multipart/form-data; boundary=part-boundary` content type, where `{part-boundary}` is a string that signals the start and end of each data part.</span></span></p> |  
| <span data-ttu-id="469dc-193">接受标头</span><span class="sxs-lookup"><span data-stu-id="469dc-193">Accept header</span></span> | `application/json` | 

<br/>

| <span data-ttu-id="469dc-194">响应数据</span><span class="sxs-lookup"><span data-stu-id="469dc-194">Response data</span></span> | <span data-ttu-id="469dc-195">说明</span><span class="sxs-lookup"><span data-stu-id="469dc-195">Description</span></span> |  
|------|------|  
| <span data-ttu-id="469dc-196">成功代码</span><span class="sxs-lookup"><span data-stu-id="469dc-196">Success code</span></span> | <span data-ttu-id="469dc-197">201 HTTP 状态代码。</span><span class="sxs-lookup"><span data-stu-id="469dc-197">A 201 HTTP status code.</span></span> |  
| <span data-ttu-id="469dc-198">响应正文</span><span class="sxs-lookup"><span data-stu-id="469dc-198">Response body</span></span> | <span data-ttu-id="469dc-199">采用 JSON 格式的新页的 OData 表示形式。</span><span class="sxs-lookup"><span data-stu-id="469dc-199">A OData representation of the new page in JSON format.</span></span> |  
| <span data-ttu-id="469dc-200">错误</span><span class="sxs-lookup"><span data-stu-id="469dc-200">Errors</span></span> | <span data-ttu-id="469dc-201">如果请求失败，API 将在响应正文的 **\@api.diagnostics** 对象中返回错误。</span><span class="sxs-lookup"><span data-stu-id="469dc-201">If the request fails, the API returns errors in the **\@api.diagnostics** object in the response body.</span></span> |  
| <span data-ttu-id="469dc-202">位置标头</span><span class="sxs-lookup"><span data-stu-id="469dc-202">Location header</span></span> | <span data-ttu-id="469dc-203">新页的资源 URL。</span><span class="sxs-lookup"><span data-stu-id="469dc-203">The resource URL for the new page.</span></span> |  
| <span data-ttu-id="469dc-204">X-CorrelationId 标头</span><span class="sxs-lookup"><span data-stu-id="469dc-204">X-CorrelationId header</span></span> | <span data-ttu-id="469dc-205">唯一标识该请求的 GUID。</span><span class="sxs-lookup"><span data-stu-id="469dc-205">A GUID that uniquely identifies the request.</span></span> <span data-ttu-id="469dc-206">在与 Microsoft 支持部门协作来解决问题时，可以使用此值和日期标头值。</span><span class="sxs-lookup"><span data-stu-id="469dc-206">You can use this value along with the value of the Date header when working with Microsoft support to troubleshoot issues.</span></span> |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a><span data-ttu-id="469dc-207">构建 Microsoft Graph 服务根 URL</span><span class="sxs-lookup"><span data-stu-id="469dc-207">Constructing the Microsoft Graph service root URL</span></span>

<span data-ttu-id="469dc-208">Microsoft Graph 服务根 URL 为 Microsoft Graph 的所有调用使用以下格式：</span><span class="sxs-lookup"><span data-stu-id="469dc-208">The Microsoft Graph service root URL uses the following format for all calls to Microsoft Graph:</span></span>

`https://graph.microsoft.com/{version}/me/onenote/`  

<span data-ttu-id="469dc-209">URL 中的 `version` 段表示想要使用的 Microsoft Graph 的版本。</span><span class="sxs-lookup"><span data-stu-id="469dc-209">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span> <span data-ttu-id="469dc-210">`v1.0` 用于稳定的生产代码。</span><span class="sxs-lookup"><span data-stu-id="469dc-210">Use `v1.0` for stable production code.</span></span> <span data-ttu-id="469dc-211">`beta` 用于试用正在开发的功能。</span><span class="sxs-lookup"><span data-stu-id="469dc-211">Use `beta` to try out a feature that's in development.</span></span> <span data-ttu-id="469dc-212">Beta 版中的特性和功能可能会有所更改，因此，不应将其用于生产代码。</span><span class="sxs-lookup"><span data-stu-id="469dc-212">Features and functionality in beta may change, so you shouldn't use it in your production code.</span></span> 

<span data-ttu-id="469dc-213">为当前用户可以访问的 OneNote 内容（拥有和共享）使用 `me`。</span><span class="sxs-lookup"><span data-stu-id="469dc-213">Use `me` for OneNote content that the current user can access (owned and shared).</span></span> <span data-ttu-id="469dc-214">为指定用户已与当前用户共享的 OneNote 内容（此 URL 中）使用 `users/{id}`。</span><span class="sxs-lookup"><span data-stu-id="469dc-214">Use `users/{id}` for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="469dc-215">使用 [Microsoft Graph](https://graph.microsoft.com/v1.0/users) 获取用户 ID。</span><span class="sxs-lookup"><span data-stu-id="469dc-215">Use [Microsoft Graph](https://graph.microsoft.com/v1.0/users) to get user IDs.</span></span> 

<a name="limitations"></a>

## <a name="onenote-section-size-limitations"></a><span data-ttu-id="469dc-216">OneNote 分区大小限制</span><span class="sxs-lookup"><span data-stu-id="469dc-216">OneNote section size limitations</span></span>
<span data-ttu-id="469dc-217">对可使用 OneNote API 添加到分区的页面数量有一些限制。</span><span class="sxs-lookup"><span data-stu-id="469dc-217">There is a limit to the number of pages that you can add to a section using the OneNote API.</span></span> <span data-ttu-id="469dc-218">当某个分区达到此限制并尝试在该分区中创建新页面时，你将看到 HTTP 状态代码为 `507` 的响应，并显示消息“已超出每个分区允许的最大页面数”。</span><span class="sxs-lookup"><span data-stu-id="469dc-218">When this limit is reached for a section and an attempt is made to create a new page in that section, you will see a response with HTTP status code `507` and message "Exceeded the maximum number of pages allowed per section".</span></span> <span data-ttu-id="469dc-219">有关此错误代码的详细信息，请参阅 [OneNote 错误代码](onenote-error-codes.md)。</span><span class="sxs-lookup"><span data-stu-id="469dc-219">For more information about this error code, see [OneNote error codes](onenote-error-codes.md).</span></span>

<span data-ttu-id="469dc-220">可以使用下列解决办法之一：</span><span class="sxs-lookup"><span data-stu-id="469dc-220">You can use one of the following workarounds:</span></span>
- <span data-ttu-id="469dc-221">创建新分区并从中添加新页面。</span><span class="sxs-lookup"><span data-stu-id="469dc-221">Create a new section and add new pages there.</span></span>
- <span data-ttu-id="469dc-222">删除已达到页面限制的现有分区的未使用页面。</span><span class="sxs-lookup"><span data-stu-id="469dc-222">Delete unused pages of an existing section that has reached the page limit.</span></span>

<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="469dc-223">权限</span><span class="sxs-lookup"><span data-stu-id="469dc-223">Permissions</span></span>

<span data-ttu-id="469dc-224">若要创建 OneNote 页面，需要请求相应的权限。</span><span class="sxs-lookup"><span data-stu-id="469dc-224">To create OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="469dc-225">选择应用运行所需的最低级别的权限。</span><span class="sxs-lookup"><span data-stu-id="469dc-225">Choose the lowest level of permissions that your app needs to do its work.</span></span>

<span data-ttu-id="469dc-226">从以下项中进行选择：</span><span class="sxs-lookup"><span data-stu-id="469dc-226">Choose from:</span></span>

- <span data-ttu-id="469dc-227">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="469dc-227">Notes.Create</span></span>
- <span data-ttu-id="469dc-228">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="469dc-228">Notes.ReadWrite</span></span>
- <span data-ttu-id="469dc-229">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="469dc-229">Notes.ReadWrite.All</span></span>

<span data-ttu-id="469dc-230">有关权限范围及其工作方式的详细信息，请参阅 [Microsoft Graph 权限引用](permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="469dc-230">For more information about permission scopes and how they work, see [Microsoft Graph permissions reference](permissions-reference.md).</span></span>




<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="469dc-231">另请参阅</span><span class="sxs-lookup"><span data-stu-id="469dc-231">See also</span></span>

- [<span data-ttu-id="469dc-232">添加图像和文件</span><span class="sxs-lookup"><span data-stu-id="469dc-232">Add images and files</span></span>](onenote-images-files.md)
- [<span data-ttu-id="469dc-233">创建绝对定位的元素</span><span class="sxs-lookup"><span data-stu-id="469dc-233">Create absolute positioned elements</span></span>](onenote-abs-pos.md)  
- [<span data-ttu-id="469dc-234">提取数据</span><span class="sxs-lookup"><span data-stu-id="469dc-234">Extract data</span></span>](onenote-extract-data.md)
- [<span data-ttu-id="469dc-235">使用笔记标记</span><span class="sxs-lookup"><span data-stu-id="469dc-235">Use note tags</span></span>](onenote-note-tags.md)
- [<span data-ttu-id="469dc-236">与 OneNote 集成</span><span class="sxs-lookup"><span data-stu-id="469dc-236">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="469dc-237">OneNote 开发者博客</span><span class="sxs-lookup"><span data-stu-id="469dc-237">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="469dc-238">Microsoft Q&A 上的 OneNote 开发问题</span><span class="sxs-lookup"><span data-stu-id="469dc-238">OneNote development questions on Microsoft Q&A</span></span>](/answers/topics/microsoft-graph-notes.html)
- [<span data-ttu-id="469dc-239">OneNote GitHub 存储库</span><span class="sxs-lookup"><span data-stu-id="469dc-239">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)