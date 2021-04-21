---
title: 将图像、视频和文件添加到 OneNote 页面
description: " Microsoft 365 中的企业笔记本"
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: 3a3f8b969fba5842f8c2f7b7a0f253a6f6f65282
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921642"
---
# <a name="add-images-videos-and-files-to-onenote-pages"></a><span data-ttu-id="268d6-103">将图像、视频和文件添加到 OneNote 页面</span><span class="sxs-lookup"><span data-stu-id="268d6-103">Add images, videos, and files to OneNote pages</span></span>

<span data-ttu-id="268d6-104">**适用于** OneDrive 上的消费者笔记本 | Microsoft 365 上的企业级笔记本</span><span class="sxs-lookup"><span data-stu-id="268d6-104">**Applies to** Consumer notebooks on OneDrive | Enterprise notebooks on Microsoft 365</span></span>

<span data-ttu-id="268d6-105">在 [创建](onenote-create-page.md)或 [更新](onenote-update-page.md)页面时，可以使用 **img**、**object** 和 **iframe** 元素将图像、视频和文件添加到 OneNote 页面。</span><span class="sxs-lookup"><span data-stu-id="268d6-105">You can use **img**, **object**, and **iframe** elements to add images, videos, and files to a OneNote page when you're [creating](onenote-create-page.md) or [updating](onenote-update-page.md) the page.</span></span> 

- <span data-ttu-id="268d6-106">使用 **img** 在页面上呈现图像。</span><span class="sxs-lookup"><span data-stu-id="268d6-106">Use **img** to render an image on the page.</span></span>
- <span data-ttu-id="268d6-107">使用 **iframe** 在页面上嵌入视频。</span><span class="sxs-lookup"><span data-stu-id="268d6-107">Use **iframe** to embed a video on the page.</span></span>
- <span data-ttu-id="268d6-108">使用 **object** 将文件附件添加到页面。</span><span class="sxs-lookup"><span data-stu-id="268d6-108">Use **object** to add a file attachment to the page.</span></span>


<a name="images"></a>

## <a name="adding-images"></a><span data-ttu-id="268d6-109">添加图像</span><span class="sxs-lookup"><span data-stu-id="268d6-109">Adding images</span></span>

<span data-ttu-id="268d6-110">图像可以通过 URL 引用或发送原始数据来进行添加。</span><span class="sxs-lookup"><span data-stu-id="268d6-110">Images can be added by URL reference or by sending raw data.</span></span> <span data-ttu-id="268d6-111">Microsoft Graph 支持以下可将图像、徽标和照片添加到 OneNote 页面的方法。</span><span class="sxs-lookup"><span data-stu-id="268d6-111">Microsoft Graph supports the following methods of adding images, logos, and photos to OneNote pages.</span></span> 

