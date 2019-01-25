---
title: driveItem： 预览
description: 此操作，可以获取项目的短期嵌入 Url 以便呈现临时预览。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a49a05e1e01616bc9bbbb713fd05805d9af3070
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508536"
---
# <a name="driveitem-preview"></a><span data-ttu-id="615ae-103">driveItem： 预览</span><span class="sxs-lookup"><span data-stu-id="615ae-103">driveItem: preview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="615ae-104">此操作，可以获取项目的短期嵌入 Url 以便呈现临时预览。</span><span class="sxs-lookup"><span data-stu-id="615ae-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="615ae-105">如果您想要获取长生存期嵌入链接，请改用[createLink][] API。</span><span class="sxs-lookup"><span data-stu-id="615ae-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="615ae-106">**注意：\*\*\*\*预览**操作才当前 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="615ae-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="615ae-108">权限</span><span class="sxs-lookup"><span data-stu-id="615ae-108">Permissions</span></span>

<span data-ttu-id="615ae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="615ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="615ae-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="615ae-111">Permission type</span></span>                        | <span data-ttu-id="615ae-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="615ae-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="615ae-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="615ae-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="615ae-114">Files.Read，Files.ReadWrite，Files.ReadWrite.All Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="615ae-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="615ae-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="615ae-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="615ae-116">Files.Read，Files.ReadWrite，Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="615ae-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="615ae-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="615ae-117">Application</span></span>                            | <span data-ttu-id="615ae-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="615ae-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="615ae-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="615ae-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="615ae-120">请求正文</span><span class="sxs-lookup"><span data-stu-id="615ae-120">Request body</span></span>

<span data-ttu-id="615ae-121">在请求正文定义嵌入请求您的应用程序的 URL 的属性。</span><span class="sxs-lookup"><span data-stu-id="615ae-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="615ae-122">请求应为具有以下属性的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="615ae-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="615ae-123">名称</span><span class="sxs-lookup"><span data-stu-id="615ae-123">Name</span></span>      |  <span data-ttu-id="615ae-124">类型</span><span class="sxs-lookup"><span data-stu-id="615ae-124">Type</span></span>         | <span data-ttu-id="615ae-125">说明</span><span class="sxs-lookup"><span data-stu-id="615ae-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="615ae-126">查看器</span><span class="sxs-lookup"><span data-stu-id="615ae-126">viewer</span></span>      | <span data-ttu-id="615ae-127">string</span><span class="sxs-lookup"><span data-stu-id="615ae-127">string</span></span>        | <span data-ttu-id="615ae-128">可选。</span><span class="sxs-lookup"><span data-stu-id="615ae-128">Optional.</span></span> <span data-ttu-id="615ae-129">预览应用程序使用。</span><span class="sxs-lookup"><span data-stu-id="615ae-129">Preview app to use.</span></span> <span data-ttu-id="615ae-130">`onedrive` 或 `office`）。</span><span class="sxs-lookup"><span data-stu-id="615ae-130">`onedrive` or `office`.</span></span> <span data-ttu-id="615ae-131">如果为空，将自动选择合适的查看器。</span><span class="sxs-lookup"><span data-stu-id="615ae-131">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="615ae-132">边框</span><span class="sxs-lookup"><span data-stu-id="615ae-132">chromeless</span></span>  | <span data-ttu-id="615ae-133">布尔</span><span class="sxs-lookup"><span data-stu-id="615ae-133">boolean</span></span>       | <span data-ttu-id="615ae-134">可选。</span><span class="sxs-lookup"><span data-stu-id="615ae-134">Optional.</span></span> <span data-ttu-id="615ae-135">如果`true`（默认），嵌入视图将不包括任何控件。</span><span class="sxs-lookup"><span data-stu-id="615ae-135">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="615ae-136">AllowEdit</span><span class="sxs-lookup"><span data-stu-id="615ae-136">allowEdit</span></span>   | <span data-ttu-id="615ae-137">布尔</span><span class="sxs-lookup"><span data-stu-id="615ae-137">boolean</span></span>       | <span data-ttu-id="615ae-138">可选。</span><span class="sxs-lookup"><span data-stu-id="615ae-138">Optional.</span></span> <span data-ttu-id="615ae-139">如果`true`，该文件可以从嵌入 UI 进行编辑。</span><span class="sxs-lookup"><span data-stu-id="615ae-139">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="615ae-140">page</span><span class="sxs-lookup"><span data-stu-id="615ae-140">page</span></span>        | <span data-ttu-id="615ae-141">字符串/编号</span><span class="sxs-lookup"><span data-stu-id="615ae-141">string/number</span></span> | <span data-ttu-id="615ae-142">可选。</span><span class="sxs-lookup"><span data-stu-id="615ae-142">Optional.</span></span> <span data-ttu-id="615ae-143">要启动，如果适用文档的页码。</span><span class="sxs-lookup"><span data-stu-id="615ae-143">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="615ae-144">指定为字符串的文件类型，如 ZIP 周围的将来使用情况。</span><span class="sxs-lookup"><span data-stu-id="615ae-144">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="615ae-145">zoom</span><span class="sxs-lookup"><span data-stu-id="615ae-145">zoom</span></span>        | <span data-ttu-id="615ae-146">数字</span><span class="sxs-lookup"><span data-stu-id="615ae-146">number</span></span>        | <span data-ttu-id="615ae-147">可选。</span><span class="sxs-lookup"><span data-stu-id="615ae-147">Optional.</span></span> <span data-ttu-id="615ae-148">如果适用，则缩放级别，从开始。</span><span class="sxs-lookup"><span data-stu-id="615ae-148">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="615ae-149">响应</span><span class="sxs-lookup"><span data-stu-id="615ae-149">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="615ae-150">响应将是一个 JSON 对象，包含以下属性：</span><span class="sxs-lookup"><span data-stu-id="615ae-150">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="615ae-151">名称</span><span class="sxs-lookup"><span data-stu-id="615ae-151">Name</span></span>           | <span data-ttu-id="615ae-152">类型</span><span class="sxs-lookup"><span data-stu-id="615ae-152">Type</span></span>   | <span data-ttu-id="615ae-153">说明</span><span class="sxs-lookup"><span data-stu-id="615ae-153">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="615ae-154">getUrl</span><span class="sxs-lookup"><span data-stu-id="615ae-154">getUrl</span></span>         | <span data-ttu-id="615ae-155">string</span><span class="sxs-lookup"><span data-stu-id="615ae-155">string</span></span> | <span data-ttu-id="615ae-156">适用于嵌入使用 HTTP GET （iframe 等） 的 URL</span><span class="sxs-lookup"><span data-stu-id="615ae-156">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="615ae-157">postUrl</span><span class="sxs-lookup"><span data-stu-id="615ae-157">postUrl</span></span>        | <span data-ttu-id="615ae-158">string</span><span class="sxs-lookup"><span data-stu-id="615ae-158">string</span></span> | <span data-ttu-id="615ae-159">适用于嵌入使用 HTTP POST URL （窗体发布，JS 等。）</span><span class="sxs-lookup"><span data-stu-id="615ae-159">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="615ae-160">postParameters</span><span class="sxs-lookup"><span data-stu-id="615ae-160">postParameters</span></span> | <span data-ttu-id="615ae-161">string</span><span class="sxs-lookup"><span data-stu-id="615ae-161">string</span></span> | <span data-ttu-id="615ae-162">如果使用 postUrl 包括 POST 参数</span><span class="sxs-lookup"><span data-stu-id="615ae-162">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="615ae-163">GetUrl、 postUrl，或同时可能会返回根据嵌入支持指定的选项的当前状态。</span><span class="sxs-lookup"><span data-stu-id="615ae-163">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="615ae-164">postParameters 是字符串格式设置为`application/x-www-form-urlencoded`，并且应该相应地设置执行 POST 到 postUrl 内容类型。</span><span class="sxs-lookup"><span data-stu-id="615ae-164">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="615ae-165">例如：</span><span class="sxs-lookup"><span data-stu-id="615ae-165">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="615ae-166">查看者</span><span class="sxs-lookup"><span data-stu-id="615ae-166">Viewers</span></span>

