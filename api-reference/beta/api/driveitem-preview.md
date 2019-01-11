---
title: driveItem： 预览
description: 此操作，可以获取项目的短期嵌入 Url 以便呈现临时预览。
localization_priority: Normal
ms.openlocfilehash: 4487e18ed1921f4164c335ba477e0ae5b74e456a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833171"
---
# <a name="driveitem-preview"></a><span data-ttu-id="0b8ce-103">driveItem： 预览</span><span class="sxs-lookup"><span data-stu-id="0b8ce-103">driveItem: preview</span></span>

> <span data-ttu-id="0b8ce-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b8ce-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0b8ce-106">此操作，可以获取项目的短期嵌入 Url 以便呈现临时预览。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-106">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="0b8ce-107">如果您想要获取长生存期嵌入链接，请改用[createLink][] API。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-107">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="0b8ce-108">**注意：\*\*\*\*预览**操作才当前 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-108">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="0b8ce-110">权限</span><span class="sxs-lookup"><span data-stu-id="0b8ce-110">Permissions</span></span>

<span data-ttu-id="0b8ce-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b8ce-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b8ce-113">Permission type</span></span>                        | <span data-ttu-id="0b8ce-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b8ce-114">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="0b8ce-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b8ce-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b8ce-116">Files.Read，Files.ReadWrite，Files.ReadWrite.All Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b8ce-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="0b8ce-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b8ce-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b8ce-118">Files.Read，Files.ReadWrite，Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b8ce-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="0b8ce-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b8ce-119">Application</span></span>                            | <span data-ttu-id="0b8ce-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-120">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="0b8ce-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b8ce-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="0b8ce-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b8ce-122">Request body</span></span>

<span data-ttu-id="0b8ce-123">在请求正文定义嵌入请求您的应用程序的 URL 的属性。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-123">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="0b8ce-124">请求应为具有以下属性的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-124">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="0b8ce-125">名称</span><span class="sxs-lookup"><span data-stu-id="0b8ce-125">Name</span></span>      |  <span data-ttu-id="0b8ce-126">类型</span><span class="sxs-lookup"><span data-stu-id="0b8ce-126">Type</span></span>         | <span data-ttu-id="0b8ce-127">Description</span><span class="sxs-lookup"><span data-stu-id="0b8ce-127">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="0b8ce-128">查看器</span><span class="sxs-lookup"><span data-stu-id="0b8ce-128">viewer</span></span>      | <span data-ttu-id="0b8ce-129">string</span><span class="sxs-lookup"><span data-stu-id="0b8ce-129">string</span></span>        | <span data-ttu-id="0b8ce-130">可选。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-130">Optional.</span></span> <span data-ttu-id="0b8ce-131">预览应用程序使用。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-131">Preview app to use.</span></span> <span data-ttu-id="0b8ce-132">`onedrive` 或 `office`）。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-132">`onedrive` or `office`.</span></span> <span data-ttu-id="0b8ce-133">如果为空，将自动选择合适的查看器。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-133">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="0b8ce-134">边框</span><span class="sxs-lookup"><span data-stu-id="0b8ce-134">chromeless</span></span>  | <span data-ttu-id="0b8ce-135">boolean</span><span class="sxs-lookup"><span data-stu-id="0b8ce-135">boolean</span></span>       | <span data-ttu-id="0b8ce-136">可选。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-136">Optional.</span></span> <span data-ttu-id="0b8ce-137">如果`true`（默认），嵌入视图将不包括任何控件。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-137">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="0b8ce-138">allowEdit</span><span class="sxs-lookup"><span data-stu-id="0b8ce-138">allowEdit</span></span>   | <span data-ttu-id="0b8ce-139">boolean</span><span class="sxs-lookup"><span data-stu-id="0b8ce-139">boolean</span></span>       | <span data-ttu-id="0b8ce-140">可选。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-140">Optional.</span></span> <span data-ttu-id="0b8ce-141">如果`true`，该文件可以从嵌入 UI 进行编辑。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-141">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="0b8ce-142">page</span><span class="sxs-lookup"><span data-stu-id="0b8ce-142">page</span></span>        | <span data-ttu-id="0b8ce-143">字符串/编号</span><span class="sxs-lookup"><span data-stu-id="0b8ce-143">string/number</span></span> | <span data-ttu-id="0b8ce-144">可选。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-144">Optional.</span></span> <span data-ttu-id="0b8ce-145">要启动，如果适用文档的页码。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-145">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="0b8ce-146">指定为字符串的文件类型，如 ZIP 周围的将来使用情况。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-146">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="0b8ce-147">zoom</span><span class="sxs-lookup"><span data-stu-id="0b8ce-147">zoom</span></span>        | <span data-ttu-id="0b8ce-148">数字</span><span class="sxs-lookup"><span data-stu-id="0b8ce-148">number</span></span>        | <span data-ttu-id="0b8ce-149">可选。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-149">Optional.</span></span> <span data-ttu-id="0b8ce-150">如果适用，则缩放级别，从开始。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-150">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="0b8ce-151">响应</span><span class="sxs-lookup"><span data-stu-id="0b8ce-151">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="0b8ce-152">响应将是一个 JSON 对象，包含以下属性：</span><span class="sxs-lookup"><span data-stu-id="0b8ce-152">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="0b8ce-153">名称</span><span class="sxs-lookup"><span data-stu-id="0b8ce-153">Name</span></span>           | <span data-ttu-id="0b8ce-154">类型</span><span class="sxs-lookup"><span data-stu-id="0b8ce-154">Type</span></span>   | <span data-ttu-id="0b8ce-155">Description</span><span class="sxs-lookup"><span data-stu-id="0b8ce-155">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="0b8ce-156">getUrl</span><span class="sxs-lookup"><span data-stu-id="0b8ce-156">getUrl</span></span>         | <span data-ttu-id="0b8ce-157">string</span><span class="sxs-lookup"><span data-stu-id="0b8ce-157">string</span></span> | <span data-ttu-id="0b8ce-158">适用于嵌入使用 HTTP GET （iframe 等） 的 URL</span><span class="sxs-lookup"><span data-stu-id="0b8ce-158">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="0b8ce-159">postUrl</span><span class="sxs-lookup"><span data-stu-id="0b8ce-159">postUrl</span></span>        | <span data-ttu-id="0b8ce-160">string</span><span class="sxs-lookup"><span data-stu-id="0b8ce-160">string</span></span> | <span data-ttu-id="0b8ce-161">适用于嵌入使用 HTTP POST URL （窗体发布，JS 等。）</span><span class="sxs-lookup"><span data-stu-id="0b8ce-161">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="0b8ce-162">postParameters</span><span class="sxs-lookup"><span data-stu-id="0b8ce-162">postParameters</span></span> | <span data-ttu-id="0b8ce-163">string</span><span class="sxs-lookup"><span data-stu-id="0b8ce-163">string</span></span> | <span data-ttu-id="0b8ce-164">如果使用 postUrl 包括 POST 参数</span><span class="sxs-lookup"><span data-stu-id="0b8ce-164">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="0b8ce-165">GetUrl、 postUrl，或同时可能会返回根据嵌入支持指定的选项的当前状态。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-165">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="0b8ce-166">postParameters 是字符串格式设置为`application/x-www-form-urlencoded`，并且应该相应地设置执行 POST 到 postUrl 内容类型。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-166">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="0b8ce-167">例如：</span><span class="sxs-lookup"><span data-stu-id="0b8ce-167">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="0b8ce-168">查看者</span><span class="sxs-lookup"><span data-stu-id="0b8ce-168">Viewers</span></span>

