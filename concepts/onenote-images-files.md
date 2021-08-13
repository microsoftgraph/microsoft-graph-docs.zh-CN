---
title: 将图像、视频和文件添加到 OneNote 页面
description: " Microsoft 365 中的企业笔记本"
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: 06252d15755d7e11cce703657cb0aea0ff914075021c1d11cf548c96359fe4dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54159671"
---
# <a name="add-images-videos-and-files-to-onenote-pages"></a>将图像、视频和文件添加到 OneNote 页面

**适用于** OneDrive 上的消费者笔记本 | Microsoft 365 上的企业级笔记本

在 [创建](onenote-create-page.md)或 [更新](onenote-update-page.md)页面时，可以使用 **img**、**object** 和 **iframe** 元素将图像、视频和文件添加到 OneNote 页面。 

- 使用 **img** 在页面上呈现图像。
- 使用 **iframe** 在页面上嵌入视频。
- 使用 **object** 将文件附件添加到页面。


<a name="images"></a>

## <a name="adding-images"></a>添加图像

图像可以通过 URL 引用或发送原始数据来进行添加。 Microsoft Graph 支持以下可将图像、徽标和照片添加到 OneNote 页面的方法。 

[从 Web 添加公共图像](#add-a-public-image-from-the-web)

将 `img` 与 `src="https://image-url"` 结合使用，并指定可公开访问图像的 URL。 在 OneNote 页面上呈现图像。

[使用二进制数据添加图像](#add-an-image-using-binary-data)

将 `img` 与 `src="name:image-block-name"` 结合使用，并发送多部分请求的数据部件中的图像文件。 在 OneNote 页面上呈现图像。

[添加网页快照](#add-a-webpage-snapshot)

将 `img` 与 `data-render-src="https://webpage-url"` 结合使用，并指定网页的 URL。 在 OneNote 页面上呈现整个网页的快照。

[添加从 HTML 呈现的图像](#add-an-image-rendered-from-html)

将 `img` 与 `data-render-src="name:html-block-name"` 结合使用，并发送多部分请求的数据部件中的 HTML。 在 OneNote 页面上将 HTML 呈现为图像。

[添加 PDF 文件内容的图像](#add-images-of-pdf-file-contents)

使用 `<img data-render-src="name:part-name" />`，并发送多部分请求的数据部件中的 PDF 文件。 在 OneNote 页面上将每个 PDF 页面呈现为单独图像。

[将图像文件添加为文件附件](#add-an-image-file-as-an-attachment)

将 `object` 与 `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` 结合使用，并发送多部分请求的数据部件中的图像文件。 将文件附件添加到 OneNote 页面，并显示文件图标。


> **注意：** 若要获取 OneNote 页面上的图像，首先发送 [GET 请求获取页面内容](onenote-get-content.md#page-html-content)。 这会将 URL 返回到页面上的图像资源。 然后，将 [GET 请求与图像资源分开](onenote-get-content.md#image-or-other-file-resource)。


#### <a name="image-attributes"></a>图像属性 

**img** 元素可以选择包括 **alt**、**height** 和 **width** 属性，以及样式属性 **max-width** 和 **max-height**。

#### <a name="image-media-types"></a>图像媒体类型

Microsoft Graph 支持 TIFF、PNG、GIF、JPEG 和 BMP 图像类型。 若要捕获使用不想转换的其他格式的图像，请在多部分请求中[发送二进制数据](#add-an-image-using-binary-data)。 不需要使用 Base64，或其他方式对发送的二进制数据进行编码。

> **注意：** API 会检测原始输入图像类型，并在 [输出 HTML](onenote-input-output-html.md#output-html) 中将其作为 **data-fullres-src-type** 属性返回。 此外，API 还会在 **data-src-type** 中返回优化图像的图像类型。
 
请参阅创建包含媒体的页面时应用的[限制](#size-limitations-for-post-pages-requests)。


<a name="image-img-url-src"></a>

### <a name="add-a-public-image-from-the-web"></a>从 Web 添加公共图像

在请求的输入 HTML 中，包括 `<img src="https://..." />` 并为 **src** 属性指定可公开访问图像的 URL。

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

### <a name="add-an-image-using-binary-data"></a>使用二进制数据添加图像

在请求的 **演示** 部分的输入 HTML 中，包括 `<img src="name:part-name" />`，其中 *part-name* 是包含二进制图像数据的 [多部分请求](onenote-create-page.md#example-request)中数据部分的唯一标识符。 请只发送二进制数据，不要使用 Base64 或其他方式对其进行编码。

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

### <a name="add-a-webpage-snapshot"></a>添加网页快照

可以使用 Microsoft Graph 截取整个网页的快照，并将其插入到新页面中。 此方法对存档网页或捕获具有 OneNote 不支持的功能（如某些 CSS）的复杂网页很有用。  

在请求的输入 HTML 中，包括 `<img src="https://..." />` 并指定要为 **src** 属性插入的网页的 URL。

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

### <a name="add-an-image-rendered-from-html"></a>添加从 HTML 呈现的图像

将 HTML 作为数据块传递时，请确保没有需要用户凭据或预加载浏览器插件的活动内容。 Microsoft Graph 用于将 HTML 页面呈现为图像的引擎无法登录用户，且不包含诸如 Adobe Flash、Apple QuickTime 等插件。 这也意味着，如果获取数据需要用户登录凭据或 Cookie，将不会显示动态加载的内容（如可能带有 AJAX 脚本）。

在请求的 **演示** 部分的输入 HTML 中，包括 `<img data-render-src="name:part-name" />`，其中 *part-name* 是包含 HTML 的 [多部分请求](onenote-create-page.md#example-request)中数据部分的唯一标识符。


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

### <a name="add-an-image-file-as-an-attachment"></a>将图像文件添加为附件

在请求的 **演示** 部分的输入 HTML 中，包括 `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`，其中 *part-name* 是包含二进制图像数据的 [多部分请求](onenote-create-page.md#example-request)中数据部分的唯一标识符。 请只发送二进制数据，不要使用 Base64 或其他方式对其进行编码。

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

了解有关[文件媒体类型](#file-media-types)的详细信息。



<a name="adding-videos"></a>

## <a name="adding-videos"></a>添加视频

可以在输入 HTML 中使用 `<iframe data-original-src="https://..." />` 在 OneNote 页面中嵌入视频。 

### <a name="supported-video-sites"></a>支持的视频网站

- Dailymotion
- Office Mix
- Sway
- Sketchfab
- TED
- YouTube
- Vimeo
- Vine

### <a name="iframe-attributes"></a>iframe 属性

#### <a name="data-original-src"></a>data-original-src

必需。 视频的 URL。

示例：`data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`

#### <a name="width"></a>width

可选。 包含视频的 iframe 的宽度。 默认值为 480。

示例：`width="300"`

#### <a name="height"></a>height

可选。 包含视频的 iframe 的高度。 默认值为 360。

示例：`height="300"`

### <a name="example"></a>示例

在请求的输入 HTML 中，包括 `<iframe data-original-src="https://..." />` 并为 **data-original-src** 属性指定视频的 URL。

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

## <a name="adding-files"></a>添加文件

可以在输入 HTML 中使用 **object** 对象元素将文件附件添加到 OneNote 页面。 如果要添加 PDF 文件，则可以使用 **img** 元素将 PDF 元素页呈现为图像。 

[添加文件附件](#add-a-file-attachment)

使用 `<object .../>`，并发送多部分请求的数据部件中的文件。 添加在 OneNote 页面上显示文件图标的文件附件。

[添加 PDF 文件内容的图像](#add-images-of-pdf-file-contents)

使用 `<img data-render-src="name:part-name" />`，并发送多部分请求的数据部件中的 PDF 文件。 在 OneNote 页上将每个 PDF 页呈现为单独图像。

#### <a name="file-attributes"></a>文件属性

**object** 元素需要下列属性。

**data-attachment**

要在 OneNote 页面上显示的文件名和扩展名。

示例：`data-attachment="filename.docx"`

**data**

包含二进制文件数据的多部分请求的正文部分的名称。 Microsoft Graph 不支持在此处传递 URL 引用。

示例：`data="name:part-name"`

**type**

文件媒体类型用于确定页面上使用的文件图标，同时还确定当用户从 OneNote 激活设备上的文件时，会启动哪个应用程序。

示例：`type="application/pdf"`


<a name="file-media-types"></a>

#### <a name="file-media-types"></a>文件媒体类型  

Microsoft Graph 为附加文件使用预定义的文件类型图标，当 API 不识别文件类型时，Microsoft Graph 会为其使用通用图标。 下表显示了 API 可识别的一些常见文件类型。

- application/pdf  
- application/vnd.openxmlformats-officedocument.wordprocessingml.document  
- application/vnd.openxmlformats-officedocument.presentationml.presentation
- application/vnd.openxmlformats-officedocument.spreadsheetml.sheet
- image/png
- image/jpeg
- image/gif
- audio/wav
- video/mp4
- application/msword
- application/mspowerpoint
- application/excel

请参阅创建包含媒体的页面时应用的[限制](#size-limitations-for-post-pages-requests)。


<a name="file-object"></a>

### <a name="add-a-file-attachment"></a>添加文件附件

在请求的 **演示** 部分的输入 HTML 中，包括 `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`，其中 *part-name* 是包含二进制文件数据的 [多部分请求](onenote-create-page.md#example-request)中的数据部分的唯一标识符。 请只发送二进制数据，不要使用 Base64 或其他方式对其进行编码。

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

### <a name="add-images-of-pdf-file-contents"></a>添加 PDF 文件内容的图像

在请求的 **演示** 部分的输入 HTML 中，包括 `<img data-render-src="name:part-name" ... />`，其中 *part-name* 是包含二进制文件数据的 [多部分请求](onenote-create-page.md#example-request)中的数据部分的唯一标识符。 请只发送二进制数据，不要使用 Base64 或其他方式对其进行编码。

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

## <a name="size-limitations-for-post-pages-requests"></a>POST 页面请求的大小限制

发送图像和文件数据时，应注意以下限制： <!--TODO: check these-->

- Microsoft Graph REST API 具有 4 MB 请求限制。 上方的所有项目将失败，显示错误消息“请求过大 (413)”。 

- 底层 OneNote REST API 的请求限制较高，但你无法通过 Microsoft Graph API 访问它。 
  - POST 的总大小限制为 ~ 70 MB，包括图像、文件和其他数据。 实际限制会受下游编码的影响，因此没有固定的字节计数限制。 超过此限制的请求可能会产生不可靠的结果。
  - 每个数据部件限制为 25 MB，包括部件标头。 Microsoft Graph 将拒绝超过此限制的数据部件。 

- 每个页面的最大图像数为 150。 使用 `src="https://..."` 属性时，API 将忽略超出此限制的 **img** 标记。

- 数据部件的最大数量是每个 POST 6 个，包括必需的 **Presentation** 部件。

- 每个请求可以包含最多 5 个使用 **data-render-src** 的 **img** 元素和一个使用 **data-render-src** 的 **object** 元素。其他图像和文件引用将被忽略。

- 无论使用哪种方法将图像发送到 API，单个 POST 中图像的最大数量都是 30 个。 其他图像将被忽略。 如果想要捕获包含大量图像的网页，请考虑[捕获整个页面作为快照](#add-a-webpage-snapshot)。


## <a name="when-to-use-html-versus-data-render-src"></a>何时将 HTML 与 data-render-src 结合使用 

尝试在直接将 HTML 置于 OneNote 页面与使用 **data-render-src** 属性之间选择时，请考虑以下情况：

- 最好通过 **data-render-src** 发送复杂 HTML 来呈现引擎，而不是尝试修改 HTML 来使其符合 Microsoft Graph 的要求。 此外，当 HTML 包含不支持的标记时，这也是如此。

- 精确页面呈现，以保留页面布局和外观时，最好是通过 **data-render-src** 使用呈现引擎完成。

- 直接可编辑文本，实现时通常需要将 HTML 直接插入页面。呈现的图像由光学字符识别 (OCR) 系统进行扫描，但会有所不同。

- 用于历史记录或存档目的的实时快照最好使用 **data-render-src** 方法来捕获。

- 标记网页设计以便于修订，是 **data-render-src** 的亮点所在。您可以使用 OneNote 的墨迹书写功能在图像上绘图，以指示更改或标出重要区域。将网页处理为图像可大大简化该过程。

- 对于很大的图像或格式不是 OneNote 可直接接受的图像，有时可以生成缩略图，与在自己的代码中进行图像转换相比，使用 **data-render-src** 属性转换更为容易。 虽然图像也可以在线使用，但通过减少生成 OneNote 页所需的往返总次数，将数据嵌入到 POST 中，有时可以使 OneNote 用户更快地使用捕获到的页面。

有时，确定哪种方法最适合用户的最佳方法是在开发应用时尝试这两种方法。


<a name="permissions"></a>

## <a name="permissions"></a>权限

若要创建或更新 OneNote 页面，需要请求相应的权限。 选择应用正常运行所需的最低级别。

#### <a name="permissions-for-post-pages"></a>POST 页面的权限

- Notes.Create
- Notes.ReadWrite
- Notes.ReadWrite.All 

#### <a name="permissions-for-patch-pages"></a>PATCH 页面的权限

- Notes.ReadWrite
- Notes.ReadWrite.All

有关权限范围及其工作方式的详细信息，请参阅 [OneNote 权限范围](permissions-reference.md#notes-permissions)。


<a name="see-also"></a>

## <a name="see-also"></a>另请参阅

- [与 OneNote 集成](integrate-with-onenote.md)
- [OneNote 开发者博客](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Microsoft Q&A 上的 OneNote 开发问题](/answers/topics/microsoft-graph-notes.html)
- [OneNote GitHub 存储库](https://go.microsoft.com/fwlink/?LinkID=390178)