---
title: 'driveItem: preview'
description: 此操作允许您获取项目的短生存期可嵌入 Url, 以呈现临时预览。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5e260e3dc360464b39daa5dde671a1bc11c9c6b6
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236298"
---
# <a name="driveitem-preview"></a><span data-ttu-id="61fd5-103">driveItem: preview</span><span class="sxs-lookup"><span data-stu-id="61fd5-103">driveItem: preview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61fd5-104">此操作允许您获取项目的短生存期可嵌入 Url, 以呈现临时预览。</span><span class="sxs-lookup"><span data-stu-id="61fd5-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="61fd5-105">如果要获取持续生存期的可嵌入链接, 请改用[createLink][] API。</span><span class="sxs-lookup"><span data-stu-id="61fd5-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="61fd5-106">**注意:\*\*\*\*预览**操作当前仅适用于 SharePoint 和 OneDrive for business。</span><span class="sxs-lookup"><span data-stu-id="61fd5-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="61fd5-108">权限</span><span class="sxs-lookup"><span data-stu-id="61fd5-108">Permissions</span></span>

<span data-ttu-id="61fd5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="61fd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="61fd5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="61fd5-111">Permission type</span></span>                        | <span data-ttu-id="61fd5-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="61fd5-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="61fd5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61fd5-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="61fd5-114">文件. 读取、文件读写、全部、读写全部。</span><span class="sxs-lookup"><span data-stu-id="61fd5-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="61fd5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61fd5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61fd5-116">Read, 文件. ReadWrite, 全部文件。</span><span class="sxs-lookup"><span data-stu-id="61fd5-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="61fd5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="61fd5-117">Application</span></span>                            | <span data-ttu-id="61fd5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="61fd5-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="61fd5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61fd5-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="61fd5-120">请求正文</span><span class="sxs-lookup"><span data-stu-id="61fd5-120">Request body</span></span>

