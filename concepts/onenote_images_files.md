
# <a name="add-images-videos-and-files-to-onenote-pages"></a><span data-ttu-id="d64e6-101">将图像、视频和文件添加到 OneNote 页面</span><span class="sxs-lookup"><span data-stu-id="d64e6-101">Add images, videos, and files to OneNote pages</span></span>

<span data-ttu-id="d64e6-102">*__适用于：__ OneDrive 上的消费者笔记本 | Office 365 上的企业级笔记本*</span><span class="sxs-lookup"><span data-stu-id="d64e6-102">*__Applies to:__ Consumer notebooks on OneDrive | Enterprise notebooks on Office 365*</span></span>

<span data-ttu-id="d64e6-103">在[创建](onenote-create-page.md)或[更新](onenote_update_page.md)页面时，可以使用 **img**、**object** 和 **iframe** 元素将图像、视频和文件添加到 OneNote 页面。</span><span class="sxs-lookup"><span data-stu-id="d64e6-103">You can use **img**, **object**, and **iframe** elements to add images, videos, and files to a OneNote page when you're [creating](onenote-create-page.md) or [updating](onenote_update_page.md) the page.</span></span> 

- <span data-ttu-id="d64e6-104">使用 **img** 在页面上呈现图像。</span><span class="sxs-lookup"><span data-stu-id="d64e6-104">Use **img** to render an image on the page.</span></span>
- <span data-ttu-id="d64e6-105">使用 **iframe** 在页面上嵌入视频。</span><span class="sxs-lookup"><span data-stu-id="d64e6-105">Use **iframe** to embed a video on the page.</span></span>
- <span data-ttu-id="d64e6-106">使用 **object** 将文件附件添加到页面。</span><span class="sxs-lookup"><span data-stu-id="d64e6-106">Use **object** to add a file attachment to the page.</span></span>


<a name="images"></a>
## <a name="adding-images"></a><span data-ttu-id="d64e6-107">添加图像</span><span class="sxs-lookup"><span data-stu-id="d64e6-107">Adding images</span></span>

<span data-ttu-id="d64e6-108">图像可以通过 URL 引用或发送原始数据来进行添加。</span><span class="sxs-lookup"><span data-stu-id="d64e6-108">Images can be added by URL reference or by sending raw data.</span></span> <span data-ttu-id="d64e6-109">Microsoft Graph 支持以下可将图像、徽标和照片添加到 OneNote 页面的方法。</span><span class="sxs-lookup"><span data-stu-id="d64e6-109">Microsoft Graph supports the following methods of adding images, logos, and photos to OneNote pages.</span></span> 

