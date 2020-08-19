---
title: driveItem： preview
description: 此操作允许您获取项目的短生存期可嵌入 Url，以呈现临时预览。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
author: JeremyKelley
ms.openlocfilehash: 074bc4c0da2362c6be9958be3ffec8dd4027b690
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808821"
---
# <a name="driveitem-preview"></a><span data-ttu-id="0b964-103">driveItem： preview</span><span class="sxs-lookup"><span data-stu-id="0b964-103">driveItem: preview</span></span>

<span data-ttu-id="0b964-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b964-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b964-105">此操作允许您获取项目的短生存期可嵌入 Url，以呈现临时预览。</span><span class="sxs-lookup"><span data-stu-id="0b964-105">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="0b964-106">如果要获取持续生存期的可嵌入链接，请改用 [createLink][] API。</span><span class="sxs-lookup"><span data-stu-id="0b964-106">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="0b964-107">**注意：\*\*\*\*预览**操作当前仅适用于 SharePoint 和 OneDrive for business。</span><span class="sxs-lookup"><span data-stu-id="0b964-107">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="0b964-109">权限</span><span class="sxs-lookup"><span data-stu-id="0b964-109">Permissions</span></span>

<span data-ttu-id="0b964-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b964-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b964-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b964-112">Permission type</span></span>                        | <span data-ttu-id="0b964-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b964-113">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="0b964-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b964-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b964-115">文件. 读取、文件读写、全部、读写全部。</span><span class="sxs-lookup"><span data-stu-id="0b964-115">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="0b964-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b964-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b964-117">Read，文件. ReadWrite，全部文件。</span><span class="sxs-lookup"><span data-stu-id="0b964-117">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="0b964-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b964-118">Application</span></span>                            | <span data-ttu-id="0b964-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b964-119">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="0b964-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b964-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="0b964-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b964-121">Request body</span></span>

<span data-ttu-id="0b964-122">请求正文定义您的应用程序所请求的可嵌入 URL 的属性。</span><span class="sxs-lookup"><span data-stu-id="0b964-122">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="0b964-123">请求应为具有以下属性的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0b964-123">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="0b964-124">名称</span><span class="sxs-lookup"><span data-stu-id="0b964-124">Name</span></span>      |  <span data-ttu-id="0b964-125">类型</span><span class="sxs-lookup"><span data-stu-id="0b964-125">Type</span></span>         | <span data-ttu-id="0b964-126">说明</span><span class="sxs-lookup"><span data-stu-id="0b964-126">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="0b964-127">格式</span><span class="sxs-lookup"><span data-stu-id="0b964-127">viewer</span></span>      | <span data-ttu-id="0b964-128">string</span><span class="sxs-lookup"><span data-stu-id="0b964-128">string</span></span>        | <span data-ttu-id="0b964-129">可选。</span><span class="sxs-lookup"><span data-stu-id="0b964-129">Optional.</span></span> <span data-ttu-id="0b964-130">要使用的预览应用。</span><span class="sxs-lookup"><span data-stu-id="0b964-130">Preview app to use.</span></span> <span data-ttu-id="0b964-131">`onedrive` 或 `office`）。</span><span class="sxs-lookup"><span data-stu-id="0b964-131">`onedrive` or `office`.</span></span> <span data-ttu-id="0b964-132">如果为 null，则将自动选择合适的查看器。</span><span class="sxs-lookup"><span data-stu-id="0b964-132">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="0b964-133">chromeless</span><span class="sxs-lookup"><span data-stu-id="0b964-133">chromeless</span></span>  | <span data-ttu-id="0b964-134">布尔</span><span class="sxs-lookup"><span data-stu-id="0b964-134">boolean</span></span>       | <span data-ttu-id="0b964-135">可选。</span><span class="sxs-lookup"><span data-stu-id="0b964-135">Optional.</span></span> <span data-ttu-id="0b964-136">如果 `true` (默认) ，则嵌入的视图将不包含任何控件。</span><span class="sxs-lookup"><span data-stu-id="0b964-136">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="0b964-137">allowEdit</span><span class="sxs-lookup"><span data-stu-id="0b964-137">allowEdit</span></span>   | <span data-ttu-id="0b964-138">布尔</span><span class="sxs-lookup"><span data-stu-id="0b964-138">boolean</span></span>       | <span data-ttu-id="0b964-139">可选。</span><span class="sxs-lookup"><span data-stu-id="0b964-139">Optional.</span></span> <span data-ttu-id="0b964-140">如果 `true` 是，则可以从嵌入的 UI 编辑该文件。</span><span class="sxs-lookup"><span data-stu-id="0b964-140">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="0b964-141">page</span><span class="sxs-lookup"><span data-stu-id="0b964-141">page</span></span>        | <span data-ttu-id="0b964-142">string/number</span><span class="sxs-lookup"><span data-stu-id="0b964-142">string/number</span></span> | <span data-ttu-id="0b964-143">可选。</span><span class="sxs-lookup"><span data-stu-id="0b964-143">Optional.</span></span> <span data-ttu-id="0b964-144">要从其开始的文档的页码（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="0b964-144">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="0b964-145">为在文件类型（如 ZIP）周围的将来用例指定为字符串。</span><span class="sxs-lookup"><span data-stu-id="0b964-145">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="0b964-146">zoom</span><span class="sxs-lookup"><span data-stu-id="0b964-146">zoom</span></span>        | <span data-ttu-id="0b964-147">number</span><span class="sxs-lookup"><span data-stu-id="0b964-147">number</span></span>        | <span data-ttu-id="0b964-148">可选。</span><span class="sxs-lookup"><span data-stu-id="0b964-148">Optional.</span></span> <span data-ttu-id="0b964-149">要从其开始的缩放级别（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="0b964-149">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="0b964-150">响应</span><span class="sxs-lookup"><span data-stu-id="0b964-150">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="0b964-151">响应将是一个包含以下属性的 JSON 对象：</span><span class="sxs-lookup"><span data-stu-id="0b964-151">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="0b964-152">名称</span><span class="sxs-lookup"><span data-stu-id="0b964-152">Name</span></span>           | <span data-ttu-id="0b964-153">类型</span><span class="sxs-lookup"><span data-stu-id="0b964-153">Type</span></span>   | <span data-ttu-id="0b964-154">说明</span><span class="sxs-lookup"><span data-stu-id="0b964-154">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="0b964-155">getUrl</span><span class="sxs-lookup"><span data-stu-id="0b964-155">getUrl</span></span>         | <span data-ttu-id="0b964-156">string</span><span class="sxs-lookup"><span data-stu-id="0b964-156">string</span></span> | <span data-ttu-id="0b964-157">适用于使用 HTTP GET (iframe 等嵌入的 URL ) </span><span class="sxs-lookup"><span data-stu-id="0b964-157">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="0b964-158">postUrl</span><span class="sxs-lookup"><span data-stu-id="0b964-158">postUrl</span></span>        | <span data-ttu-id="0b964-159">string</span><span class="sxs-lookup"><span data-stu-id="0b964-159">string</span></span> | <span data-ttu-id="0b964-160">适合使用 HTTP POST (表单 post、JS 等进行嵌入的 URL ) </span><span class="sxs-lookup"><span data-stu-id="0b964-160">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="0b964-161">postParameters</span><span class="sxs-lookup"><span data-stu-id="0b964-161">postParameters</span></span> | <span data-ttu-id="0b964-162">string</span><span class="sxs-lookup"><span data-stu-id="0b964-162">string</span></span> | <span data-ttu-id="0b964-163">如果使用 postUrl，则发布要包括的参数</span><span class="sxs-lookup"><span data-stu-id="0b964-163">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="0b964-164">根据指定选项的 embed 支持的当前状态，可能会返回 getUrl、postUrl 或 both。</span><span class="sxs-lookup"><span data-stu-id="0b964-164">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="0b964-165">postParameters 是格式为的字符串 `application/x-www-form-urlencoded` ，如果向 postUrl 执行 POST，应相应地设置内容类型。</span><span class="sxs-lookup"><span data-stu-id="0b964-165">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="0b964-166">例如：</span><span class="sxs-lookup"><span data-stu-id="0b964-166">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="0b964-167">查看者</span><span class="sxs-lookup"><span data-stu-id="0b964-167">Viewers</span></span>

