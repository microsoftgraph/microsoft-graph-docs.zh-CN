
# <a name="add-images-videos-and-files-to-onenote-pages"></a><span data-ttu-id="8f9a2-101">将图像、视频和文件添加到 OneNote 页面</span><span class="sxs-lookup"><span data-stu-id="8f9a2-101">Add images, videos, and files to OneNote pages</span></span>

<span data-ttu-id="8f9a2-102">**适用于** OneDrive 上的消费者笔记本 | Office 365 上的企业级笔记本</span><span class="sxs-lookup"><span data-stu-id="8f9a2-102">**Applies to:** Consumer notebooks on OneDrive | Enterprise notebooks on Office 365</span></span>

<span data-ttu-id="8f9a2-103">在[创建](onenote-create-page.md)或[更新](onenote_update_page.md)页面时，可以使用 **img**、**object** 和 **iframe** 元素将图像、视频和文件添加到 OneNote 页面。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-103">You can use **img**, **object**, and **iframe** elements to add images, videos, and files to a OneNote page when you're [creating](onenote-create-page.md) or [updating](onenote_update_page.md) the page.</span></span> 

- <span data-ttu-id="8f9a2-104">使用 **img** 在页面上呈现图像。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-104">Use **img** to render an image on the page.</span></span>
- <span data-ttu-id="8f9a2-105">使用 **iframe** 在页面上嵌入视频。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-105">Use **iframe** to embed a video on the page.</span></span>
- <span data-ttu-id="8f9a2-106">使用 **object** 将文件附件添加到页面。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-106">Use **object** to add a file attachment to the page.</span></span>


<a name="images"></a>

## <a name="adding-images"></a><span data-ttu-id="8f9a2-107">添加图像</span><span class="sxs-lookup"><span data-stu-id="8f9a2-107">Adding images</span></span>

<span data-ttu-id="8f9a2-108">图像可以通过 URL 引用或发送原始数据来进行添加。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-108">Images can be added by URL reference or by sending raw data.</span></span> <span data-ttu-id="8f9a2-109">Microsoft Graph 支持以下可将图像、徽标和照片添加到 OneNote 页面的方法。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-109">Microsoft Graph supports the following methods of adding images, logos, and photos to OneNote pages.</span></span> 