<span data-ttu-id="0b8ce-169">**查看器**参数允许以下值。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-169">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="0b8ce-170">类型值</span><span class="sxs-lookup"><span data-stu-id="0b8ce-170">Type value</span></span> | <span data-ttu-id="0b8ce-171">说明</span><span class="sxs-lookup"><span data-stu-id="0b8ce-171">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="0b8ce-172">(null)</span><span class="sxs-lookup"><span data-stu-id="0b8ce-172">(null)</span></span>     | <span data-ttu-id="0b8ce-173">选择相应的应用程序用于呈现该文件。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-173">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="0b8ce-174">这将在大多数情况下使用`onedrive`预览器，但可能因文件类型。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-174">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="0b8ce-175">使用 OneDrive previewer app 呈现该文件。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-175">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="0b8ce-176">WAC (Office online) 用于呈现该文件。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-176">Use the WAC (Office online) to render the file.</span></span> <span data-ttu-id="0b8ce-177">唯一有效的 Office 文档。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-177">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="0b8ce-178">部件版式 vs 边框</span><span class="sxs-lookup"><span data-stu-id="0b8ce-178">Chrome vs chromeless</span></span>

<span data-ttu-id="0b8ce-179">如果`chromeless`是 true，则预览将该文件裸机呈现。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-179">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="0b8ce-180">否则，可能有其他工具栏/按钮显示与文档/视图进行交互。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-180">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="0b8ce-181">查看/编辑</span><span class="sxs-lookup"><span data-stu-id="0b8ce-181">View/edit</span></span>

<span data-ttu-id="0b8ce-182">如果`allowEdit`是 true，则可以通过嵌入的预览与用户交互修改文档。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-182">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="0b8ce-183">此功能可能不可用的全部预览应用程序或文件类型。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-183">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="0b8ce-184">页/缩放</span><span class="sxs-lookup"><span data-stu-id="0b8ce-184">Page/zoom</span></span>

<span data-ttu-id="0b8ce-185">`page`和`zoom`选项可能不是可用于所有预览应用程序，但如果预览应用程序支持将应用。</span><span class="sxs-lookup"><span data-stu-id="0b8ce-185">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