<span data-ttu-id="615ae-167">**查看器**参数允许以下值。</span><span class="sxs-lookup"><span data-stu-id="615ae-167">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="615ae-168">类型值</span><span class="sxs-lookup"><span data-stu-id="615ae-168">Type value</span></span> | <span data-ttu-id="615ae-169">说明</span><span class="sxs-lookup"><span data-stu-id="615ae-169">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="615ae-170">Null
</span><span class="sxs-lookup"><span data-stu-id="615ae-170">(null)</span></span>     | <span data-ttu-id="615ae-171">选择相应的应用程序用于呈现该文件。</span><span class="sxs-lookup"><span data-stu-id="615ae-171">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="615ae-172">这将在大多数情况下使用`onedrive`预览器，但可能因文件类型。</span><span class="sxs-lookup"><span data-stu-id="615ae-172">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="615ae-173">使用 OneDrive previewer app 呈现该文件。</span><span class="sxs-lookup"><span data-stu-id="615ae-173">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="615ae-174">WAC (Office online) 用于呈现该文件。</span><span class="sxs-lookup"><span data-stu-id="615ae-174">Use the WAC (Office online) to render the file.</span></span> <span data-ttu-id="615ae-175">唯一有效的 Office 文档。</span><span class="sxs-lookup"><span data-stu-id="615ae-175">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="615ae-176">部件版式 vs 边框</span><span class="sxs-lookup"><span data-stu-id="615ae-176">Chrome vs chromeless</span></span>

<span data-ttu-id="615ae-177">如果`chromeless`是 true，则预览将该文件裸机呈现。</span><span class="sxs-lookup"><span data-stu-id="615ae-177">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="615ae-178">否则，可能有其他工具栏/按钮显示与文档/视图进行交互。</span><span class="sxs-lookup"><span data-stu-id="615ae-178">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="615ae-179">查看/编辑</span><span class="sxs-lookup"><span data-stu-id="615ae-179">View/edit</span></span>

<span data-ttu-id="615ae-180">如果`allowEdit`是 true，则可以通过嵌入的预览与用户交互修改文档。</span><span class="sxs-lookup"><span data-stu-id="615ae-180">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="615ae-181">此功能可能不可用的全部预览应用程序或文件类型。</span><span class="sxs-lookup"><span data-stu-id="615ae-181">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="615ae-182">页/缩放</span><span class="sxs-lookup"><span data-stu-id="615ae-182">Page/zoom</span></span>

<span data-ttu-id="615ae-183">`page`和`zoom`选项可能不是可用于所有预览应用程序，但如果预览应用程序支持将应用。</span><span class="sxs-lookup"><span data-stu-id="615ae-183">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-preview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