[<span data-ttu-id="8f9a2-110">从 Web 添加公共图像</span><span class="sxs-lookup"><span data-stu-id="8f9a2-110">Add a public image from the web</span></span>](#add-a-public-image-from-the-web)

<span data-ttu-id="8f9a2-111">将 `img` 与 `src="http://image-url"` 结合使用，并指定可公开访问图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-111">Use `img` with `src="http://image-url"` and specify the URL of a publicly accessible image.</span></span> <span data-ttu-id="8f9a2-112">在 OneNote 页面上呈现图像。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-112">Renders the image on the OneNote page.</span></span>

[<span data-ttu-id="8f9a2-113">使用二进制数据添加图像</span><span class="sxs-lookup"><span data-stu-id="8f9a2-113">Add an image using binary data</span></span>](#add-an-image-using-binary-data)

<span data-ttu-id="8f9a2-114">将 `img` 与 `src="name:image-block-name"` 结合使用，并发送多部分请求的数据部件中的图像文件。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-114">Use `img` with `src="name:image-block-name"` and send the image file in a data part of a multipart request.</span></span> <span data-ttu-id="8f9a2-115">在 OneNote 页面上呈现图像。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-115">Renders the image on the OneNote page.</span></span>

[<span data-ttu-id="8f9a2-116">添加网页快照</span><span class="sxs-lookup"><span data-stu-id="8f9a2-116">Add a webpage snapshot</span></span>](#add-a-webpage-snapshot)

<span data-ttu-id="8f9a2-117">将 `img` 与 `data-render-src="http://webpage-url"` 结合使用，并指定网页的 URL。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-117">Use `img` with `data-render-src="http://webpage-url"` and specify the URL of a webpage.</span></span> <span data-ttu-id="8f9a2-118">在 OneNote 页面上呈现整个网页的快照。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-118">Renders a snapshot of the whole webpage on the OneNote page.</span></span>

[<span data-ttu-id="8f9a2-119">添加从 HTML 呈现的图像</span><span class="sxs-lookup"><span data-stu-id="8f9a2-119">Add an image rendered from HTML</span></span>](#add-an-image-rendered-from-html)

<span data-ttu-id="8f9a2-120">将 `img` 与 `data-render-src="name:html-block-name"` 结合使用，并发送多部分请求的数据部件中的 HTML。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-120">Use `img` with `data-render-src="name:html-block-name"` and send HTML in the data part of a multipart request.</span></span> <span data-ttu-id="8f9a2-121">在 OneNote 页面上将 HTML 呈现为图像。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-121">Renders the HTML as an image on the OneNote page.</span></span>

[<span data-ttu-id="8f9a2-122">添加 PDF 文件内容的图像</span><span class="sxs-lookup"><span data-stu-id="8f9a2-122">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)

<span data-ttu-id="8f9a2-123">使用 `<img data-render-src="name:part-name" />`，并发送多部分请求的数据部件中的 PDF 文件。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-123">Use `<img data-render-src="name:part-name" />` and send the PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="8f9a2-124">在 OneNote 页面上将每个 PDF 页面呈现为单独图像。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-124">Renders each PDF page as a separate image on the OneNote page.</span></span>

[<span data-ttu-id="8f9a2-125">将图像文件添加为文件附件</span><span class="sxs-lookup"><span data-stu-id="8f9a2-125">Add an image file as a file attachment</span></span>](#add-an-image-file-as-an-attachment)

<span data-ttu-id="8f9a2-126">将 `object` 与 `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` 结合使用，并发送多部分请求的数据部件中的图像文件。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-126">Use `object` with `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` and send an image file in the data part of a multipart request.</span></span> <span data-ttu-id="8f9a2-127">将文件附件添加到 OneNote 页面，并显示文件图标。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-127">Adds a file attachment to the OneNote page and displays a file icon.</span></span>


> <span data-ttu-id="8f9a2-128">**注意：** 若要获取 OneNote 页面上的图像，首先发送 [GET 请求获取页面内容](onenote-get-content.md#page-html-content)。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-128">**Note:** To get images on a OneNote page, first send a [GET request for the page content](onenote-get-content.md#page-html-content).</span></span> <span data-ttu-id="8f9a2-129">这会将 URL 返回到页面上的图像资源。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-129">This returns the URLs to the image resources on the page.</span></span> <span data-ttu-id="8f9a2-130">然后，将 [GET 请求与图像资源分开](onenote-get-content.md#image-or-other-file-resource)。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-130">Then you separate [GET requests to the image resources](onenote-get-content.md#image-or-other-file-resource).</span></span>


#### <a name="image-attributes"></a><span data-ttu-id="8f9a2-131">图像属性</span><span class="sxs-lookup"><span data-stu-id="8f9a2-131">Image attributes</span></span> 

<span data-ttu-id="8f9a2-132">**img** 元素可以选择包括 **alt**、**height** 和 **width** 属性，以及样式属性 **max-width** 和 **max-height**。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-132">An **img** element can optionally include **alt**, **height**, and **width** attributes, and the style attributes **max-width** and **max-height**.</span></span>

#### <a name="image-media-types"></a><span data-ttu-id="8f9a2-133">图像媒体类型</span><span class="sxs-lookup"><span data-stu-id="8f9a2-133">Image media types</span></span>

<span data-ttu-id="8f9a2-134">Microsoft Graph 支持 TIFF、PNG、GIF、JPEG 和 BMP 图像类型。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-134">Microsoft Graph supports TIFF, PNG, GIF, JPEG, and BMP image types.</span></span> <span data-ttu-id="8f9a2-135">若要捕获使用不想转换的其他格式的图像，请在多部分请求中[发送二进制数据](#add-an-image-using-binary-data)。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-135">To capture an image that uses a different format that you don't want to convert, [send the binary data](#add-an-image-using-binary-data) in a multipart request.</span></span> <span data-ttu-id="8f9a2-136">不需要使用 Base64，或其他方式对发送的二进制数据进行编码。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-136">You don't need to use Base64 or otherwise encode the binary data that you send.</span></span>

> <span data-ttu-id="8f9a2-137">**注意：** API 会检测原始输入图像类型，并在[输出 HTML](onenote_input_output_html.md#output-html) 中将其作为 **data-fullres-src-type** 属性返回。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-137">**Note:** The API detects the original input image type, and returns it as the **data-fullres-src-type** attribute in the [output HTML](onenote_input_output_html.md#output-html).</span></span> <span data-ttu-id="8f9a2-138">此外，API 还会在 **data-src-type** 中返回优化图像的图像类型。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-138">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 
<span data-ttu-id="8f9a2-139">请参阅创建包含媒体的页面时应用的[限制](#size-limitations-for-post-pages-requests)。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-139">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="image-img-url-src"></a>

### <a name="add-a-public-image-from-the-web"></a><span data-ttu-id="8f9a2-140">从 Web 添加公共图像</span><span class="sxs-lookup"><span data-stu-id="8f9a2-140">Add a public image from the web</span></span>

<span data-ttu-id="8f9a2-141">在请求的输入 HTML 中，包括 `<img src="http://..." />` 并为 **src** 属性指定可公开访问图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-141">In the input HTML of your request, include  `<img src="http://..." />` and specify the URL of a publicly accessible image for the **src** attribute.</span></span>

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
    <img src="http://..." width="300"/>
  </body>
</html>

--MyAppPartBoundary--  
```

<a name="image-img-binary-src"></a>

### <a name="add-an-image-using-binary-data"></a><span data-ttu-id="8f9a2-142">使用二进制数据添加图像</span><span class="sxs-lookup"><span data-stu-id="8f9a2-142">Add an image using binary data</span></span>

<span data-ttu-id="8f9a2-143">在请求的**演示**部分的输入 HTML 中，包括 `<img src="name:part-name" />`，其中 *part-name* 是包含二进制图像数据的[多部分请求](onenote-create-page.md#example-request)中数据部分的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-143">In the input HTML of your request's **Presentation** part, include  `<img src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="8f9a2-144">请只发送二进制数据，不要使用 Base64 或其他方式对其进行编码。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-144">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

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

### <a name="add-a-webpage-snapshot"></a><span data-ttu-id="8f9a2-145">添加网页快照</span><span class="sxs-lookup"><span data-stu-id="8f9a2-145">Add a webpage snapshot</span></span>

<span data-ttu-id="8f9a2-146">可以使用 Microsoft Graph 截取整个网页的快照，并将其插入到新页面中。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-146">You can use Microsoft Graph to snapshot entire webpages and insert them into new pages.</span></span> <span data-ttu-id="8f9a2-147">此方法对存档网页或捕获具有 OneNote 不支持的功能（如某些 CSS）的复杂网页很有用。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-147">This method is useful to archive webpages or capture complex webpages that have features that OneNote doesn't support (like some CSS).</span></span>  

<span data-ttu-id="8f9a2-148">在请求的输入 HTML 中，包括 `<img src="http://..." />` 并指定要为 **src** 属性插入的网页的 URL。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-148">In the input HTML of your request, include  `<img src="http://..." />` and specify the URL of the webpage you want to insert for the **src** attribute.</span></span>

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
    <img data-render-src="http://www.onenote.com" width="200"/>
  </body>
</html>

--MyAppPartBoundary--  
```


<a name="image-img-binary-data-render-src"></a>

### <a name="add-an-image-rendered-from-html"></a><span data-ttu-id="8f9a2-149">添加从 HTML 呈现的图像</span><span class="sxs-lookup"><span data-stu-id="8f9a2-149">Add an image rendered from HTML</span></span>

<span data-ttu-id="8f9a2-150">将 HTML 作为数据块传递时，请确保没有需要用户凭据或预加载浏览器插件的活动内容。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-150">When you pass the HTML as a data-block, be sure there is no active content that would require user credentials, or a pre-loaded browser plug-in.</span></span> <span data-ttu-id="8f9a2-151">Microsoft Graph 用于将 HTML 页面呈现为图像的引擎无法登录用户，且不包含诸如 Adobe Flash、Apple QuickTime 等插件。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-151">The engine that Microsoft Graph uses to render the HTML page into an image has no ability to log in a user, and doesn't include plug-ins like Adobe Flash, Apple QuickTime, and so-on.</span></span> <span data-ttu-id="8f9a2-152">这也意味着，如果获取数据需要用户登录凭据或 Cookie，将不会显示动态加载的内容（如可能带有 AJAX 脚本）。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-152">That also means that dynamically-loaded content, like might come with an AJAX script, won't appear if getting the data requires user login credentials or cookies.</span></span>

<span data-ttu-id="8f9a2-153">在请求的**演示**部分的输入 HTML 中，包括 `<img data-render-src="name:part-name" />`，其中 *part-name* 是包含 HTML 的[多部分请求](onenote-create-page.md#example-request)中数据部分的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-153">In the input HTML of your request's **Presentation** part, include  `<img data-render-src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the HTML.</span></span>


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
<img src="http://cdn.onenote.net/1664161560_Images/OneNote.ico" />
</body>
</html>

--MyAppPartBoundary--  
```


<a name="image-object"></a>

### <a name="add-an-image-file-as-an-attachment"></a><span data-ttu-id="8f9a2-154">将图像文件添加为附件</span><span class="sxs-lookup"><span data-stu-id="8f9a2-154">Add an image file as an attachment</span></span>

<span data-ttu-id="8f9a2-155">在请求的**演示**部分的输入 HTML 中，包括 `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`，其中 *part-name* 是包含二进制图像数据的[多部分请求](onenote-create-page.md#example-request)中数据部分的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-155">In the input HTML of your request's **Presentation** part, include  `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="8f9a2-156">请只发送二进制数据，不要使用 Base64 或其他方式对其进行编码。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-156">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

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

<span data-ttu-id="8f9a2-157">了解有关[文件媒体类型](#file-media-types)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-157">Learn more about [file media types](#file-media-types).</span></span>



<a name="adding-videos"></a>

## <a name="adding-videos"></a><span data-ttu-id="8f9a2-158">添加视频</span><span class="sxs-lookup"><span data-stu-id="8f9a2-158">Adding videos</span></span>

<span data-ttu-id="8f9a2-159">可以在输入 HTML 中使用 `<iframe data-original-src="http://..." />` 在 OneNote 页面中嵌入视频。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-159">You can embed videos in OneNote pages using `<iframe data-original-src="http://..." />` in the input HTML.</span></span> 

### <a name="supported-video-sites"></a><span data-ttu-id="8f9a2-160">支持的视频网站</span><span class="sxs-lookup"><span data-stu-id="8f9a2-160">Supported video sites</span></span>

- <span data-ttu-id="8f9a2-161">Dailymotion</span><span class="sxs-lookup"><span data-stu-id="8f9a2-161">Dailymotion</span></span>
- <span data-ttu-id="8f9a2-162">Office Mix</span><span class="sxs-lookup"><span data-stu-id="8f9a2-162">Office Mix</span></span>
- <span data-ttu-id="8f9a2-163">Sway</span><span class="sxs-lookup"><span data-stu-id="8f9a2-163">Sway</span></span>
- <span data-ttu-id="8f9a2-164">Sketchfab</span><span class="sxs-lookup"><span data-stu-id="8f9a2-164">Sketchfab</span></span>
- <span data-ttu-id="8f9a2-165">TED</span><span class="sxs-lookup"><span data-stu-id="8f9a2-165">TED</span></span>
- <span data-ttu-id="8f9a2-166">YouTube</span><span class="sxs-lookup"><span data-stu-id="8f9a2-166">YouTube</span></span>
- <span data-ttu-id="8f9a2-167">Vimeo</span><span class="sxs-lookup"><span data-stu-id="8f9a2-167">Vimeo</span></span>
- <span data-ttu-id="8f9a2-168">Vine</span><span class="sxs-lookup"><span data-stu-id="8f9a2-168">Vine</span></span>

### <a name="iframe-attributes"></a><span data-ttu-id="8f9a2-169">iframe 属性</span><span class="sxs-lookup"><span data-stu-id="8f9a2-169">iframe attributes</span></span>

#### <a name="data-original-src"></a><span data-ttu-id="8f9a2-170">data-original-src</span><span class="sxs-lookup"><span data-stu-id="8f9a2-170">data-original-src</span></span>

<span data-ttu-id="8f9a2-171">必需。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-171">Required.</span></span> <span data-ttu-id="8f9a2-172">视频的 URL。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-172">The URL of the video.</span></span>

<span data-ttu-id="8f9a2-173">示例：`data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="8f9a2-173">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span>

#### <a name="width"></a><span data-ttu-id="8f9a2-174">width</span><span class="sxs-lookup"><span data-stu-id="8f9a2-174">width</span></span>

<span data-ttu-id="8f9a2-175">可选。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-175">Optional.</span></span> <span data-ttu-id="8f9a2-176">包含视频的 iframe 的宽度。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-176">The width of the iframe that contains the video.</span></span> <span data-ttu-id="8f9a2-177">默认值为 480。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-177">Default is 480.</span></span>

<span data-ttu-id="8f9a2-178">示例：`width="300"`</span><span class="sxs-lookup"><span data-stu-id="8f9a2-178">Example: `width="300"`</span></span>

#### <a name="height"></a><span data-ttu-id="8f9a2-179">height</span><span class="sxs-lookup"><span data-stu-id="8f9a2-179">height</span></span>

<span data-ttu-id="8f9a2-180">可选。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-180">Optional.</span></span> <span data-ttu-id="8f9a2-181">包含视频的 iframe 的高度。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-181">The height of the iframe that contains the video.</span></span> <span data-ttu-id="8f9a2-182">默认值为 360。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-182">Default is 360.</span></span>

<span data-ttu-id="8f9a2-183">示例：`height="300"`</span><span class="sxs-lookup"><span data-stu-id="8f9a2-183">Example: `height="300"`</span></span>

### <a name="example"></a><span data-ttu-id="8f9a2-184">示例</span><span class="sxs-lookup"><span data-stu-id="8f9a2-184">Example</span></span>

<span data-ttu-id="8f9a2-185">在请求的输入 HTML 中，包括 `<iframe data-original-src="http://..." />` 并为 **data-original-src** 属性指定视频的 URL。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-185">In the input HTML of your request, include `<iframe data-original-src="http://..." />` and specify the URL of the video for the **data-original-src** attribute.</span></span>

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

## <a name="adding-files"></a><span data-ttu-id="8f9a2-186">添加文件</span><span class="sxs-lookup"><span data-stu-id="8f9a2-186">Adding files</span></span>

<span data-ttu-id="8f9a2-187">可以在输入 HTML 中使用 **object** 对象元素将文件附件添加到 OneNote 页面。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-187">You can add file attachments to OneNote pages using an **object** element in the input HTML.</span></span> <span data-ttu-id="8f9a2-188">如果要添加 PDF 文件，则可以使用 **img** 元素将 PDF 元素页呈现为图像。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-188">If you're adding a PDF file, you can use an **img** element to render the PDF pages as images.</span></span> 

[<span data-ttu-id="8f9a2-189">添加文件附件</span><span class="sxs-lookup"><span data-stu-id="8f9a2-189">Add a file attachment</span></span>](#add-a-file-attachment)

<span data-ttu-id="8f9a2-190">使用 `<object .../>`，并发送多部分请求的数据部件中的文件。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-190">Use `<object .../>` and send the file in a data part of a multipart request.</span></span> <span data-ttu-id="8f9a2-191">添加在 OneNote 页面上显示文件图标的文件附件。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-191">Adds a file attachment that displays a file icon on the OneNote page.</span></span>

[<span data-ttu-id="8f9a2-192">添加 PDF 文件内容的图像</span><span class="sxs-lookup"><span data-stu-id="8f9a2-192">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)

<span data-ttu-id="8f9a2-193">使用 `<img data-render-src="name:part-name" />`，并发送多部分请求的数据部件中的 PDF 文件。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-193">Use `<img data-render-src="name:part-name" />` and send a PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="8f9a2-194">在 OneNote 页上将每个 PDF 页呈现为单独图像。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-194">Renders each PDF page as a separate image on the OneNote page.</span></span>

#### <a name="file-attributes"></a><span data-ttu-id="8f9a2-195">文件属性</span><span class="sxs-lookup"><span data-stu-id="8f9a2-195">File attributes</span></span>

<span data-ttu-id="8f9a2-196">**object** 元素需要下列属性。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-196">The **object** element requires the following attributes.</span></span>

<span data-ttu-id="8f9a2-197">**data-attachment**</span><span class="sxs-lookup"><span data-stu-id="8f9a2-197">**data-attachment**</span></span>

<span data-ttu-id="8f9a2-198">要在 OneNote 页面上显示的文件名和扩展名。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-198">The file name and extension to display on the OneNote page.</span></span>

<span data-ttu-id="8f9a2-199">示例：`data-attachment="filename.docx"`</span><span class="sxs-lookup"><span data-stu-id="8f9a2-199">Example: `data-attachment="filename.docx"`</span></span>

<span data-ttu-id="8f9a2-200">**data**</span><span class="sxs-lookup"><span data-stu-id="8f9a2-200">**data**</span></span>

<span data-ttu-id="8f9a2-201">包含二进制文件数据的多部分请求的正文部分的名称。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-201">The name of the body part in the multipart request that contains the binary file data.</span></span> <span data-ttu-id="8f9a2-202">Microsoft Graph 不支持在此处传递 URL 引用。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-202">Microsoft Graph does not support passing a URL reference here.</span></span>

<span data-ttu-id="8f9a2-203">示例：`data="name:part-name"`</span><span class="sxs-lookup"><span data-stu-id="8f9a2-203">Example: `data="name:part-name"`</span></span>

<span data-ttu-id="8f9a2-204">**type**</span><span class="sxs-lookup"><span data-stu-id="8f9a2-204">**type**</span></span>

<span data-ttu-id="8f9a2-205">文件媒体类型用于确定页面上使用的文件图标，同时还确定当用户从 OneNote 激活设备上的文件时，会启动哪个应用程序。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-205">The file media type, used to determine the file icon to use on the page, and which application starts when the user activates the file on the device from OneNote.</span></span>

<span data-ttu-id="8f9a2-206">示例：`type="application/pdf"`</span><span class="sxs-lookup"><span data-stu-id="8f9a2-206">Example: `type="application/pdf"`</span></span>


<a name="file-media-types"></a>

#### <a name="file-media-types"></a><span data-ttu-id="8f9a2-207">文件媒体类型</span><span class="sxs-lookup"><span data-stu-id="8f9a2-207">File media types</span></span>  

<span data-ttu-id="8f9a2-208">Microsoft Graph 为附加文件使用预定义的文件类型图标，当 API 不识别文件类型时，Microsoft Graph 会为其使用通用图标。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-208">Microsoft Graph uses predefined file-types icon for attached files, or a generic icon when the API doesn't recognize the file type.</span></span> <span data-ttu-id="8f9a2-209">下表显示了 API 可识别的一些常见文件类型。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-209">The following table shows some common file types that are recognized by the API.</span></span>

- <span data-ttu-id="8f9a2-210">application/pdf</span><span class="sxs-lookup"><span data-stu-id="8f9a2-210">application/pdf</span></span>  
- <span data-ttu-id="8f9a2-211">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span><span class="sxs-lookup"><span data-stu-id="8f9a2-211">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span></span>  
- <span data-ttu-id="8f9a2-212">application/vnd.openxmlformats-officedocument.presentationml.presentation</span><span class="sxs-lookup"><span data-stu-id="8f9a2-212">application/vnd.openxmlformats-officedocument.presentationml.presentation</span></span>
- <span data-ttu-id="8f9a2-213">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span><span class="sxs-lookup"><span data-stu-id="8f9a2-213">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span></span>
- <span data-ttu-id="8f9a2-214">image/png</span><span class="sxs-lookup"><span data-stu-id="8f9a2-214">image/png</span></span>
- <span data-ttu-id="8f9a2-215">image/jpeg</span><span class="sxs-lookup"><span data-stu-id="8f9a2-215">image/jpeg</span></span>
- <span data-ttu-id="8f9a2-216">image/gif</span><span class="sxs-lookup"><span data-stu-id="8f9a2-216">image/gif</span></span>
- <span data-ttu-id="8f9a2-217">audio/wav</span><span class="sxs-lookup"><span data-stu-id="8f9a2-217">audio/wav</span></span>
- <span data-ttu-id="8f9a2-218">video/mp4</span><span class="sxs-lookup"><span data-stu-id="8f9a2-218">video/mp4</span></span>
- <span data-ttu-id="8f9a2-219">application/msword</span><span class="sxs-lookup"><span data-stu-id="8f9a2-219">application/msword</span></span>
- <span data-ttu-id="8f9a2-220">application/mspowerpoint</span><span class="sxs-lookup"><span data-stu-id="8f9a2-220">application/mspowerpoint</span></span>
- <span data-ttu-id="8f9a2-221">application/excel</span><span class="sxs-lookup"><span data-stu-id="8f9a2-221">application/excel</span></span>

<span data-ttu-id="8f9a2-222">请参阅创建包含媒体的页面时应用的[限制](#size-limitations-for-post-pages-requests)。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-222">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="file-object"></a>

### <a name="add-a-file-attachment"></a><span data-ttu-id="8f9a2-223">添加文件附件</span><span class="sxs-lookup"><span data-stu-id="8f9a2-223">Add a file attachment</span></span>

<span data-ttu-id="8f9a2-224">在请求的**演示**部分的输入 HTML 中，包括 `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`，其中 *part-name* 是包含二进制文件数据的[多部分请求](onenote-create-page.md#example-request)中的数据部分的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-224">In the input HTML of your request's **Presentation** part, include  `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="8f9a2-225">请只发送二进制数据，不要使用 Base64 或其他方式对其进行编码。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-225">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

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

### <a name="add-images-of-pdf-file-contents"></a><span data-ttu-id="8f9a2-226">添加 PDF 文件内容的图像</span><span class="sxs-lookup"><span data-stu-id="8f9a2-226">Add images of PDF file contents</span></span>

<span data-ttu-id="8f9a2-227">在请求的**演示**部分的输入 HTML 中，包括 `<img data-render-src="name:part-name" ... />`，其中 *part-name* 是包含二进制文件数据的[多部分请求](onenote-create-page.md#example-request)中的数据部分的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-227">In the input HTML of your request's **Presentation** part, include  `<img data-render-src="name:part-name" ... />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="8f9a2-228">请只发送二进制数据，不要使用 Base64 或其他方式对其进行编码。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-228">Just send the binary data, don't use Base64 or otherwise encode it.</span></span>

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

## <a name="size-limitations-for-post-pages-requests"></a><span data-ttu-id="8f9a2-229">POST 页面请求的大小限制</span><span class="sxs-lookup"><span data-stu-id="8f9a2-229">Size limitations for POST pages requests</span></span>

<span data-ttu-id="8f9a2-230">发送图像和文件数据时，应注意以下限制：<!--TODO: check these--></span><span class="sxs-lookup"><span data-stu-id="8f9a2-230">When sending image and file data, be aware of these limitations: <!--TODO: check these--></span></span>

- <span data-ttu-id="8f9a2-231">POST 的总大小限制为 ~ 70 MB，包括图像、文件和其他数据。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-231">The total POST size limit is ~70 MB, including images, files, and other data.</span></span> <span data-ttu-id="8f9a2-232">实际限制会受下游编码的影响，因此没有固定的字节计数限制。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-232">The actual limit is affected by downstream encoding, so there's no fixed byte-count limit.</span></span> <span data-ttu-id="8f9a2-233">超过此限制的请求可能会产生不可靠的结果。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-233">Requests that exceed the limit may produce unreliable results.</span></span>

- <span data-ttu-id="8f9a2-234">每个数据部件限制为 25 MB，包括部件标头。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-234">The limit for each data part is 25 MB, including the part headers.</span></span> <span data-ttu-id="8f9a2-235">Microsoft Graph 将拒绝超过此限制的数据部件。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-235">Data parts that exceed the limit are rejected by Microsoft Graph.</span></span> 

- <span data-ttu-id="8f9a2-236">每个页面的最大图像数为 150。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-236">The maximum number of images per page is 150.</span></span> <span data-ttu-id="8f9a2-237">使用 `src="http://..."` 属性时，API 将忽略超出此限制的 **img** 标记。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-237">When using the `src="http://..."` attribute, the API ignores **img** tags beyond the limit.</span></span>

- <span data-ttu-id="8f9a2-238">数据部件的最大数量是每个 POST 6 个，包括必需的 **Presentation** 部件。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-238">The maximum number of data parts is 6 per POST, including the required **Presentation** part.</span></span>

- <span data-ttu-id="8f9a2-239">每个请求可以包含最多 5 个使用 **data-render-src** 的 **img** 元素和一个使用 **data-render-src** 的 **object** 元素。其他图像和文件引用将被忽略。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-239">Each request can contain up to five **img** elements that use **data-render-src** and one **object** elements that uses **data-render-src**. Additional image and file references are ignored.</span></span>

- <span data-ttu-id="8f9a2-240">无论使用哪种方法将图像发送到 API，单个 POST 中图像的最大数量都是 30 个。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-240">The maximum number of images in a single POST is 30, no matter which method you use to send them to the API.</span></span> <span data-ttu-id="8f9a2-241">其他图像将被忽略。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-241">Additional images are ignored.</span></span> <span data-ttu-id="8f9a2-242">如果想要捕获包含大量图像的网页，请考虑[捕获整个页面作为快照](#add-a-webpage-snapshot)。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-242">If you want to capture a webpage that contains a lot of images, consider [capturing the whole page as a snapshot](#add-a-webpage-snapshot).</span></span>


## <a name="when-to-use-html-versus-data-render-src"></a><span data-ttu-id="8f9a2-243">何时将 HTML 与 data-render-src 结合使用</span><span class="sxs-lookup"><span data-stu-id="8f9a2-243">When to use HTML versus data-render-src</span></span> 

<span data-ttu-id="8f9a2-244">尝试在直接将 HTML 置于 OneNote 页面与使用 **data-render-src** 属性之间选择时，请考虑以下情况：</span><span class="sxs-lookup"><span data-stu-id="8f9a2-244">When trying to decide between putting HTML directly onto the OneNote page instead of using the **data-render-src** attribute, consider the following:</span></span>

- <span data-ttu-id="8f9a2-245">最好通过 **data-render-src** 发送复杂 HTML 来呈现引擎，而不是尝试修改 HTML 来使其符合 Microsoft Graph 的要求。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-245">Complex HTML is probably best sent to the rendering engine via **data-render-src**, rather than attempting to modify the HTML to fit into what Microsoft Graph can accept.</span></span> <span data-ttu-id="8f9a2-246">此外，当 HTML 包含不支持的标记时，这也是如此。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-246">This is also true when your HTML includes tags that aren't supported supported.</span></span>

- <span data-ttu-id="8f9a2-247">精确页面呈现，以保留页面布局和外观时，最好是通过 **data-render-src** 使用呈现引擎完成。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-247">Accurate page rendering to preserve the layout and look of the page is probably best done with the rendering engine via **data-render-src**.</span></span>

- <span data-ttu-id="8f9a2-p130">直接可编辑文本，实现时通常需要将 HTML 直接插入页面。呈现的图像由光学字符识别 (OCR) 系统进行扫描，但会有所不同。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-p130">Directly-editable text is often best done with inserting the HTML directly onto the page. The rendered images are scanned by an optical character recognition (OCR) system, but it's just not the same.</span></span>

- <span data-ttu-id="8f9a2-250">用于历史记录或存档目的的实时快照最好使用 **data-render-src** 方法来捕获。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-250">Snapshot-in-time for historical or archival purposes is usually best done with the data-render-src method.</span></span>

- <span data-ttu-id="8f9a2-p131">标记网页设计以便于修订，是 **data-render-src** 的亮点所在。您可以使用 OneNote 的墨迹书写功能在图像上绘图，以指示更改或标出重要区域。将网页处理为图像可大大简化该过程。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-p131">Marking-up a web page design for revisions is one place the **data-render-src** truly shines. Using OneNote's inking capabilities, you can draw on the image to indicate changes or call out important areas. Having the web page as an image makes that a lot easier.</span></span>

- <span data-ttu-id="8f9a2-254">对于很大的图像或格式不是 OneNote 可直接接受的图像，有时可以生成缩略图，与在自己的代码中进行图像转换相比，使用 **data-render-src** 属性转换更为容易。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-254">Very large images, or images in formats that OneNote doesn't directly accept can sometimes be thumbnailed and converted with the **data-render-src** attribure more easily than by doing it in your own code.</span></span> <span data-ttu-id="8f9a2-255">虽然图像也可以在线使用，但通过减少生成 OneNote 页所需的往返总次数，将数据嵌入到 POST 中，有时可以使 OneNote 用户更快地使用捕获到的页面。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-255">Even if the image is also available onlinet, embedding the data in your POST can sometimes make the captured page available to OneNote user sooner, by reducing the total number of round-trips needed to build the OneNote page.</span></span>

<span data-ttu-id="8f9a2-256">有时，确定哪种方法最适合用户的最佳方法是在开发应用时尝试这两种方法。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-256">Sometimes, the best way to determine which method will work best for your users is to try it both ways as you develop your app.</span></span>


<a name="permissions"></a>

## <a name="permissions"></a><span data-ttu-id="8f9a2-257">权限</span><span class="sxs-lookup"><span data-stu-id="8f9a2-257">Permissions</span></span>

<span data-ttu-id="8f9a2-258">若要创建或更新 OneNote 页面，需要请求相应的权限。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-258">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="8f9a2-259">选择应用正常运行所需的最低级别。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-259">Choose the lowest level that your app needs to do its work.</span></span>

#### <a name="permissions-for-post-pages"></a><span data-ttu-id="8f9a2-260">POST 页面的权限</span><span class="sxs-lookup"><span data-stu-id="8f9a2-260">Permissions for POST pages</span></span>

- <span data-ttu-id="8f9a2-261">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="8f9a2-261">Notes.Create</span></span>
- <span data-ttu-id="8f9a2-262">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f9a2-262">Notes.ReadWrite</span></span>
- <span data-ttu-id="8f9a2-263">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f9a2-263">Notes.ReadWrite.All</span></span> 

#### <a name="permissions-for-patch-pages"></a><span data-ttu-id="8f9a2-264">PATCH 页面的权限</span><span class="sxs-lookup"><span data-stu-id="8f9a2-264">Permissions for PATCH pages</span></span>

- <span data-ttu-id="8f9a2-265">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8f9a2-265">Notes.ReadWrite</span></span>
- <span data-ttu-id="8f9a2-266">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f9a2-266">Notes.ReadWrite.All</span></span>

<span data-ttu-id="8f9a2-267">有关权限范围及其工作方式的详细信息，请参阅 [OneNote 权限范围](permissions_reference.md#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="8f9a2-267">For more information about permission scopes and how they work, see [OneNote permission scopes](permissions_reference.md#notes-permissions).</span></span>


<a name="see-also"></a>

## <a name="see-also"></a><span data-ttu-id="8f9a2-268">另请参阅</span><span class="sxs-lookup"><span data-stu-id="8f9a2-268">See also</span></span>

- [<span data-ttu-id="8f9a2-269">与 OneNote 集成</span><span class="sxs-lookup"><span data-stu-id="8f9a2-269">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="8f9a2-270">OneNote 开发者博客</span><span class="sxs-lookup"><span data-stu-id="8f9a2-270">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="8f9a2-271">关于 Stack Overflow 的 OneNote 开发问题</span><span class="sxs-lookup"><span data-stu-id="8f9a2-271">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="8f9a2-272">OneNote GitHub 存储库</span><span class="sxs-lookup"><span data-stu-id="8f9a2-272">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