[<span data-ttu-id="268d6-112">从 Web 添加公共图像</span><span class="sxs-lookup"><span data-stu-id="268d6-112">Add a public image from the web</span></span>](#add-a-public-image-from-the-web)

<span data-ttu-id="268d6-113">将 `img` 与 `src="https://image-url"` 结合使用，并指定可公开访问图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="268d6-113">Use `img` with `src="https://image-url"` and specify the URL of a publicly accessible image.</span></span> <span data-ttu-id="268d6-114">在 OneNote 页面上呈现图像。</span><span class="sxs-lookup"><span data-stu-id="268d6-114">Renders the image on the OneNote page.</span></span>

[<span data-ttu-id="268d6-115">使用二进制数据添加图像</span><span class="sxs-lookup"><span data-stu-id="268d6-115">Add an image using binary data</span></span>](#add-an-image-using-binary-data)

<span data-ttu-id="268d6-116">将 `img` 与 `src="name:image-block-name"` 结合使用，并发送多部分请求的数据部件中的图像文件。</span><span class="sxs-lookup"><span data-stu-id="268d6-116">Use `img` with `src="name:image-block-name"` and send the image file in a data part of a multipart request.</span></span> <span data-ttu-id="268d6-117">在 OneNote 页面上呈现图像。</span><span class="sxs-lookup"><span data-stu-id="268d6-117">Renders the image on the OneNote page.</span></span>

[<span data-ttu-id="268d6-118">添加网页快照</span><span class="sxs-lookup"><span data-stu-id="268d6-118">Add a webpage snapshot</span></span>](#add-a-webpage-snapshot)

<span data-ttu-id="268d6-119">将 `img` 与 `data-render-src="https://webpage-url"` 结合使用，并指定网页的 URL。</span><span class="sxs-lookup"><span data-stu-id="268d6-119">Use `img` with `data-render-src="https://webpage-url"` and specify the URL of a webpage.</span></span> <span data-ttu-id="268d6-120">在 OneNote 页面上呈现整个网页的快照。</span><span class="sxs-lookup"><span data-stu-id="268d6-120">Renders a snapshot of the whole webpage on the OneNote page.</span></span>

[<span data-ttu-id="268d6-121">添加从 HTML 呈现的图像</span><span class="sxs-lookup"><span data-stu-id="268d6-121">Add an image rendered from HTML</span></span>](#add-an-image-rendered-from-html)

<span data-ttu-id="268d6-122">将 `img` 与 `data-render-src="name:html-block-name"` 结合使用，并发送多部分请求的数据部件中的 HTML。</span><span class="sxs-lookup"><span data-stu-id="268d6-122">Use `img` with `data-render-src="name:html-block-name"` and send HTML in the data part of a multipart request.</span></span> <span data-ttu-id="268d6-123">在 OneNote 页面上将 HTML 呈现为图像。</span><span class="sxs-lookup"><span data-stu-id="268d6-123">Renders the HTML as an image on the OneNote page.</span></span>

[<span data-ttu-id="268d6-124">添加 PDF 文件内容的图像</span><span class="sxs-lookup"><span data-stu-id="268d6-124">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)

<span data-ttu-id="268d6-125">使用 `<img data-render-src="name:part-name" />`，并发送多部分请求的数据部件中的 PDF 文件。</span><span class="sxs-lookup"><span data-stu-id="268d6-125">Use `<img data-render-src="name:part-name" />` and send the PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="268d6-126">在 OneNote 页面上将每个 PDF 页面呈现为单独图像。</span><span class="sxs-lookup"><span data-stu-id="268d6-126">Renders each PDF page as a separate image on the OneNote page.</span></span>

[<span data-ttu-id="268d6-127">将图像文件添加为文件附件</span><span class="sxs-lookup"><span data-stu-id="268d6-127">Add an image file as a file attachment</span></span>](#add-an-image-file-as-an-attachment)

<span data-ttu-id="268d6-128">将 `object` 与 `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` 结合使用，并发送多部分请求的数据部件中的图像文件。</span><span class="sxs-lookup"><span data-stu-id="268d6-128">Use `object` with `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` and send an image file in the data part of a multipart request.</span></span> <span data-ttu-id="268d6-129">将文件附件添加到 OneNote 页面，并显示文件图标。</span><span class="sxs-lookup"><span data-stu-id="268d6-129">Adds a file attachment to the OneNote page and displays a file icon.</span></span>


> <span data-ttu-id="268d6-130">**注意：** 若要获取 OneNote 页面上的图像，首先发送 [GET 请求获取页面内容](onenote-get-content.md#page-html-content)。</span><span class="sxs-lookup"><span data-stu-id="268d6-130">**Note:** To get images on a OneNote page, first send a [GET request for the page content](onenote-get-content.md#page-html-content).</span></span> <span data-ttu-id="268d6-131">这会将 URL 返回到页面上的图像资源。</span><span class="sxs-lookup"><span data-stu-id="268d6-131">This returns the URLs to the image resources on the page.</span></span> <span data-ttu-id="268d6-132">然后，将 [GET 请求与图像资源分开](onenote-get-content.md#image-or-other-file-resource)。</span><span class="sxs-lookup"><span data-stu-id="268d6-132">You then separate [GET requests to the image resources](onenote-get-content.md#image-or-other-file-resource).</span></span>


#### <a name="image-attributes"></a><span data-ttu-id="268d6-133">图像属性</span><span class="sxs-lookup"><span data-stu-id="268d6-133">Image attributes</span></span> 

<span data-ttu-id="268d6-134">**img** 元素可以选择包括 **alt**、**height** 和 **width** 属性，以及样式属性 **max-width** 和 **max-height**。</span><span class="sxs-lookup"><span data-stu-id="268d6-134">An **img** element can optionally include **alt**, **height**, and **width** attributes, and the style attributes **max-width** and **max-height**.</span></span>

#### <a name="image-media-types"></a><span data-ttu-id="268d6-135">图像媒体类型</span><span class="sxs-lookup"><span data-stu-id="268d6-135">Image media types</span></span>

<span data-ttu-id="268d6-136">Microsoft Graph 支持 TIFF、PNG、GIF、JPEG 和 BMP 图像类型。</span><span class="sxs-lookup"><span data-stu-id="268d6-136">Microsoft Graph supports TIFF, PNG, GIF, JPEG, and BMP image types.</span></span> <span data-ttu-id="268d6-137">若要捕获使用不想转换的其他格式的图像，请在多部分请求中[发送二进制数据](#add-an-image-using-binary-data)。</span><span class="sxs-lookup"><span data-stu-id="268d6-137">To capture an image that uses a different format that you don't want to convert, [send the binary data](#add-an-image-using-binary-data) in a multipart request.</span></span> <span data-ttu-id="268d6-138">不需要使用 Base64，或其他方式对发送的二进制数据进行编码。</span><span class="sxs-lookup"><span data-stu-id="268d6-138">You don't need to use Base64 or otherwise encode the binary data that you send.</span></span>

> <span data-ttu-id="268d6-139">**注意：** API 会检测原始输入图像类型，并在 [输出 HTML](onenote-input-output-html.md#output-html) 中将其作为 **data-fullres-src-type** 属性返回。</span><span class="sxs-lookup"><span data-stu-id="268d6-139">**Note:** The API detects the original input image type, and returns it as the **data-fullres-src-type** attribute in the [output HTML](onenote-input-output-html.md#output-html).</span></span> <span data-ttu-id="268d6-140">此外，API 还会在 **data-src-type** 中返回优化图像的图像类型。</span><span class="sxs-lookup"><span data-stu-id="268d6-140">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 
<span data-ttu-id="268d6-141">请参阅创建包含媒体的页面时应用的[限制](#size-limitations-for-post-pages-requests)。</span><span class="sxs-lookup"><span data-stu-id="268d6-141">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="image-img-url-src"></a>

### <a name="add-a-public-image-from-the-web"></a><span data-ttu-id="268d6-142">从 Web 添加公共图像</span><span class="sxs-lookup"><span data-stu-id="268d6-142">Add a public image from the web</span></span>

<span data-ttu-id="268d6-143">在请求的输入 HTML 中，包括 `<img src="https://..." />` 并为 **src** 属性指定可公开访问图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="268d6-143">In the input HTML of your request, include `<img src="https://..." />` and specify the URL of a publicly accessible image for the **src** attribute.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Public URL</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays an image from the web.</p>
    <img src="https://..." width="300"/>
  </body>
</html>

--MyAppPartBoundary--  
```

<a name="image-img-binary-src"></a>

### <a name="add-an-image-using-binary-data"></a><span data-ttu-id="268d6-144">使用二进制数据添加图像</span><span class="sxs-lookup"><span data-stu-id="268d6-144">Add an image using binary data</span></span>

<span data-ttu-id="268d6-145">在请求的 **演示** 部分的输入 HTML 中，包括 `<img src="name:part-name" />`，其中 *part-name* 是包含二进制图像数据的 [多部分请求](onenote-create-page.md#example-request)中数据部分的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="268d6-145">In the input HTML of your request's **Presentation** part, include `<img src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="268d6-146">请只发送二进制数据，不要使用 Base64 或其他方式对其进行编码。</span><span class="sxs-lookup"><span data-stu-id="268d6-146">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Image binary data</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays the uploaded image.</p>
    <img src="name:image-block-name" alt="a cool image" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="MyAppPictureId"
Content-Type: image/jpeg

... image binary data ...

--MyAppPartBoundary--  
```


<a name="image-img-url-data-render-src"></a>

### <a name="add-a-webpage-snapshot"></a><span data-ttu-id="268d6-147">添加网页快照</span><span class="sxs-lookup"><span data-stu-id="268d6-147">Add a webpage snapshot</span></span>

<span data-ttu-id="268d6-148">可以使用 Microsoft Graph 截取整个网页的快照，并将其插入到新页面中。</span><span class="sxs-lookup"><span data-stu-id="268d6-148">You can use Microsoft Graph to snapshot entire webpages and insert them into new pages.</span></span> <span data-ttu-id="268d6-149">此方法对存档网页或捕获具有 OneNote 不支持的功能（如某些 CSS）的复杂网页很有用。</span><span class="sxs-lookup"><span data-stu-id="268d6-149">This method is useful to archive webpages or capture complex webpages that have features that OneNote doesn't support (like some CSS).</span></span>  

<span data-ttu-id="268d6-150">在请求的输入 HTML 中，包括 `<img src="https://..." />` 并指定要为 **src** 属性插入的网页的 URL。</span><span class="sxs-lookup"><span data-stu-id="268d6-150">In the input HTML of your request, include `<img src="https://..." />` and specify the URL of the webpage you want to insert for the **src** attribute.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Webpage capture</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays an image of the webpage.</p>
    <img data-render-src="https://www.onenote.com" width="200"/>
  </body>
</html>

--MyAppPartBoundary--  
```


<a name="image-img-binary-data-render-src"></a>

### <a name="add-an-image-rendered-from-html"></a><span data-ttu-id="268d6-151">添加从 HTML 呈现的图像</span><span class="sxs-lookup"><span data-stu-id="268d6-151">Add an image rendered from HTML</span></span>

<span data-ttu-id="268d6-152">将 HTML 作为数据块传递时，请确保没有需要用户凭据或预加载浏览器插件的活动内容。</span><span class="sxs-lookup"><span data-stu-id="268d6-152">When you pass the HTML as a data-block, be sure there is no active content that would require user credentials, or a pre-loaded browser plug-in.</span></span> <span data-ttu-id="268d6-153">Microsoft Graph 用于将 HTML 页面呈现为图像的引擎无法登录用户，且不包含诸如 Adobe Flash、Apple QuickTime 等插件。</span><span class="sxs-lookup"><span data-stu-id="268d6-153">The engine that Microsoft Graph uses to render the HTML page into an image has no ability to log in a user, and doesn't include plug-ins like Adobe Flash, Apple QuickTime, and so on.</span></span> <span data-ttu-id="268d6-154">这也意味着，如果获取数据需要用户登录凭据或 Cookie，将不会显示动态加载的内容（如可能带有 AJAX 脚本）。</span><span class="sxs-lookup"><span data-stu-id="268d6-154">That also means that dynamically-loaded content, such as might come with an AJAX script, won't appear if getting the data requires user login credentials or cookies.</span></span>

<span data-ttu-id="268d6-155">在请求的 **演示** 部分的输入 HTML 中，包括 `<img data-render-src="name:part-name" />`，其中 *part-name* 是包含 HTML 的 [多部分请求](onenote-create-page.md#example-request)中数据部分的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="268d6-155">In the input HTML of your request's **Presentation** part, include `<img data-render-src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the HTML.</span></span>


```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: HTML block</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page displays the block of HTML as an image.</p>
    <img data-render-src="name:html-block-name" alt="a cool image" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="html-block-name"
Content-Type: text/html

<html>
<body>
<h1>This HTML will render as an image</h1>
<p><b>Don't</b> try to embed another <i>data-render-src</i> type-image inside the HTML part--
it won't work. Instead, use URL-based real images like this:</p>
<img src="https://cdn.onenote.net/1664161560_Images/OneNote.ico" />
</body>
</html>

--MyAppPartBoundary--  
```


<a name="image-object"></a>

### <a name="add-an-image-file-as-an-attachment"></a><span data-ttu-id="268d6-156">将图像文件添加为附件</span><span class="sxs-lookup"><span data-stu-id="268d6-156">Add an image file as an attachment</span></span>

<span data-ttu-id="268d6-157">在请求的 **演示** 部分的输入 HTML 中，包括 `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`，其中 *part-name* 是包含二进制图像数据的 [多部分请求](onenote-create-page.md#example-request)中数据部分的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="268d6-157">In the input HTML of your request's **Presentation** part, include `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="268d6-158">请只发送二进制数据，不要使用 Base64 或其他方式对其进行编码。</span><span class="sxs-lookup"><span data-stu-id="268d6-158">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image: Binary image data as file attachment</title>
    <meta name="created" value="2015-11-11T12:45:00.000-8:00"/>
  </head>
  <body>
    <p>This page contains the image as a file attachment.</p>
    <object data-attachment="image-file.jpg" data="name:image-block-name" type="image/jpeg" />
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="logo1-file"
Content-Type: image/jpeg

... binary file data ...

--MyAppPartBoundary--
```

<span data-ttu-id="268d6-159">了解有关[文件媒体类型](#file-media-types)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="268d6-159">Learn more about [file media types](#file-media-types).</span></span>



<a name="adding-videos"></a>

## <a name="adding-videos"></a><span data-ttu-id="268d6-160">添加视频</span><span class="sxs-lookup"><span data-stu-id="268d6-160">Adding videos</span></span>

<span data-ttu-id="268d6-161">可以在输入 HTML 中使用 `<iframe data-original-src="https://..." />` 在 OneNote 页面中嵌入视频。</span><span class="sxs-lookup"><span data-stu-id="268d6-161">You can embed videos in OneNote pages using `<iframe data-original-src="https://..." />` in the input HTML.</span></span> 

### <a name="supported-video-sites"></a><span data-ttu-id="268d6-162">支持的视频网站</span><span class="sxs-lookup"><span data-stu-id="268d6-162">Supported video sites</span></span>

- <span data-ttu-id="268d6-163">Dailymotion</span><span class="sxs-lookup"><span data-stu-id="268d6-163">Dailymotion</span></span>
- <span data-ttu-id="268d6-164">Office Mix</span><span class="sxs-lookup"><span data-stu-id="268d6-164">Office Mix</span></span>
- <span data-ttu-id="268d6-165">Sway</span><span class="sxs-lookup"><span data-stu-id="268d6-165">Sway</span></span>
- <span data-ttu-id="268d6-166">Sketchfab</span><span class="sxs-lookup"><span data-stu-id="268d6-166">Sketchfab</span></span>
- <span data-ttu-id="268d6-167">TED</span><span class="sxs-lookup"><span data-stu-id="268d6-167">TED</span></span>
- <span data-ttu-id="268d6-168">YouTube</span><span class="sxs-lookup"><span data-stu-id="268d6-168">YouTube</span></span>
- <span data-ttu-id="268d6-169">Vimeo</span><span class="sxs-lookup"><span data-stu-id="268d6-169">Vimeo</span></span>
- <span data-ttu-id="268d6-170">Vine</span><span class="sxs-lookup"><span data-stu-id="268d6-170">Vine</span></span>

### <a name="iframe-attributes"></a><span data-ttu-id="268d6-171">iframe 属性</span><span class="sxs-lookup"><span data-stu-id="268d6-171">iframe attributes</span></span>

#### <a name="data-original-src"></a><span data-ttu-id="268d6-172">data-original-src</span><span class="sxs-lookup"><span data-stu-id="268d6-172">data-original-src</span></span>

<span data-ttu-id="268d6-173">必需。</span><span class="sxs-lookup"><span data-stu-id="268d6-173">Required.</span></span> <span data-ttu-id="268d6-174">视频的 URL。</span><span class="sxs-lookup"><span data-stu-id="268d6-174">The URL of the video.</span></span>

<span data-ttu-id="268d6-175">示例：`data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="268d6-175">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span>

#### <a name="width"></a><span data-ttu-id="268d6-176">width</span><span class="sxs-lookup"><span data-stu-id="268d6-176">width</span></span>

<span data-ttu-id="268d6-177">可选。</span><span class="sxs-lookup"><span data-stu-id="268d6-177">Optional.</span></span> <span data-ttu-id="268d6-178">包含视频的 iframe 的宽度。</span><span class="sxs-lookup"><span data-stu-id="268d6-178">The width of the iframe that contains the video.</span></span> <span data-ttu-id="268d6-179">默认值为 480。</span><span class="sxs-lookup"><span data-stu-id="268d6-179">Default is 480.</span></span>

<span data-ttu-id="268d6-180">示例：`width="300"`</span><span class="sxs-lookup"><span data-stu-id="268d6-180">Example: `width="300"`</span></span>

#### <a name="height"></a><span data-ttu-id="268d6-181">height</span><span class="sxs-lookup"><span data-stu-id="268d6-181">height</span></span>

<span data-ttu-id="268d6-182">可选。</span><span class="sxs-lookup"><span data-stu-id="268d6-182">Optional.</span></span> <span data-ttu-id="268d6-183">包含视频的 iframe 的高度。</span><span class="sxs-lookup"><span data-stu-id="268d6-183">The height of the iframe that contains the video.</span></span> <span data-ttu-id="268d6-184">默认值为 360。</span><span class="sxs-lookup"><span data-stu-id="268d6-184">Default is 360.</span></span>

<span data-ttu-id="268d6-185">示例：`height="300"`</span><span class="sxs-lookup"><span data-stu-id="268d6-185">Example: `height="300"`</span></span>

### <a name="example"></a><span data-ttu-id="268d6-186">示例</span><span class="sxs-lookup"><span data-stu-id="268d6-186">Example</span></span>

<span data-ttu-id="268d6-187">在请求的输入 HTML 中，包括 `<iframe data-original-src="https://..." />` 并为 **data-original-src** 属性指定视频的 URL。</span><span class="sxs-lookup"><span data-stu-id="268d6-187">In the input HTML of your request, include `<iframe data-original-src="https://..." />` and specify the URL of the video for the **data-original-src** attribute.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
    <head>
        <title>A page with an embedded video</title>
    </head>
    <body>
        <iframe data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8" width="340" height="280"/>
    </body>
</html>

--MyAppPartBoundary--
```


<a name="adding-files"></a>

## <a name="adding-files"></a><span data-ttu-id="268d6-188">添加文件</span><span class="sxs-lookup"><span data-stu-id="268d6-188">Adding files</span></span>

<span data-ttu-id="268d6-189">可以在输入 HTML 中使用 **object** 对象元素将文件附件添加到 OneNote 页面。</span><span class="sxs-lookup"><span data-stu-id="268d6-189">You can add file attachments to OneNote pages using an **object** element in the input HTML.</span></span> <span data-ttu-id="268d6-190">如果要添加 PDF 文件，则可以使用 **img** 元素将 PDF 元素页呈现为图像。</span><span class="sxs-lookup"><span data-stu-id="268d6-190">If you're adding a PDF file, you can use an **img** element to render the PDF pages as images.</span></span> 

[<span data-ttu-id="268d6-191">添加文件附件</span><span class="sxs-lookup"><span data-stu-id="268d6-191">Add a file attachment</span></span>](#add-a-file-attachment)

<span data-ttu-id="268d6-192">使用 `<object .../>`，并发送多部分请求的数据部件中的文件。</span><span class="sxs-lookup"><span data-stu-id="268d6-192">Use `<object .../>` and send the file in a data part of a multipart request.</span></span> <span data-ttu-id="268d6-193">添加在 OneNote 页面上显示文件图标的文件附件。</span><span class="sxs-lookup"><span data-stu-id="268d6-193">Adds a file attachment that displays a file icon on the OneNote page.</span></span>

[<span data-ttu-id="268d6-194">添加 PDF 文件内容的图像</span><span class="sxs-lookup"><span data-stu-id="268d6-194">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)

<span data-ttu-id="268d6-195">使用 `<img data-render-src="name:part-name" />`，并发送多部分请求的数据部件中的 PDF 文件。</span><span class="sxs-lookup"><span data-stu-id="268d6-195">Use `<img data-render-src="name:part-name" />` and send a PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="268d6-196">在 OneNote 页上将每个 PDF 页呈现为单独图像。</span><span class="sxs-lookup"><span data-stu-id="268d6-196">Renders each PDF page as a separate image on the OneNote page.</span></span>

#### <a name="file-attributes"></a><span data-ttu-id="268d6-197">文件属性</span><span class="sxs-lookup"><span data-stu-id="268d6-197">File attributes</span></span>

<span data-ttu-id="268d6-198">**object** 元素需要下列属性。</span><span class="sxs-lookup"><span data-stu-id="268d6-198">The **object** element requires the following attributes.</span></span>

<span data-ttu-id="268d6-199">**data-attachment**</span><span class="sxs-lookup"><span data-stu-id="268d6-199">**data-attachment**</span></span>

<span data-ttu-id="268d6-200">要在 OneNote 页面上显示的文件名和扩展名。</span><span class="sxs-lookup"><span data-stu-id="268d6-200">The file name and extension to display on the OneNote page.</span></span>

<span data-ttu-id="268d6-201">示例：`data-attachment="filename.docx"`</span><span class="sxs-lookup"><span data-stu-id="268d6-201">Example: `data-attachment="filename.docx"`</span></span>

<span data-ttu-id="268d6-202">**data**</span><span class="sxs-lookup"><span data-stu-id="268d6-202">**data**</span></span>

<span data-ttu-id="268d6-203">包含二进制文件数据的多部分请求的正文部分的名称。</span><span class="sxs-lookup"><span data-stu-id="268d6-203">The name of the body part in the multipart request that contains the binary file data.</span></span> <span data-ttu-id="268d6-204">Microsoft Graph 不支持在此处传递 URL 引用。</span><span class="sxs-lookup"><span data-stu-id="268d6-204">Microsoft Graph does not support passing a URL reference here.</span></span>

<span data-ttu-id="268d6-205">示例：`data="name:part-name"`</span><span class="sxs-lookup"><span data-stu-id="268d6-205">Example: `data="name:part-name"`</span></span>

<span data-ttu-id="268d6-206">**type**</span><span class="sxs-lookup"><span data-stu-id="268d6-206">**type**</span></span>

<span data-ttu-id="268d6-207">文件媒体类型用于确定页面上使用的文件图标，同时还确定当用户从 OneNote 激活设备上的文件时，会启动哪个应用程序。</span><span class="sxs-lookup"><span data-stu-id="268d6-207">The file media type, used to determine the file icon to use on the page, and which application starts when the user activates the file on the device from OneNote.</span></span>

<span data-ttu-id="268d6-208">示例：`type="application/pdf"`</span><span class="sxs-lookup"><span data-stu-id="268d6-208">Example: `type="application/pdf"`</span></span>


<a name="file-media-types"></a>

#### <a name="file-media-types"></a><span data-ttu-id="268d6-209">文件媒体类型</span><span class="sxs-lookup"><span data-stu-id="268d6-209">File media types</span></span>  

<span data-ttu-id="268d6-210">Microsoft Graph 为附加文件使用预定义的文件类型图标，当 API 不识别文件类型时，Microsoft Graph 会为其使用通用图标。</span><span class="sxs-lookup"><span data-stu-id="268d6-210">Microsoft Graph uses predefined file-types icon for attached files, or a generic icon when the API doesn't recognize the file type.</span></span> <span data-ttu-id="268d6-211">下表显示了 API 可识别的一些常见文件类型。</span><span class="sxs-lookup"><span data-stu-id="268d6-211">The following table shows some common file types that are recognized by the API.</span></span>

- <span data-ttu-id="268d6-212">application/pdf</span><span class="sxs-lookup"><span data-stu-id="268d6-212">application/pdf</span></span>  
- <span data-ttu-id="268d6-213">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span><span class="sxs-lookup"><span data-stu-id="268d6-213">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span></span>  
- <span data-ttu-id="268d6-214">application/vnd.openxmlformats-officedocument.presentationml.presentation</span><span class="sxs-lookup"><span data-stu-id="268d6-214">application/vnd.openxmlformats-officedocument.presentationml.presentation</span></span>
- <span data-ttu-id="268d6-215">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span><span class="sxs-lookup"><span data-stu-id="268d6-215">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span></span>
- <span data-ttu-id="268d6-216">image/png</span><span class="sxs-lookup"><span data-stu-id="268d6-216">image/png</span></span>
- <span data-ttu-id="268d6-217">image/jpeg</span><span class="sxs-lookup"><span data-stu-id="268d6-217">image/jpeg</span></span>
- <span data-ttu-id="268d6-218">image/gif</span><span class="sxs-lookup"><span data-stu-id="268d6-218">image/gif</span></span>
- <span data-ttu-id="268d6-219">audio/wav</span><span class="sxs-lookup"><span data-stu-id="268d6-219">audio/wav</span></span>
- <span data-ttu-id="268d6-220">video/mp4</span><span class="sxs-lookup"><span data-stu-id="268d6-220">video/mp4</span></span>
- <span data-ttu-id="268d6-221">application/msword</span><span class="sxs-lookup"><span data-stu-id="268d6-221">application/msword</span></span>
- <span data-ttu-id="268d6-222">application/mspowerpoint</span><span class="sxs-lookup"><span data-stu-id="268d6-222">application/mspowerpoint</span></span>
- <span data-ttu-id="268d6-223">application/excel</span><span class="sxs-lookup"><span data-stu-id="268d6-223">application/excel</span></span>

<span data-ttu-id="268d6-224">请参阅创建包含媒体的页面时应用的[限制](#size-limitations-for-post-pages-requests)。</span><span class="sxs-lookup"><span data-stu-id="268d6-224">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="file-object"></a>

### <a name="add-a-file-attachment"></a><span data-ttu-id="268d6-225">添加文件附件</span><span class="sxs-lookup"><span data-stu-id="268d6-225">Add a file attachment</span></span>

<span data-ttu-id="268d6-226">在请求的 **演示** 部分的输入 HTML 中，包括 `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`，其中 *part-name* 是包含二进制文件数据的 [多部分请求](onenote-create-page.md#example-request)中的数据部分的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="268d6-226">In the input HTML of your request's **Presentation** part, include `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="268d6-227">请只发送二进制数据，不要使用 Base64 或其他方式对其进行编码。</span><span class="sxs-lookup"><span data-stu-id="268d6-227">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with an image file attachment</title>
  </head>
  <body>
    <p>This is an image file attachment.</p>
    <object data-attachment="Logo.jpg" data="name:logo1-file" type="image/jpeg" />
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="logo1-file"
Content-Type: image/jpeg

... binary file data ...

--MyAppPartBoundary--
```


<a name="file-binary-data-render-src"></a>

### <a name="add-images-of-pdf-file-contents"></a><span data-ttu-id="268d6-228">添加 PDF 文件内容的图像</span><span class="sxs-lookup"><span data-stu-id="268d6-228">Add images of PDF file contents</span></span>

<span data-ttu-id="268d6-229">在请求的 **演示** 部分的输入 HTML 中，包括 `<img data-render-src="name:part-name" ... />`，其中 *part-name* 是包含二进制文件数据的 [多部分请求](onenote-create-page.md#example-request)中的数据部分的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="268d6-229">In the input HTML of your request's **Presentation** part, include `<img data-render-src="name:part-name" ... />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="268d6-230">请只发送二进制数据，不要使用 Base64 或其他方式对其进行编码。</span><span class="sxs-lookup"><span data-stu-id="268d6-230">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

```html
Content-Type: multipart/form-data; boundary=MyAppPartBoundary
Authorization: Bearer {access-token}

--MyAppPartBoundary
Content-Disposition: form-data; name="Presentation"
Content-Type: text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with images of the pages of a PDF file</title>
  </head>
  <body>
    <p>The pages of this PDF file render as images.</p>
    <img data-render-src="name:file-part" alt="PDF file as images" width="500"/>
  </body>
</html>

--MyAppPartBoundary
Content-Disposition: form-data; name="file-part"
Content-Type: application/pdf

... binary file data ...

--MyAppPartBoundary--  
```


<a name="size-limits"></a>

## <a name="size-limitations-for-post-pages-requests"></a><span data-ttu-id="268d6-231">POST 页面请求的大小限制</span><span class="sxs-lookup"><span data-stu-id="268d6-231">Size limitations for POST pages requests</span></span>

<span data-ttu-id="268d6-232">发送图像和文件数据时，应注意以下限制：</span><span class="sxs-lookup"><span data-stu-id="268d6-232">When sending image and file data, be aware of these limitations:</span></span> <!--TODO: check these-->

- <span data-ttu-id="268d6-233">Microsoft Graph REST API 具有 4 MB 请求限制。</span><span class="sxs-lookup"><span data-stu-id="268d6-233">The Microsoft Graph REST API has a 4 MB request limit.</span></span> <span data-ttu-id="268d6-234">上方的所有项目将失败，显示错误消息“请求过大 (413)”。</span><span class="sxs-lookup"><span data-stu-id="268d6-234">Anything above this will fail with the error message "request too large (413)".</span></span> 

- <span data-ttu-id="268d6-235">底层 OneNote REST API 的请求限制较高，但你无法通过 Microsoft Graph API 访问它。</span><span class="sxs-lookup"><span data-stu-id="268d6-235">The request limit of the underlying OneNote REST API is higher, but you cannot access it via the Microsoft Graph API.</span></span> 
  - <span data-ttu-id="268d6-236">POST 的总大小限制为 ~ 70 MB，包括图像、文件和其他数据。</span><span class="sxs-lookup"><span data-stu-id="268d6-236">The total POST size limit is ~70 MB, including images, files, and other data.</span></span> <span data-ttu-id="268d6-237">实际限制会受下游编码的影响，因此没有固定的字节计数限制。</span><span class="sxs-lookup"><span data-stu-id="268d6-237">The actual limit is affected by downstream encoding, so there's no fixed byte-count limit.</span></span> <span data-ttu-id="268d6-238">超过此限制的请求可能会产生不可靠的结果。</span><span class="sxs-lookup"><span data-stu-id="268d6-238">Requests that exceed the limit might produce unreliable results.</span></span>
  - <span data-ttu-id="268d6-239">每个数据部件限制为 25 MB，包括部件标头。</span><span class="sxs-lookup"><span data-stu-id="268d6-239">The limit for each data part is 25 MB, including the part headers.</span></span> <span data-ttu-id="268d6-240">Microsoft Graph 将拒绝超过此限制的数据部件。</span><span class="sxs-lookup"><span data-stu-id="268d6-240">Data parts that exceed the limit are rejected by Microsoft Graph.</span></span> 

- <span data-ttu-id="268d6-241">每个页面的最大图像数为 150。</span><span class="sxs-lookup"><span data-stu-id="268d6-241">The maximum number of images per page is 150.</span></span> <span data-ttu-id="268d6-242">使用 `src="https://..."` 属性时，API 将忽略超出此限制的 **img** 标记。</span><span class="sxs-lookup"><span data-stu-id="268d6-242">When using the `src="https://..."` attribute, the API ignores **img** tags beyond the limit.</span></span>

- <span data-ttu-id="268d6-243">数据部件的最大数量是每个 POST 6 个，包括必需的 **Presentation** 部件。</span><span class="sxs-lookup"><span data-stu-id="268d6-243">The maximum number of data parts is 6 per POST, including the required **Presentation** part.</span></span>

- <span data-ttu-id="268d6-p129">每个请求可以包含最多 5 个使用 **data-render-src** 的 **img** 元素和一个使用 **data-render-src** 的 **object** 元素。其他图像和文件引用将被忽略。</span><span class="sxs-lookup"><span data-stu-id="268d6-p129">Each request can contain up to five **img** elements that use **data-render-src** and one **object** elements that uses **data-render-src**. Additional image and file references are ignored.</span></span>

- <span data-ttu-id="268d6-246">无论使用哪种方法将图像发送到 API，单个 POST 中图像的最大数量都是 30 个。</span><span class="sxs-lookup"><span data-stu-id="268d6-246">The maximum number of images in a single POST is 30, no matter which method you use to send them to the API.</span></span> <span data-ttu-id="268d6-247">其他图像将被忽略。</span><span class="sxs-lookup"><span data-stu-id="268d6-247">Additional images are ignored.</span></span> <span data-ttu-id="268d6-248">如果想要捕获包含大量图像的网页，请考虑[捕获整个页面作为快照](#add-a-webpage-snapshot)。</span><span class="sxs-lookup"><span data-stu-id="268d6-248">If you want to capture a webpage that contains a lot of images, consider [capturing the whole page as a snapshot](#add-a-webpage-snapshot).</span></span>


## <a name="when-to-use-html-versus-data-render-src"></a><span data-ttu-id="268d6-249">何时将 HTML 与 data-render-src 结合使用</span><span class="sxs-lookup"><span data-stu-id="268d6-249">When to use HTML versus data-render-src</span></span> 

<span data-ttu-id="268d6-250">尝试在直接将 HTML 置于 OneNote 页面与使用 **data-render-src** 属性之间选择时，请考虑以下情况：</span><span class="sxs-lookup"><span data-stu-id="268d6-250">When trying to decide between putting HTML directly onto the OneNote page instead of using the **data-render-src** attribute, consider the following:</span></span>

- <span data-ttu-id="268d6-251">最好通过 **data-render-src** 发送复杂 HTML 来呈现引擎，而不是尝试修改 HTML 来使其符合 Microsoft Graph 的要求。</span><span class="sxs-lookup"><span data-stu-id="268d6-251">Complex HTML is probably best sent to the rendering engine via **data-render-src**, rather than attempting to modify the HTML to fit into what Microsoft Graph can accept.</span></span> <span data-ttu-id="268d6-252">此外，当 HTML 包含不支持的标记时，这也是如此。</span><span class="sxs-lookup"><span data-stu-id="268d6-252">This is also true when your HTML includes tags that aren't supported supported.</span></span>

- <span data-ttu-id="268d6-253">精确页面呈现，以保留页面布局和外观时，最好是通过 **data-render-src** 使用呈现引擎完成。</span><span class="sxs-lookup"><span data-stu-id="268d6-253">Accurate page rendering to preserve the layout and look of the page is probably best done with the rendering engine via **data-render-src**.</span></span>

- <span data-ttu-id="268d6-p132">直接可编辑文本，实现时通常需要将 HTML 直接插入页面。呈现的图像由光学字符识别 (OCR) 系统进行扫描，但会有所不同。</span><span class="sxs-lookup"><span data-stu-id="268d6-p132">Directly-editable text is often best done with inserting the HTML directly onto the page. The rendered images are scanned by an optical character recognition (OCR) system, but it's just not the same.</span></span>

- <span data-ttu-id="268d6-256">用于历史记录或存档目的的实时快照最好使用 **data-render-src** 方法来捕获。</span><span class="sxs-lookup"><span data-stu-id="268d6-256">Snapshot-in-time for historical or archival purposes is usually best done with the **data-render-src** method.</span></span>

- <span data-ttu-id="268d6-p133">标记网页设计以便于修订，是 **data-render-src** 的亮点所在。您可以使用 OneNote 的墨迹书写功能在图像上绘图，以指示更改或标出重要区域。将网页处理为图像可大大简化该过程。</span><span class="sxs-lookup"><span data-stu-id="268d6-p133">Marking-up a web page design for revisions is one place the **data-render-src** truly shines. Using OneNote's inking capabilities, you can draw on the image to indicate changes or call out important areas. Having the web page as an image makes that a lot easier.</span></span>

- <span data-ttu-id="268d6-260">对于很大的图像或格式不是 OneNote 可直接接受的图像，有时可以生成缩略图，与在自己的代码中进行图像转换相比，使用 **data-render-src** 属性转换更为容易。</span><span class="sxs-lookup"><span data-stu-id="268d6-260">Very large images, or images in formats that OneNote doesn't directly accept, can sometimes be thumbnailed and converted with the **data-render-src** attribute more easily than by doing it in your own code.</span></span> <span data-ttu-id="268d6-261">虽然图像也可以在线使用，但通过减少生成 OneNote 页所需的往返总次数，将数据嵌入到 POST 中，有时可以使 OneNote 用户更快地使用捕获到的页面。</span><span class="sxs-lookup"><span data-stu-id="268d6-261">Even if the image is also available online, embedding the data in your POST can sometimes make the captured page available to OneNote users sooner, by reducing the total number of round-trips needed to build the OneNote page.</span></span>

<span data-ttu-id="268d6-262">有时，确定哪种方法最适合用户的最佳方法是在开发应用时尝试这两种方法。</span><span class="sxs-lookup"><span data-stu-id="268d6-262">Sometimes, the best way to determine which method will work best for your users is to try it both ways as you develop your app.</span></span>


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="268d6-263">权限</span><span class="sxs-lookup"><span data-stu-id="268d6-263">Permissions</span></span>

<span data-ttu-id="268d6-264">若要创建或更新 OneNote 页面，需要请求相应的权限。</span><span class="sxs-lookup"><span data-stu-id="268d6-264">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="268d6-265">选择应用正常运行所需的最低级别。</span><span class="sxs-lookup"><span data-stu-id="268d6-265">Choose the lowest level that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="268d6-266">POST 页面的权限</span><span class="sxs-lookup"><span data-stu-id="268d6-266">Permissions for POST pages</span></span>

- <span data-ttu-id="268d6-267">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="268d6-267">Notes.Create</span></span>
- <span data-ttu-id="268d6-268">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="268d6-268">Notes.ReadWrite</span></span>
- <span data-ttu-id="268d6-269">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="268d6-269">Notes.ReadWrite.All</span></span> 

#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="268d6-270">PATCH 页面的权限</span><span class="sxs-lookup"><span data-stu-id="268d6-270">Permissions for PATCH pages</span></span>

- <span data-ttu-id="268d6-271">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="268d6-271">Notes.ReadWrite</span></span>
- <span data-ttu-id="268d6-272">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="268d6-272">Notes.ReadWrite.All</span></span>

<span data-ttu-id="268d6-273">有关权限范围及其工作方式的详细信息，请参阅 [OneNote 权限范围](permissions-reference.md#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="268d6-273">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions-reference.md#notes-permissions).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="268d6-274">另请参阅</span><span class="sxs-lookup"><span data-stu-id="268d6-274">See also</span></span>

- [<span data-ttu-id="268d6-275">与 OneNote 集成</span><span class="sxs-lookup"><span data-stu-id="268d6-275">Integrate with OneNote</span></span>](integrate-with-onenote.md)
- [<span data-ttu-id="268d6-276">OneNote 开发者博客</span><span class="sxs-lookup"><span data-stu-id="268d6-276">OneNote Developer Blog</span></span>](https://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="268d6-277">Microsoft Q&A 上的 OneNote 开发问题</span><span class="sxs-lookup"><span data-stu-id="268d6-277">OneNote development questions on Microsoft Q&A</span></span>](/answers/topics/microsoft-graph-notes.html)
- [<span data-ttu-id="268d6-278">OneNote GitHub 存储库</span><span class="sxs-lookup"><span data-stu-id="268d6-278">OneNote GitHub repos</span></span>](https://go.microsoft.com/fwlink/?LinkID=390178)