<span data-ttu-id="0b964-168">**查看器**参数允许使用以下值。</span><span class="sxs-lookup"><span data-stu-id="0b964-168">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="0b964-169">类型值</span><span class="sxs-lookup"><span data-stu-id="0b964-169">Type value</span></span> | <span data-ttu-id="0b964-170">说明</span><span class="sxs-lookup"><span data-stu-id="0b964-170">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="0b964-171"> (null) </span><span class="sxs-lookup"><span data-stu-id="0b964-171">(null)</span></span>     | <span data-ttu-id="0b964-172">选择用于呈现文件的适当的应用程序。</span><span class="sxs-lookup"><span data-stu-id="0b964-172">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="0b964-173">在大多数情况下，这将使用 `onedrive` 预览器，但可能因文件类型而异。</span><span class="sxs-lookup"><span data-stu-id="0b964-173">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="0b964-174">使用 OneDrive 预览器应用程序呈现文件。</span><span class="sxs-lookup"><span data-stu-id="0b964-174">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="0b964-175">使用 Office 的 web 版本呈现文件。</span><span class="sxs-lookup"><span data-stu-id="0b964-175">Use the web version of Office to render the file.</span></span> <span data-ttu-id="0b964-176">仅对 Office 文档有效。</span><span class="sxs-lookup"><span data-stu-id="0b964-176">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="0b964-177">Chrome vs chromeless</span><span class="sxs-lookup"><span data-stu-id="0b964-177">Chrome vs chromeless</span></span>

<span data-ttu-id="0b964-178">如果 `chromeless` 为 true，预览将是文件的简略呈现。</span><span class="sxs-lookup"><span data-stu-id="0b964-178">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="0b964-179">否则，可能会显示其他工具栏/按钮以与文档/视图进行交互。</span><span class="sxs-lookup"><span data-stu-id="0b964-179">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="0b964-180">查看/编辑</span><span class="sxs-lookup"><span data-stu-id="0b964-180">View/edit</span></span>

<span data-ttu-id="0b964-181">如果 `allowEdit` 为 true，则文档可以通过嵌入预览的用户交互进行修改。</span><span class="sxs-lookup"><span data-stu-id="0b964-181">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="0b964-182">此功能可能不适用于所有预览版应用或文件类型。</span><span class="sxs-lookup"><span data-stu-id="0b964-182">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="0b964-183">页面/缩放</span><span class="sxs-lookup"><span data-stu-id="0b964-183">Page/zoom</span></span>

<span data-ttu-id="0b964-184">"" 和 "" `page` `zoom` 选项可能不适用于所有预览版应用，但如果预览应用支持它，则将应用 "" 和 "" 选项。</span><span class="sxs-lookup"><span data-stu-id="0b964-184">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