[<span data-ttu-id="d64e6-110">从 Web 添加公共图像</span><span class="sxs-lookup"><span data-stu-id="d64e6-110">Add a public image from the web</span></span>](#add-a-public-image-from-the-web)  
<span data-ttu-id="d64e6-111">将 `img` 与 `src="http://image-url"` 结合使用，并指定可公开访问图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="d64e6-111">Use `img` with `src="http://image-url"` and specify the URL of a publicly accessible image.</span></span> <span data-ttu-id="d64e6-112">在 OneNote 页面上呈现图像。</span><span class="sxs-lookup"><span data-stu-id="d64e6-112">Renders the image on the OneNote page.</span></span></p>
[<span data-ttu-id="d64e6-113">使用二进制数据添加图像</span><span class="sxs-lookup"><span data-stu-id="d64e6-113">Add an image using binary data</span></span>](#add-an-image-using-binary-data)</p>
<span data-ttu-id="d64e6-114">将 `img` 与 `src="name:image-block-name"` 结合使用，并发送多部分请求的数据部件中的图像文件。</span><span class="sxs-lookup"><span data-stu-id="d64e6-114">Use `img` with `src="name:image-block-name"` and send the image file in a data part of a multipart request.</span></span> <span data-ttu-id="d64e6-115">在 OneNote 页面上呈现图像。</span><span class="sxs-lookup"><span data-stu-id="d64e6-115">Renders the image on the OneNote page.</span></span></p>
[<span data-ttu-id="d64e6-116">添加网页快照</span><span class="sxs-lookup"><span data-stu-id="d64e6-116">Add a webpage snapshot</span></span>](#add-a-webpage-snapshot)</p>
<span data-ttu-id="d64e6-117">将 `img` 与 `data-render-src="http://webpage-url"` 结合使用，并指定网页的 URL。</span><span class="sxs-lookup"><span data-stu-id="d64e6-117">Use `img` with `data-render-src="http://webpage-url"` and specify the URL of a webpage.</span></span> <span data-ttu-id="d64e6-118">在 OneNote 页面上呈现整个网页的快照。</span><span class="sxs-lookup"><span data-stu-id="d64e6-118">Renders a snapshot of the whole webpage on the OneNote page.</span></span></p>
[<span data-ttu-id="d64e6-119">添加从 HTML 呈现的图像</span><span class="sxs-lookup"><span data-stu-id="d64e6-119">Add an image rendered from HTML</span></span>](#add-an-image-rendered-from-html)</p>
<span data-ttu-id="d64e6-120">将 `img` 与 `data-render-src="name:html-block-name"` 结合使用，并发送多部分请求的数据部件中的 HTML。</span><span class="sxs-lookup"><span data-stu-id="d64e6-120">Use `img` with `data-render-src="name:html-block-name"` and send HTML in the data part of a multipart request.</span></span> <span data-ttu-id="d64e6-121">在 OneNote 页面上将 HTML 呈现为图像。</span><span class="sxs-lookup"><span data-stu-id="d64e6-121">Renders the HTML as an image on the OneNote page.</span></span></p>
[<span data-ttu-id="d64e6-122">添加 PDF 文件内容的图像</span><span class="sxs-lookup"><span data-stu-id="d64e6-122">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)</p>
<span data-ttu-id="d64e6-123">使用 `<img data-render-src="name:part-name" />`，并发送多部分请求的数据部件中的 PDF 文件。</span><span class="sxs-lookup"><span data-stu-id="d64e6-123">Use `<img data-render-src="name:part-name" />` and send the PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="d64e6-124">在 OneNote 页面上将每个 PDF 页面呈现为单独图像。</span><span class="sxs-lookup"><span data-stu-id="d64e6-124">Renders each PDF page as a separate image on the OneNote page.</span></span></p>
[<span data-ttu-id="d64e6-125">将图像文件添加为文件附件</span><span class="sxs-lookup"><span data-stu-id="d64e6-125">Add an image file as a file attachment</span></span>](#add-an-image-file-as-an-attachment)</p>
<span data-ttu-id="d64e6-126">将 `object` 与 `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` 结合使用，并发送多部分请求的数据部件中的图像文件。</span><span class="sxs-lookup"><span data-stu-id="d64e6-126">Use `object` with `data="name:file-block-name" data-attachment="file-name.file-ext" type="media-type"` and send an image file in the data part of a multipart request.</span></span> <span data-ttu-id="d64e6-127">将文件附件添加到 OneNote 页面，并显示文件图标。</span><span class="sxs-lookup"><span data-stu-id="d64e6-127">Adds a file attachment to the OneNote page and displays a file icon.</span></span></p>

> <span data-ttu-id="d64e6-128">**注意：** 若要获取 OneNote 页面上的图像，首先发送 [GET 请求获取页面内容](onenote-get-content.md#page-html-content)。</span><span class="sxs-lookup"><span data-stu-id="d64e6-128">**Note:** To get images on a OneNote page, first send a [GET request for the page content](onenote-get-content.md#page-html-content).</span></span> <span data-ttu-id="d64e6-129">这会将 URL 返回到页面上的图像资源。</span><span class="sxs-lookup"><span data-stu-id="d64e6-129">This returns the URLs to the image resources on the page.</span></span> <span data-ttu-id="d64e6-130">然后，将 [GET 请求与图像资源分开](onenote-get-content.md#image-or-other-file-resource)。</span><span class="sxs-lookup"><span data-stu-id="d64e6-130">Then you separate [GET requests to the image resources](onenote-get-content.md#image-or-other-file-resource).</span></span>


<span data-ttu-id="d64e6-131">**图像属性**</span><span class="sxs-lookup"><span data-stu-id="d64e6-131">**Image attributes**</span></span> 

<span data-ttu-id="d64e6-132">**img** 元素可以选择包括 **alt**、**height** 和 **width** 属性，以及样式属性 **max-width** 和 **max-height**。</span><span class="sxs-lookup"><span data-stu-id="d64e6-132">An **img** element can optionally include **alt**, **height**, and **width** attributes, and the style attributes **max-width** and **max-height**.</span></span>

<span data-ttu-id="d64e6-133">**图像媒体类型**</span><span class="sxs-lookup"><span data-stu-id="d64e6-133">**Image media types**</span></span>

<span data-ttu-id="d64e6-134">Microsoft Graph 支持 TIFF、PNG、GIF、JPEG 和 BMP 图像类型。</span><span class="sxs-lookup"><span data-stu-id="d64e6-134">Microsoft Graph supports TIFF, PNG, GIF, JPEG, and BMP image types.</span></span> <span data-ttu-id="d64e6-135">若要捕获使用不想转换的其他格式的图像，请在多部分请求中[发送二进制数据](#add-an-image-using-binary-data)。</span><span class="sxs-lookup"><span data-stu-id="d64e6-135">To capture an image that uses a different format that you don't want to convert, [send the binary data](#add-an-image-using-binary-data) in a multipart request.</span></span> <span data-ttu-id="d64e6-136">不需要使用 Base64，或其他方式对发送的二进制数据进行编码。</span><span class="sxs-lookup"><span data-stu-id="d64e6-136">You don't need to use Base64 or otherwise encode the binary data that you send.</span></span>

> <span data-ttu-id="d64e6-137">**注意：** API 会检测原始输入图像类型，并在[输出 HTML](onenote_input_output_html.md#output-html) 中将其作为 **data-fullres-src-type** 属性返回。</span><span class="sxs-lookup"><span data-stu-id="d64e6-137">**Note:** The OneNote APIs automatically detect the input image type, and returns it as the **data-fullres-src-type** in the output HTML.</span></span> <span data-ttu-id="d64e6-138">此外，API 还会在 **data-src-type** 中返回优化图像的图像类型。</span><span class="sxs-lookup"><span data-stu-id="d64e6-138">The API also returns the image type of the optimized image in **data-src-type**.</span></span>
 
<span data-ttu-id="d64e6-139">请参阅创建包含媒体的页面时应用的[限制](#size-limitations-for-post-pages-requests)。</span><span class="sxs-lookup"><span data-stu-id="d64e6-139">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="image-img-url-src"></a>
### <a name="add-a-public-image-from-the-web"></a><span data-ttu-id="d64e6-140">从 Web 添加公共图像</span><span class="sxs-lookup"><span data-stu-id="d64e6-140">Add a public image from the web</span></span>

<span data-ttu-id="d64e6-141">在请求的输入 HTML 中，包括 `<img src="http://..." />` 并为 **src** 属性指定可公开访问图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="d64e6-141">In the input HTML of your request, include  `<img src="http://..." />` and specify the URL of a publicly accessible image for the **src** attribute.</span></span>

```
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
### <a name="add-an-image-using-binary-data"></a><span data-ttu-id="d64e6-142">使用二进制数据添加图像</span><span class="sxs-lookup"><span data-stu-id="d64e6-142">Add an image using binary data</span></span>

<span data-ttu-id="d64e6-143">在请求的 **Presentation** 部件的输入 HTML 中，包括 `<img src="name:part-name" />`，其中 *part-name* 是包含二进制图像数据的[多部分请求](onenote-create-page.md#example-request)中数据部件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d64e6-143">In the input HTML of your request's **Presentation** part, include  `<img src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="d64e6-144">请只发送二进制数据，不要使用 Base64 或其他方式对其进行编码。</span><span class="sxs-lookup"><span data-stu-id="d64e6-144">The image data is the binary file data; don't use Base64 or otherwise encode it.</span></span>

```
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
### <a name="add-a-webpage-snapshot"></a><span data-ttu-id="d64e6-145">添加网页快照</span><span class="sxs-lookup"><span data-stu-id="d64e6-145">Add a webpage snapshot</span></span>

<span data-ttu-id="d64e6-146">可以使用 Microsoft Graph 截取整个网页的快照，并将其插入到新页面中。</span><span class="sxs-lookup"><span data-stu-id="d64e6-146">You can use Microsoft Graph to snapshot entire webpages and insert them into new pages.</span></span> <span data-ttu-id="d64e6-147">此方法对存档网页或捕获具有 OneNote 不支持的功能（如某些 CSS）的复杂网页很有用。</span><span class="sxs-lookup"><span data-stu-id="d64e6-147">This method is useful to archive webpages or capture complex webpages that have features that OneNote doesn't support (like some CSS).</span></span>  

<span data-ttu-id="d64e6-148">在请求的输入 HTML 中，包括 `<img src="http://..." />` 并指定要为 **src** 属性插入的网页的 URL。</span><span class="sxs-lookup"><span data-stu-id="d64e6-148">In the input HTML of your request, include  `<img src="http://..." />` and specify the URL of the webpage you want to insert for the **src** attribute.</span></span>

```
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
### <a name="add-an-image-rendered-from-html"></a><span data-ttu-id="d64e6-149">添加从 HTML 呈现的图像</span><span class="sxs-lookup"><span data-stu-id="d64e6-149">Add an image rendered from HTML</span></span>
<span data-ttu-id="d64e6-150">将 HTML 作为数据块传递时，请确保没有需要用户凭据或预加载浏览器插件的活动内容。</span><span class="sxs-lookup"><span data-stu-id="d64e6-150">When you pass the HTML as a data-block, be sure there is no active content that would require user credentials, or a pre-loaded browser plug-in.</span></span> <span data-ttu-id="d64e6-151">Microsoft Graph 用于将 HTML 页面呈现为图像的引擎无法登录用户，且不包含诸如 Adobe Flash、Apple QuickTime 等插件。</span><span class="sxs-lookup"><span data-stu-id="d64e6-151">The engine that Microsoft Graph uses to render the HTML page into an image has no ability to log in a user, and doesn't include plug-ins like Adobe Flash, Apple QuickTime, and so-on.</span></span> <span data-ttu-id="d64e6-152">这也意味着，如果获取需要用户登录凭据或 Cookie 的数据，则动态加载的内容（如可能带有 AJAX 脚本）将不会显示。</span><span class="sxs-lookup"><span data-stu-id="d64e6-152">That also means that dynamically-loaded content, like might come with an AJAX script, won't appear if getting the data requires user login credentials or cookies.</span></span>

<span data-ttu-id="d64e6-153">在请求的 **Presentation** 部件的输入 HTML 中，包括 `<img data-render-src="name:part-name" />`，其中 *part-name* 是包含 HTML 的[多部分请求](onenote-create-page.md#example-request)中数据部件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d64e6-153">In the input HTML of your request's **Presentation** part, include  `<img data-render-src="name:part-name" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the HTML.</span></span>

```
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
### <a name="add-an-image-file-as-an-attachment"></a><span data-ttu-id="d64e6-154">将图像文件添加为附件</span><span class="sxs-lookup"><span data-stu-id="d64e6-154">Add an image file as an attachment</span></span>

<span data-ttu-id="d64e6-155">在请求的 **Presentation** 部件的输入 HTML 中，包括 `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`，其中 *part-name* 是包含二进制图像数据的[多部分请求](onenote-create-page.md#example-request)中数据部件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d64e6-155">In the input HTML of your request's **Presentation** part, include  `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary image data.</span></span> <span data-ttu-id="d64e6-156">请只发送二进制数据，不要使用 Base64 或其他方式对其进行编码。</span><span class="sxs-lookup"><span data-stu-id="d64e6-156">The image data is the binary file data; don't use Base64 or otherwise encode it.</span></span>

```
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

<span data-ttu-id="d64e6-157">了解有关[文件媒体类型](#file-media-types)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d64e6-157">Learn more about [file media types](#file-media-types).</span></span>



<a name="videos"></a>
## <a name="adding-videos"></a><span data-ttu-id="d64e6-158">添加视频</span><span class="sxs-lookup"><span data-stu-id="d64e6-158">Adding videos</span></span>

<span data-ttu-id="d64e6-159">可以在输入 HTML 中使用 `<iframe data-original-src="http://..." />` 在 OneNote 页面中嵌入视频。</span><span class="sxs-lookup"><span data-stu-id="d64e6-159">You can embed videos in OneNote pages using `<iframe data-original-src="http://..." />` in the input HTML.</span></span> 

<span data-ttu-id="d64e6-160">**支持的视频网站**</span><span class="sxs-lookup"><span data-stu-id="d64e6-160">**Supported video sites**</span></span>

- <span data-ttu-id="d64e6-161">Dailymotion</span><span class="sxs-lookup"><span data-stu-id="d64e6-161">Dailymotion</span></span>
- <span data-ttu-id="d64e6-162">Office Mix</span><span class="sxs-lookup"><span data-stu-id="d64e6-162">Office Mix</span></span>
- <span data-ttu-id="d64e6-163">Sway</span><span class="sxs-lookup"><span data-stu-id="d64e6-163">Sway</span></span>
- <span data-ttu-id="d64e6-164">Sketchfab</span><span class="sxs-lookup"><span data-stu-id="d64e6-164">Sketchfab</span></span>
- <span data-ttu-id="d64e6-165">TED</span><span class="sxs-lookup"><span data-stu-id="d64e6-165">TED</span></span>
- <span data-ttu-id="d64e6-166">YouTube</span><span class="sxs-lookup"><span data-stu-id="d64e6-166">YouTube</span></span>
- <span data-ttu-id="d64e6-167">Vimeo</span><span class="sxs-lookup"><span data-stu-id="d64e6-167">Vimeo</span></span>
- <span data-ttu-id="d64e6-168">Vine</span><span class="sxs-lookup"><span data-stu-id="d64e6-168">Vine</span></span>

<span data-ttu-id="d64e6-169">**iframe 属性**</span><span class="sxs-lookup"><span data-stu-id="d64e6-169">**iframe attributes**</span></span>

<span data-ttu-id="d64e6-170">**data-original-src**</span><span class="sxs-lookup"><span data-stu-id="d64e6-170">**data-original-src**</span></span></p>
<span data-ttu-id="d64e6-171">必需。</span><span class="sxs-lookup"><span data-stu-id="d64e6-171">Required.</span></span> <span data-ttu-id="d64e6-172">视频的 URL。</span><span class="sxs-lookup"><span data-stu-id="d64e6-172">The URL of the video source.</span></span><br /><span data-ttu-id="d64e6-173">示例：`data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span><span class="sxs-lookup"><span data-stu-id="d64e6-173">Example: `data-original-src="https://www.youtube.com/watch?v=3Ztr44aKmQ8"`</span></span></p>
<span data-ttu-id="d64e6-174">**width**</span><span class="sxs-lookup"><span data-stu-id="d64e6-174">**width**</span></span></p>
<span data-ttu-id="d64e6-175">可选。</span><span class="sxs-lookup"><span data-stu-id="d64e6-175">Optional.</span></span> <span data-ttu-id="d64e6-176">包含视频的 iframe 的宽度。</span><span class="sxs-lookup"><span data-stu-id="d64e6-176">The width of the iframe that contains the video.</span></span> <span data-ttu-id="d64e6-177">默认值为 480。</span><span class="sxs-lookup"><span data-stu-id="d64e6-177">Default is 480.</span></span><br /><span data-ttu-id="d64e6-178">示例：`width="300"`</span><span class="sxs-lookup"><span data-stu-id="d64e6-178">Example: `width="300"`</span></span></p>
<span data-ttu-id="d64e6-179">**height**</span><span class="sxs-lookup"><span data-stu-id="d64e6-179">**height**</span></span></p>
<span data-ttu-id="d64e6-180">可选。</span><span class="sxs-lookup"><span data-stu-id="d64e6-180">Optional.</span></span> <span data-ttu-id="d64e6-181">包含视频的 iframe 的高度。</span><span class="sxs-lookup"><span data-stu-id="d64e6-181">The height of the iframe that contains the video.</span></span> <span data-ttu-id="d64e6-182">默认值为 360。</span><span class="sxs-lookup"><span data-stu-id="d64e6-182">Default is 360.</span></span><br /><span data-ttu-id="d64e6-183">示例：`height="300"`</span><span class="sxs-lookup"><span data-stu-id="d64e6-183">Example: `height="300"`</span></span></p>

<span data-ttu-id="d64e6-184">**示例**</span><span class="sxs-lookup"><span data-stu-id="d64e6-184">**Example**</span></span>

<span data-ttu-id="d64e6-185">在请求的输入 HTML 中，包括 `<iframe data-original-src="http://..." />` 并为 **data-original-src** 属性指定视频的 URL。</span><span class="sxs-lookup"><span data-stu-id="d64e6-185">In the input HTML of your request, include `<iframe data-original-src="http://..." />` and specify the URL of the video for the **data-original-src** attribute.</span></span>

```
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


<a name="files"></a>
## <a name="adding-files"></a><span data-ttu-id="d64e6-186">添加文件</span><span class="sxs-lookup"><span data-stu-id="d64e6-186">Adding installation files</span></span>

<span data-ttu-id="d64e6-187">可以在输入 HTML 中使用 **object** 对象元素将文件附件添加到 OneNote 页面。</span><span class="sxs-lookup"><span data-stu-id="d64e6-187">You can add file attachments to OneNote pages using an **object** element in the input HTML.</span></span> <span data-ttu-id="d64e6-188">如果要添加 PDF 文件，则可以使用 **img** 元素将 PDF 元素页呈现为图像。</span><span class="sxs-lookup"><span data-stu-id="d64e6-188">If you're adding a PDF file, you can use an **img** element to render the PDF pages as images.</span></span> 

[<span data-ttu-id="d64e6-189">添加文件附件</span><span class="sxs-lookup"><span data-stu-id="d64e6-189">Add a file attachment</span></span>](#add-a-file-attachment)</p>
<span data-ttu-id="d64e6-190">使用 `<object .../>`，并发送多部分请求的数据部件中的文件。</span><span class="sxs-lookup"><span data-stu-id="d64e6-190">Use `<object .../>` and send the file in a data part of a multipart request.</span></span> <span data-ttu-id="d64e6-191">添加在 OneNote 页面上显示文件图标的文件附件。</span><span class="sxs-lookup"><span data-stu-id="d64e6-191">Adds a file attachment that displays a file icon on the OneNote page.</span></span></p>
[<span data-ttu-id="d64e6-192">添加 PDF 文件内容的图像</span><span class="sxs-lookup"><span data-stu-id="d64e6-192">Add images of PDF file contents</span></span>](#add-images-of-pdf-file-contents)</p>
<span data-ttu-id="d64e6-193">使用 `<img data-render-src="name:part-name" />`，并发送多部分请求的数据部件中的 PDF 文件。</span><span class="sxs-lookup"><span data-stu-id="d64e6-193">Use `<img data-render-src="name:part-name" />` and send a PDF file in the data part of a multipart request.</span></span> <span data-ttu-id="d64e6-194">在 OneNote 页面上将每个 PDF 页面呈现为单独图像。</span><span class="sxs-lookup"><span data-stu-id="d64e6-194">Renders each PDF page as a separate image on the OneNote page.</span></span></p>

<span data-ttu-id="d64e6-195">**文件属性**</span><span class="sxs-lookup"><span data-stu-id="d64e6-195">**File attributes**</span></span>

<span data-ttu-id="d64e6-196">**object** 元素需要下列属性。</span><span class="sxs-lookup"><span data-stu-id="d64e6-196">The **object** element requires the following attributes.</span></span>

<span data-ttu-id="d64e6-197">**data-attachment**</span><span class="sxs-lookup"><span data-stu-id="d64e6-197">**data-attachment**</span></span></p>
<span data-ttu-id="d64e6-198">要在 OneNote 页面上显示的文件名和扩展名。</span><span class="sxs-lookup"><span data-stu-id="d64e6-198">The file name and extension to display on the OneNote page.</span></span><br /><span data-ttu-id="d64e6-199">示例：`data-attachment="filename.docx"`</span><span class="sxs-lookup"><span data-stu-id="d64e6-199">Example: `data-attachment="filename.docx"`</span></span></p>
<span data-ttu-id="d64e6-200">**data**</span><span class="sxs-lookup"><span data-stu-id="d64e6-200">**Data**</span></span></p>
<span data-ttu-id="d64e6-201">包含二进制文件数据的多部分请求的正文部分的名称。</span><span class="sxs-lookup"><span data-stu-id="d64e6-201">The name of the body part in the multipart request that contains the binary file data.</span></span> <span data-ttu-id="d64e6-202">Microsoft Graph 不支持在此处传递 URL 引用。</span><span class="sxs-lookup"><span data-stu-id="d64e6-202">Microsoft Graph does not support passing a URL reference here.</span></span><br /><span data-ttu-id="d64e6-203">示例：`data="name:part-name"`</span><span class="sxs-lookup"><span data-stu-id="d64e6-203">Example: `data="name:part-name"`</span></span></p>
<span data-ttu-id="d64e6-204">**type**</span><span class="sxs-lookup"><span data-stu-id="d64e6-204">**type**</span></span></p>
<span data-ttu-id="d64e6-205">文件媒体类型用于确定页面上使用的文件图标，同时还确定当用户从 OneNote 激活设备上的文件时，会启动哪个应用程序。</span><span class="sxs-lookup"><span data-stu-id="d64e6-205">type="standardMimeType" indicates the file MIME type. This is used to select the file icon on the page, and also determines which application starts when the user activates the file on the device from OneNote.</span></span><br /><span data-ttu-id="d64e6-206">示例：`type="application/pdf"`</span><span class="sxs-lookup"><span data-stu-id="d64e6-206">Example: `type="application/pdf"`</span></span></p>


<a name="file-media-types"></a>

### <a name="file-media-types"></a><span data-ttu-id="d64e6-207">文件媒体类型</span><span class="sxs-lookup"><span data-stu-id="d64e6-207">File media types</span></span>  
<span data-ttu-id="d64e6-208">Microsoft Graph 为附加文件使用预定义的文件类型图标，当 API 不识别文件类型时，Microsoft Graph 会为其使用通用图标。</span><span class="sxs-lookup"><span data-stu-id="d64e6-208">Microsoft Graph uses predefined file-types icon for attached files, or a generic icon when the API doesn't recognize the file type.</span></span> <span data-ttu-id="d64e6-209">下表显示了 API 可识别的一些常见文件类型。</span><span class="sxs-lookup"><span data-stu-id="d64e6-209">The following table shows some common file types that are recognized by the API.</span></span>

- <span data-ttu-id="d64e6-210">application/pdf</span><span class="sxs-lookup"><span data-stu-id="d64e6-210">application/pdf</span></span>  
- <span data-ttu-id="d64e6-211">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span><span class="sxs-lookup"><span data-stu-id="d64e6-211">application/vnd.openxmlformats-officedocument.wordprocessingml.document</span></span>  
- <span data-ttu-id="d64e6-212">application/vnd.openxmlformats-officedocument.presentationml.presentation</span><span class="sxs-lookup"><span data-stu-id="d64e6-212">application/vnd.openxmlformats-officedocument.presentationml.presentation</span></span>
- <span data-ttu-id="d64e6-213">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span><span class="sxs-lookup"><span data-stu-id="d64e6-213">application/vnd.openxmlformats-officedocument.spreadsheetml.sheet</span></span>
- <span data-ttu-id="d64e6-214">image/png</span><span class="sxs-lookup"><span data-stu-id="d64e6-214">image/png</span></span>
- <span data-ttu-id="d64e6-215">image/jpeg</span><span class="sxs-lookup"><span data-stu-id="d64e6-215">image/jpeg</span></span>
- <span data-ttu-id="d64e6-216">image/gif</span><span class="sxs-lookup"><span data-stu-id="d64e6-216">image/gif</span></span>
- <span data-ttu-id="d64e6-217">audio/wav</span><span class="sxs-lookup"><span data-stu-id="d64e6-217">audio/wav</span></span>
- <span data-ttu-id="d64e6-218">video/mp4</span><span class="sxs-lookup"><span data-stu-id="d64e6-218">video/mp4</span></span>
- <span data-ttu-id="d64e6-219">application/msword</span><span class="sxs-lookup"><span data-stu-id="d64e6-219">application/msword</span></span>
- <span data-ttu-id="d64e6-220">application/mspowerpoint</span><span class="sxs-lookup"><span data-stu-id="d64e6-220">application/mspowerpoint</span></span>
- <span data-ttu-id="d64e6-221">application/excel</span><span class="sxs-lookup"><span data-stu-id="d64e6-221">application/excel</span></span>

<span data-ttu-id="d64e6-222">请参阅创建包含媒体的页面时应用的[限制](#size-limitations-for-post-pages-requests)。</span><span class="sxs-lookup"><span data-stu-id="d64e6-222">See [limitations](#size-limitations-for-post-pages-requests) that apply when creating pages that contain media.</span></span>


<a name="file-object"></a>
### <a name="add-a-file-attachment"></a><span data-ttu-id="d64e6-223">添加文件附件</span><span class="sxs-lookup"><span data-stu-id="d64e6-223">Add a file attachment</span></span>

<span data-ttu-id="d64e6-224">在请求的 **Presentation** 部件的输入 HTML 中，包括 `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`，其中 *part-name* 是包含二进制文件数据的[多部分请求](onenote-create-page.md#example-request)中的数据部件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d64e6-224">In the input HTML of your request's **Presentation** part, include  `<object data="name:part-name" data-attachment="file-name.file-ext" type="media-type/media-subtype" />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="d64e6-225">请只发送二进制数据，不要使用 Base64 或其他方式对其进行编码。</span><span class="sxs-lookup"><span data-stu-id="d64e6-225">The image data is the binary file data; don't use Base64 or otherwise encode it.</span></span>

```
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
### <a name="add-images-of-pdf-file-contents"></a><span data-ttu-id="d64e6-226">添加 PDF 文件内容的图像</span><span class="sxs-lookup"><span data-stu-id="d64e6-226">Add images of PDF file contents</span></span>

<span data-ttu-id="d64e6-227">在请求的 **Presentation** 部件的输入 HTML 中，包括 `<img data-render-src="name:part-name" ... />`，其中 *part-name* 是包含二进制文件数据的[多部分请求](onenote-create-page.md#example-request)中的数据部件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d64e6-227">In the input HTML of your request's **Presentation** part, include  `<img data-render-src="name:part-name" ... />`, where *part-name* is the unique identifier for the data part in your [multipart request](onenote-create-page.md#example-request) that contains the binary file data.</span></span> <span data-ttu-id="d64e6-228">请只发送二进制数据，不要使用 Base64 或其他方式对其进行编码。</span><span class="sxs-lookup"><span data-stu-id="d64e6-228">The image data is the binary file data; don't use Base64 or otherwise encode it.</span></span>

```
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
## <a name="size-limitations-for-post-pages-requests"></a><span data-ttu-id="d64e6-229">POST 页面请求的大小限制</span><span class="sxs-lookup"><span data-stu-id="d64e6-229">Size limitations for POST pages requests</span></span>

<span data-ttu-id="d64e6-230">发送图像和文件数据时，应注意以下限制：<!--TODO: check these--></span><span class="sxs-lookup"><span data-stu-id="d64e6-230">When sending image and file data, be aware of these limitations: <!--TODO: check these--></span></span>

- <span data-ttu-id="d64e6-231">POST 的总大小限制为 ~ 70 MB，包括图像、文件和其他数据。</span><span class="sxs-lookup"><span data-stu-id="d64e6-231">The total POST size limit is ~70 MB, including images, files, and other data.</span></span> <span data-ttu-id="d64e6-232">实际限制会受下游编码的影响，因此没有固定的字节计数限制。</span><span class="sxs-lookup"><span data-stu-id="d64e6-232">The actual limit is affected by downstream encoding, so there's no fixed byte-count limit.</span></span> <span data-ttu-id="d64e6-233">超过此限制的请求可能会产生不可靠的结果。</span><span class="sxs-lookup"><span data-stu-id="d64e6-233">Requests that exceed the limit may produce unreliable results.</span></span>

- <span data-ttu-id="d64e6-234">每个数据部件限制为 25 MB，包括部件标头。</span><span class="sxs-lookup"><span data-stu-id="d64e6-234">The limit for each data part is 25 MB, including the part headers.</span></span> <span data-ttu-id="d64e6-235">Microsoft Graph 将拒绝超过此限制的数据部件。</span><span class="sxs-lookup"><span data-stu-id="d64e6-235">Data parts that exceed the limit are rejected by Microsoft Graph.</span></span> 

- <span data-ttu-id="d64e6-236">每个页面的最大图像数为 150。</span><span class="sxs-lookup"><span data-stu-id="d64e6-236">The maximum number of images per page is 150.</span></span> <span data-ttu-id="d64e6-237">使用 `src="http://..."` 属性时，API 将忽略超出此限制的 **img** 标记。</span><span class="sxs-lookup"><span data-stu-id="d64e6-237">Image limit is 150 per page. When using the **src="internetURL"`src="http://..."` attribute, the API ignores <img>** tags beyond the limit.</span></span>

- <span data-ttu-id="d64e6-238">数据部件的最大数量是每个 POST 6 个，包括必需的 **Presentation** 部件。</span><span class="sxs-lookup"><span data-stu-id="d64e6-238">The maximum number of data parts is 6 per POST, including the required **Presentation** part.</span></span>

- <span data-ttu-id="d64e6-239">每个请求可以包含最多 5 个使用 **data-render-src** 的 **img** 元素和一个使用 **data-render-src** 的 **object** 元素。其他图像和文件引用将被忽略。</span><span class="sxs-lookup"><span data-stu-id="d64e6-239">Each request can contain up to five **img** elements that use **data-render-src** and one **object** elements that uses **data-render-src**. Additional image and file references are ignored.</span></span>

- <span data-ttu-id="d64e6-240">无论使用哪种方法将图像发送到 API，单个 POST 中图像的最大数量都是 30 个。</span><span class="sxs-lookup"><span data-stu-id="d64e6-240">The maximum number of images in a single POST is 30, no matter which method you use to send them to the API.</span></span> <span data-ttu-id="d64e6-241">其他图像将被忽略。</span><span class="sxs-lookup"><span data-stu-id="d64e6-241">Additional images are ignored.</span></span> <span data-ttu-id="d64e6-242">如果想要捕获包含大量图像的网页，请考虑[捕获整个页面作为快照](#add-a-webpage-snapshot)。</span><span class="sxs-lookup"><span data-stu-id="d64e6-242">If you want to capture a webpage that contains a lot of images, consider [capturing the whole page as a snapshot](#add-a-webpage-snapshot).</span></span>


## <a name="when-to-use-html-versus-data-render-src"></a><span data-ttu-id="d64e6-243">何时将 HTML 与 *data-render-src* 结合使用</span><span class="sxs-lookup"><span data-stu-id="d64e6-243">When to use HTML versus *data-render-src*</span></span> 
<span data-ttu-id="d64e6-244">尝试在直接将 HTML 置于 OneNote 页面与使用 **data-render-src** 属性之间选择时，请考虑以下情况：</span><span class="sxs-lookup"><span data-stu-id="d64e6-244">When trying to decide between directly putting HTML onto the OneNote page, versus using the data-render-src rendering, consider the following:</span></span>

- <span data-ttu-id="d64e6-245">最好通过 **data-render-src** 发送复杂 HTML 来呈现引擎，而不是尝试修改 HTML 来使其符合 Microsoft Graph 的要求。</span><span class="sxs-lookup"><span data-stu-id="d64e6-245">Complex HTML is probably best sent to the rendering engine via data-render-src, rather than attempting to modify the HTML to fit into what the oncshort API can accept. This is also true when your HTML includes tags not yet supported (see ).</span></span> <span data-ttu-id="d64e6-246">此外，当 HTML 包含不支持的标记时，这也是如此。</span><span class="sxs-lookup"><span data-stu-id="d64e6-246">This is also true when your HTML includes tags that aren't supported supported.</span></span>

- <span data-ttu-id="d64e6-247">精确页面呈现，以保留页面布局和外观时，最好是通过 **data-render-src** 使用呈现引擎完成。</span><span class="sxs-lookup"><span data-stu-id="d64e6-247">Accurate page rendering to preserve the layout and look of the page is probably best done with the rendering engine via **data-render-src**.</span></span>

- <span data-ttu-id="d64e6-248">通常，直接可编辑文本最好是通过直接将 HTML 插入到页面上来实现。</span><span class="sxs-lookup"><span data-stu-id="d64e6-248">Directly-editable text is often best done with inserting the HTML directly onto the page. The rendered images are scanned by an optical character recognition (OCR) system, but it's just not the same.</span></span> <span data-ttu-id="d64e6-249">呈现的图像由光学字符识别 (OCR) 系统进行扫描，但它不会完全相同。</span><span class="sxs-lookup"><span data-stu-id="d64e6-249">Directly-editable text is often best done with inserting the HTML directly onto the page. The rendered images are scanned by an optical character recognition (OCR) system, but it's just not the same.</span></span>

- <span data-ttu-id="d64e6-250">出于历史记录或存档目的的实时快照，最好是使用 data-render-src 方法来实现。</span><span class="sxs-lookup"><span data-stu-id="d64e6-250">Snapshot-in-time for historical or archival purposes is usually best done with the data-render-src method.</span></span>

- <span data-ttu-id="d64e6-251">为修订标记网页设计也是 **data-render-src** 能够真正发挥作用的地方。</span><span class="sxs-lookup"><span data-stu-id="d64e6-251">Marking-up a web page design for revisions is one place the **data-render-src** truly shines.</span></span> <span data-ttu-id="d64e6-252">使用 OneNote 的墨迹功能，可以在图像上绘制以指示更改或显示重要区域。</span><span class="sxs-lookup"><span data-stu-id="d64e6-252">Using OneNote's inking capabilities, you can draw on the image to indicate changes or call out important areas.</span></span> <span data-ttu-id="d64e6-253">将网页转换成图像使其更易于操作。</span><span class="sxs-lookup"><span data-stu-id="d64e6-253">Having the web page as an image makes that a lot easier.</span></span>

- <span data-ttu-id="d64e6-254">对于很大的图像或格式不是 OneNote 可直接接受的图像，有时可以生成缩略图，与在自己的代码中进行图像转换相比，使用 **data-render-src** 属性转换更为容易。</span><span class="sxs-lookup"><span data-stu-id="d64e6-254">Very large images, or images in formats that OneNote doesn't directly accept can sometimes be thumbnailed and converted with the data-render-src method more easily than by doing it in your own code.</span></span> <span data-ttu-id="d64e6-255">即使图像也可以在线使用，通过减少生成 OneNote 页面所需的往返总次数，将数据嵌入到 POST 中，有时也可以使 OneNote 用户更快地使用捕获到的页面。</span><span class="sxs-lookup"><span data-stu-id="d64e6-255">You can also send the image data for up to 150 images directly inside the oncshort API POST. This is common when the images are from a mobile device camera, or if your app is running on a hardware device like a scanner or camera. Even if the image is also available on the Internet, embedding the data in your POST can sometimes make the captured page available to OneNote user sooner, by reducing the total number of round-trips needed to build the OneNote page.</span></span>

<span data-ttu-id="d64e6-256">有时，确定哪种方法最适合用户的最佳方法是在开发应用时尝试这两种方法。</span><span class="sxs-lookup"><span data-stu-id="d64e6-256">Sometimes, the best way to determine which method will work best for your users is to try it both ways as you develop your app.</span></span>


<a name="permissions"></a>
## <a name="permissions"></a><span data-ttu-id="d64e6-257">权限</span><span class="sxs-lookup"><span data-stu-id="d64e6-257">Permissions</span></span>

<span data-ttu-id="d64e6-258">若要创建或更新 OneNote 页面，需要请求相应的权限。</span><span class="sxs-lookup"><span data-stu-id="d64e6-258">To create or update OneNote pages, you'll need to request appropriate permissions.</span></span> <span data-ttu-id="d64e6-259">选择应用正常运行所需的最低级别。</span><span class="sxs-lookup"><span data-stu-id="d64e6-259">Choose the lowest level that your app needs to do its work.</span></span>

<span data-ttu-id="d64e6-260">**_POST 页面_的权限**</span><span class="sxs-lookup"><span data-stu-id="d64e6-260">**Permissions for _POST pages_**</span></span>

- <span data-ttu-id="d64e6-261">Notes.Create</span><span class="sxs-lookup"><span data-stu-id="d64e6-261">Notes.Create</span></span>
- <span data-ttu-id="d64e6-262">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d64e6-262">Notes.ReadWrite</span></span>
- <span data-ttu-id="d64e6-263">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64e6-263">Notes.ReadWrite.All</span></span> 

<span data-ttu-id="d64e6-264">**_PATCH 页面_的权限**</span><span class="sxs-lookup"><span data-stu-id="d64e6-264">**Permissions for _PATCH pages_**</span></span>

- <span data-ttu-id="d64e6-265">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d64e6-265">Notes.ReadWrite</span></span>
- <span data-ttu-id="d64e6-266">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d64e6-266">Notes.ReadWrite.All</span></span>

<span data-ttu-id="d64e6-267">有关权限范围及其工作方式的详细信息，请参阅 [OneNote 权限范围](permissions_reference.md#notes-permissions)。</span><span class="sxs-lookup"><span data-stu-id="d64e6-267">For more information about how permission scopes work, see [OneNote permission scopes](permissions_reference.md#notes-permissions).</span></span>


<a name="see-also"></a>
## <a name="additional-resources"></a><span data-ttu-id="d64e6-268">其他资源</span><span class="sxs-lookup"><span data-stu-id="d64e6-268">Additional resources</span></span>

- [<span data-ttu-id="d64e6-269">与 OneNote 集成</span><span class="sxs-lookup"><span data-stu-id="d64e6-269">Integrate with OneNote</span></span>](integrate_with_onenote.md)
- [<span data-ttu-id="d64e6-270">OneNote 开发者博客</span><span class="sxs-lookup"><span data-stu-id="d64e6-270">OneNote Developer Blog</span></span>](http://go.microsoft.com/fwlink/?LinkID=390183)
- [<span data-ttu-id="d64e6-271">关于 Stack Overflow 的 OneNote 开发问题</span><span class="sxs-lookup"><span data-stu-id="d64e6-271">OneNote development questions on Stack Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkID=390182)
- [<span data-ttu-id="d64e6-272">OneNote GitHub 存储库</span><span class="sxs-lookup"><span data-stu-id="d64e6-272">OneNote GitHub repos</span></span>](http://go.microsoft.com/fwlink/?LinkID=390178)  
