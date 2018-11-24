# <a name="driveitem-preview"></a><span data-ttu-id="e2c03-101">driveItem： 预览</span><span class="sxs-lookup"><span data-stu-id="e2c03-101">driveItem: preview</span></span>

<span data-ttu-id="e2c03-102">此操作，可以获取项目的短期嵌入 Url 以便呈现临时预览。</span><span class="sxs-lookup"><span data-stu-id="e2c03-102">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="e2c03-103">如果您想要获取长生存期嵌入链接，请改用[createLink][] API。</span><span class="sxs-lookup"><span data-stu-id="e2c03-103">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="e2c03-104">**注意：\*\*\*\*预览**操作才当前 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="e2c03-104">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveItem_createLink.md

## <a name="permissions"></a><span data-ttu-id="e2c03-106">权限</span><span class="sxs-lookup"><span data-stu-id="e2c03-106">Permissions</span></span>

<span data-ttu-id="e2c03-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e2c03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="e2c03-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2c03-109">Permission type</span></span>                        | <span data-ttu-id="e2c03-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2c03-110">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="e2c03-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2c03-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e2c03-112">Files.Read，Files.ReadWrite，Files.ReadWrite.All Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2c03-112">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="e2c03-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2c03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2c03-114">Files.Read，Files.ReadWrite，Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2c03-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="e2c03-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2c03-115">Application</span></span>                            | <span data-ttu-id="e2c03-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2c03-116">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="e2c03-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2c03-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="e2c03-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2c03-118">Request body</span></span>

<span data-ttu-id="e2c03-119">在请求正文定义嵌入请求您的应用程序的 URL 的属性。</span><span class="sxs-lookup"><span data-stu-id="e2c03-119">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="e2c03-120">请求应为具有以下属性的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e2c03-120">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="e2c03-121">名称</span><span class="sxs-lookup"><span data-stu-id="e2c03-121">Name</span></span>      |  <span data-ttu-id="e2c03-122">类型</span><span class="sxs-lookup"><span data-stu-id="e2c03-122">Type</span></span>         | <span data-ttu-id="e2c03-123">说明</span><span class="sxs-lookup"><span data-stu-id="e2c03-123">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="e2c03-124">page</span><span class="sxs-lookup"><span data-stu-id="e2c03-124">page</span></span>        | <span data-ttu-id="e2c03-125">字符串/编号</span><span class="sxs-lookup"><span data-stu-id="e2c03-125">string/number</span></span> | <span data-ttu-id="e2c03-126">可选。</span><span class="sxs-lookup"><span data-stu-id="e2c03-126">Optional.</span></span> <span data-ttu-id="e2c03-127">要启动，如果适用文档的页码。</span><span class="sxs-lookup"><span data-stu-id="e2c03-127">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="e2c03-128">指定为字符串的文件类型，如 ZIP 周围的将来使用情况。</span><span class="sxs-lookup"><span data-stu-id="e2c03-128">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="e2c03-129">zoom</span><span class="sxs-lookup"><span data-stu-id="e2c03-129">zoom</span></span>        | <span data-ttu-id="e2c03-130">number</span><span class="sxs-lookup"><span data-stu-id="e2c03-130">number</span></span>        | <span data-ttu-id="e2c03-131">可选。</span><span class="sxs-lookup"><span data-stu-id="e2c03-131">Optional.</span></span> <span data-ttu-id="e2c03-132">如果适用，则缩放级别，从开始。</span><span class="sxs-lookup"><span data-stu-id="e2c03-132">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="e2c03-133">响应</span><span class="sxs-lookup"><span data-stu-id="e2c03-133">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="e2c03-134">响应将是一个 JSON 对象，包含以下属性：</span><span class="sxs-lookup"><span data-stu-id="e2c03-134">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="e2c03-135">名称</span><span class="sxs-lookup"><span data-stu-id="e2c03-135">Name</span></span>           | <span data-ttu-id="e2c03-136">类型</span><span class="sxs-lookup"><span data-stu-id="e2c03-136">Type</span></span>   | <span data-ttu-id="e2c03-137">说明</span><span class="sxs-lookup"><span data-stu-id="e2c03-137">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="e2c03-138">getUrl</span><span class="sxs-lookup"><span data-stu-id="e2c03-138">getUrl</span></span>         | <span data-ttu-id="e2c03-139">string</span><span class="sxs-lookup"><span data-stu-id="e2c03-139">string</span></span> | <span data-ttu-id="e2c03-140">适用于嵌入使用 HTTP GET （iframe 等） 的 URL</span><span class="sxs-lookup"><span data-stu-id="e2c03-140">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="e2c03-141">postUrl</span><span class="sxs-lookup"><span data-stu-id="e2c03-141">postUrl</span></span>        | <span data-ttu-id="e2c03-142">string</span><span class="sxs-lookup"><span data-stu-id="e2c03-142">string</span></span> | <span data-ttu-id="e2c03-143">适用于嵌入使用 HTTP POST URL （窗体发布，JS 等。）</span><span class="sxs-lookup"><span data-stu-id="e2c03-143">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="e2c03-144">postParameters</span><span class="sxs-lookup"><span data-stu-id="e2c03-144">postParameters</span></span> | <span data-ttu-id="e2c03-145">string</span><span class="sxs-lookup"><span data-stu-id="e2c03-145">string</span></span> | <span data-ttu-id="e2c03-146">如果使用 postUrl 包括 POST 参数</span><span class="sxs-lookup"><span data-stu-id="e2c03-146">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="e2c03-147">GetUrl、 postUrl，或同时可能会返回根据嵌入支持指定的选项的当前状态。</span><span class="sxs-lookup"><span data-stu-id="e2c03-147">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="e2c03-148">postParameters 是字符串格式设置为`application/x-www-form-urlencoded`，并且应该相应地设置执行 POST 到 postUrl 内容类型。</span><span class="sxs-lookup"><span data-stu-id="e2c03-148">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="e2c03-149">例如：</span><span class="sxs-lookup"><span data-stu-id="e2c03-149">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="e2c03-150">页/缩放</span><span class="sxs-lookup"><span data-stu-id="e2c03-150">Page/zoom</span></span>

<span data-ttu-id="e2c03-151">页面和缩放选项可能适用于所有预览应用程序，但如果预览应用程序支持将应用。</span><span class="sxs-lookup"><span data-stu-id="e2c03-151">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