<span data-ttu-id="61fd5-121">请求正文定义您的应用程序所请求的可嵌入 URL 的属性。</span><span class="sxs-lookup"><span data-stu-id="61fd5-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="61fd5-122">请求应为具有以下属性的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="61fd5-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="61fd5-123">名称</span><span class="sxs-lookup"><span data-stu-id="61fd5-123">Name</span></span>      |  <span data-ttu-id="61fd5-124">类型</span><span class="sxs-lookup"><span data-stu-id="61fd5-124">Type</span></span>         | <span data-ttu-id="61fd5-125">说明</span><span class="sxs-lookup"><span data-stu-id="61fd5-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="61fd5-126">格式</span><span class="sxs-lookup"><span data-stu-id="61fd5-126">viewer</span></span>      | <span data-ttu-id="61fd5-127">字符串</span><span class="sxs-lookup"><span data-stu-id="61fd5-127">string</span></span>        | <span data-ttu-id="61fd5-128">可选。</span><span class="sxs-lookup"><span data-stu-id="61fd5-128">Optional.</span></span> <span data-ttu-id="61fd5-129">要使用的预览应用。</span><span class="sxs-lookup"><span data-stu-id="61fd5-129">Preview app to use.</span></span> <span data-ttu-id="61fd5-130">`onedrive` 或 `office`）。</span><span class="sxs-lookup"><span data-stu-id="61fd5-130">`onedrive` or `office`.</span></span> <span data-ttu-id="61fd5-131">如果为 null, 则将自动选择合适的查看器。</span><span class="sxs-lookup"><span data-stu-id="61fd5-131">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="61fd5-132">chromeless</span><span class="sxs-lookup"><span data-stu-id="61fd5-132">chromeless</span></span>  | <span data-ttu-id="61fd5-133">布尔</span><span class="sxs-lookup"><span data-stu-id="61fd5-133">boolean</span></span>       | <span data-ttu-id="61fd5-134">可选。</span><span class="sxs-lookup"><span data-stu-id="61fd5-134">Optional.</span></span> <span data-ttu-id="61fd5-135">如果`true`为 (默认值), 则嵌入的视图将不包含任何控件。</span><span class="sxs-lookup"><span data-stu-id="61fd5-135">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="61fd5-136">allowEdit</span><span class="sxs-lookup"><span data-stu-id="61fd5-136">allowEdit</span></span>   | <span data-ttu-id="61fd5-137">布尔</span><span class="sxs-lookup"><span data-stu-id="61fd5-137">boolean</span></span>       | <span data-ttu-id="61fd5-138">可选。</span><span class="sxs-lookup"><span data-stu-id="61fd5-138">Optional.</span></span> <span data-ttu-id="61fd5-139">如果`true`是, 则可以从嵌入的 UI 编辑该文件。</span><span class="sxs-lookup"><span data-stu-id="61fd5-139">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="61fd5-140">page</span><span class="sxs-lookup"><span data-stu-id="61fd5-140">page</span></span>        | <span data-ttu-id="61fd5-141">string/number</span><span class="sxs-lookup"><span data-stu-id="61fd5-141">string/number</span></span> | <span data-ttu-id="61fd5-142">可选。</span><span class="sxs-lookup"><span data-stu-id="61fd5-142">Optional.</span></span> <span data-ttu-id="61fd5-143">要从其开始的文档的页码 (如果适用)。</span><span class="sxs-lookup"><span data-stu-id="61fd5-143">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="61fd5-144">为在文件类型 (如 ZIP) 周围的将来用例指定为字符串。</span><span class="sxs-lookup"><span data-stu-id="61fd5-144">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="61fd5-145">zoom</span><span class="sxs-lookup"><span data-stu-id="61fd5-145">zoom</span></span>        | <span data-ttu-id="61fd5-146">number</span><span class="sxs-lookup"><span data-stu-id="61fd5-146">number</span></span>        | <span data-ttu-id="61fd5-147">可选。</span><span class="sxs-lookup"><span data-stu-id="61fd5-147">Optional.</span></span> <span data-ttu-id="61fd5-148">要从其开始的缩放级别 (如果适用)。</span><span class="sxs-lookup"><span data-stu-id="61fd5-148">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="61fd5-149">响应</span><span class="sxs-lookup"><span data-stu-id="61fd5-149">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="61fd5-150">响应将是一个包含以下属性的 JSON 对象:</span><span class="sxs-lookup"><span data-stu-id="61fd5-150">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="61fd5-151">名称</span><span class="sxs-lookup"><span data-stu-id="61fd5-151">Name</span></span>           | <span data-ttu-id="61fd5-152">类型</span><span class="sxs-lookup"><span data-stu-id="61fd5-152">Type</span></span>   | <span data-ttu-id="61fd5-153">说明</span><span class="sxs-lookup"><span data-stu-id="61fd5-153">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="61fd5-154">getUrl</span><span class="sxs-lookup"><span data-stu-id="61fd5-154">getUrl</span></span>         | <span data-ttu-id="61fd5-155">string</span><span class="sxs-lookup"><span data-stu-id="61fd5-155">string</span></span> | <span data-ttu-id="61fd5-156">适合使用 HTTP GET (iframe 等) 进行嵌入的 URL</span><span class="sxs-lookup"><span data-stu-id="61fd5-156">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="61fd5-157">postUrl</span><span class="sxs-lookup"><span data-stu-id="61fd5-157">postUrl</span></span>        | <span data-ttu-id="61fd5-158">string</span><span class="sxs-lookup"><span data-stu-id="61fd5-158">string</span></span> | <span data-ttu-id="61fd5-159">适合使用 HTTP POST (窗体 POST、JS 等) 嵌入的 URL</span><span class="sxs-lookup"><span data-stu-id="61fd5-159">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="61fd5-160">postParameters</span><span class="sxs-lookup"><span data-stu-id="61fd5-160">postParameters</span></span> | <span data-ttu-id="61fd5-161">string</span><span class="sxs-lookup"><span data-stu-id="61fd5-161">string</span></span> | <span data-ttu-id="61fd5-162">如果使用 postUrl, 则发布要包括的参数</span><span class="sxs-lookup"><span data-stu-id="61fd5-162">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="61fd5-163">根据指定选项的 embed 支持的当前状态, 可能会返回 getUrl、postUrl 或 both。</span><span class="sxs-lookup"><span data-stu-id="61fd5-163">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="61fd5-164">postParameters 是格式为`application/x-www-form-urlencoded`的字符串, 如果向 POSTURL 执行 POST, 应相应地设置内容类型。</span><span class="sxs-lookup"><span data-stu-id="61fd5-164">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="61fd5-165">例如：</span><span class="sxs-lookup"><span data-stu-id="61fd5-165">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="61fd5-166">查看者</span><span class="sxs-lookup"><span data-stu-id="61fd5-166">Viewers</span></span>

<span data-ttu-id="61fd5-167">**查看器**参数允许使用以下值。</span><span class="sxs-lookup"><span data-stu-id="61fd5-167">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="61fd5-168">类型值</span><span class="sxs-lookup"><span data-stu-id="61fd5-168">Type value</span></span> | <span data-ttu-id="61fd5-169">说明</span><span class="sxs-lookup"><span data-stu-id="61fd5-169">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="61fd5-170">不适</span><span class="sxs-lookup"><span data-stu-id="61fd5-170">(null)</span></span>     | <span data-ttu-id="61fd5-171">选择用于呈现文件的适当的应用程序。</span><span class="sxs-lookup"><span data-stu-id="61fd5-171">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="61fd5-172">在大多数情况下, 这将`onedrive`使用预览器, 但可能因文件类型而异。</span><span class="sxs-lookup"><span data-stu-id="61fd5-172">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="61fd5-173">使用 OneDrive 预览器应用程序呈现文件。</span><span class="sxs-lookup"><span data-stu-id="61fd5-173">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="61fd5-174">使用 Office 的 web 版本呈现文件。</span><span class="sxs-lookup"><span data-stu-id="61fd5-174">Use the web version of Office to render the file.</span></span> <span data-ttu-id="61fd5-175">仅对 Office 文档有效。</span><span class="sxs-lookup"><span data-stu-id="61fd5-175">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="61fd5-176">Chrome vs chromeless</span><span class="sxs-lookup"><span data-stu-id="61fd5-176">Chrome vs chromeless</span></span>

<span data-ttu-id="61fd5-177">如果`chromeless`为 true, 预览将是文件的简略呈现。</span><span class="sxs-lookup"><span data-stu-id="61fd5-177">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="61fd5-178">否则, 可能会显示其他工具栏/按钮以与文档/视图进行交互。</span><span class="sxs-lookup"><span data-stu-id="61fd5-178">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="61fd5-179">查看/编辑</span><span class="sxs-lookup"><span data-stu-id="61fd5-179">View/edit</span></span>

<span data-ttu-id="61fd5-180">如果`allowEdit`为 true, 则文档可以通过嵌入预览的用户交互进行修改。</span><span class="sxs-lookup"><span data-stu-id="61fd5-180">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="61fd5-181">此功能可能不适用于所有预览版应用或文件类型。</span><span class="sxs-lookup"><span data-stu-id="61fd5-181">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="61fd5-182">页面/缩放</span><span class="sxs-lookup"><span data-stu-id="61fd5-182">Page/zoom</span></span>

<span data-ttu-id="61fd5-183">" `page` " `zoom`和 "" 选项可能不适用于所有预览版应用, 但如果预览应用支持它, 则将应用 "" 和 "" 选项。</span><span class="sxs-lookup"><span data-stu-id="61fd5-183">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
