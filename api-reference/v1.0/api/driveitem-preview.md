---
title: 'driveItem: preview'
description: 此操作允许您获取项目的短生存期可嵌入 Url, 以呈现临时预览。
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 1de53b8183f4277c0241a08822ef539613b83a45
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015339"
---
# <a name="driveitem-preview"></a><span data-ttu-id="262c8-103">driveItem: preview</span><span class="sxs-lookup"><span data-stu-id="262c8-103">driveItem: preview</span></span>

<span data-ttu-id="262c8-104">此操作允许您获取项目的短生存期可嵌入 Url, 以呈现临时预览。</span><span class="sxs-lookup"><span data-stu-id="262c8-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="262c8-105">如果要获取持续生存期的可嵌入链接, 请改用[createLink][] API。</span><span class="sxs-lookup"><span data-stu-id="262c8-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="262c8-106">**注意:\*\*\*\*预览**操作当前仅适用于 SharePoint 和 OneDrive for business。</span><span class="sxs-lookup"><span data-stu-id="262c8-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="262c8-108">权限</span><span class="sxs-lookup"><span data-stu-id="262c8-108">Permissions</span></span>

<span data-ttu-id="262c8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="262c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="262c8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="262c8-111">Permission type</span></span>                        | <span data-ttu-id="262c8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="262c8-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="262c8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="262c8-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="262c8-114">文件. 读取、文件读写、全部、读写全部。</span><span class="sxs-lookup"><span data-stu-id="262c8-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="262c8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="262c8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="262c8-116">Read, 文件. ReadWrite, 全部文件。</span><span class="sxs-lookup"><span data-stu-id="262c8-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="262c8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="262c8-117">Application</span></span>                            | <span data-ttu-id="262c8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="262c8-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="262c8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="262c8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="262c8-120">请求正文</span><span class="sxs-lookup"><span data-stu-id="262c8-120">Request body</span></span>

<span data-ttu-id="262c8-121">请求正文定义您的应用程序所请求的可嵌入 URL 的属性。</span><span class="sxs-lookup"><span data-stu-id="262c8-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="262c8-122">请求应为具有以下属性的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="262c8-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="262c8-123">名称</span><span class="sxs-lookup"><span data-stu-id="262c8-123">Name</span></span>      |  <span data-ttu-id="262c8-124">类型</span><span class="sxs-lookup"><span data-stu-id="262c8-124">Type</span></span>         | <span data-ttu-id="262c8-125">说明</span><span class="sxs-lookup"><span data-stu-id="262c8-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="262c8-126">page</span><span class="sxs-lookup"><span data-stu-id="262c8-126">page</span></span>        | <span data-ttu-id="262c8-127">string/number</span><span class="sxs-lookup"><span data-stu-id="262c8-127">string/number</span></span> | <span data-ttu-id="262c8-128">可选。</span><span class="sxs-lookup"><span data-stu-id="262c8-128">Optional.</span></span> <span data-ttu-id="262c8-129">要从其开始的文档的页码 (如果适用)。</span><span class="sxs-lookup"><span data-stu-id="262c8-129">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="262c8-130">为在文件类型 (如 ZIP) 周围的将来用例指定为字符串。</span><span class="sxs-lookup"><span data-stu-id="262c8-130">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="262c8-131">zoom</span><span class="sxs-lookup"><span data-stu-id="262c8-131">zoom</span></span>        | <span data-ttu-id="262c8-132">number</span><span class="sxs-lookup"><span data-stu-id="262c8-132">number</span></span>        | <span data-ttu-id="262c8-133">可选。</span><span class="sxs-lookup"><span data-stu-id="262c8-133">Optional.</span></span> <span data-ttu-id="262c8-134">要从其开始的缩放级别 (如果适用)。</span><span class="sxs-lookup"><span data-stu-id="262c8-134">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="262c8-135">响应</span><span class="sxs-lookup"><span data-stu-id="262c8-135">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="262c8-136">响应将是一个包含以下属性的 JSON 对象:</span><span class="sxs-lookup"><span data-stu-id="262c8-136">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="262c8-137">名称</span><span class="sxs-lookup"><span data-stu-id="262c8-137">Name</span></span>           | <span data-ttu-id="262c8-138">类型</span><span class="sxs-lookup"><span data-stu-id="262c8-138">Type</span></span>   | <span data-ttu-id="262c8-139">说明</span><span class="sxs-lookup"><span data-stu-id="262c8-139">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="262c8-140">getUrl</span><span class="sxs-lookup"><span data-stu-id="262c8-140">getUrl</span></span>         | <span data-ttu-id="262c8-141">string</span><span class="sxs-lookup"><span data-stu-id="262c8-141">string</span></span> | <span data-ttu-id="262c8-142">适合使用 HTTP GET (iframe 等) 进行嵌入的 URL</span><span class="sxs-lookup"><span data-stu-id="262c8-142">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="262c8-143">postUrl</span><span class="sxs-lookup"><span data-stu-id="262c8-143">postUrl</span></span>        | <span data-ttu-id="262c8-144">string</span><span class="sxs-lookup"><span data-stu-id="262c8-144">string</span></span> | <span data-ttu-id="262c8-145">适合使用 HTTP POST (窗体 POST、JS 等) 嵌入的 URL</span><span class="sxs-lookup"><span data-stu-id="262c8-145">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="262c8-146">postParameters</span><span class="sxs-lookup"><span data-stu-id="262c8-146">postParameters</span></span> | <span data-ttu-id="262c8-147">string</span><span class="sxs-lookup"><span data-stu-id="262c8-147">string</span></span> | <span data-ttu-id="262c8-148">如果使用 postUrl, 则发布要包括的参数</span><span class="sxs-lookup"><span data-stu-id="262c8-148">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="262c8-149">根据指定选项的 embed 支持的当前状态, 可能会返回 getUrl、postUrl 或 both。</span><span class="sxs-lookup"><span data-stu-id="262c8-149">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="262c8-150">postParameters 是格式为`application/x-www-form-urlencoded`的字符串, 如果向 POSTURL 执行 POST, 应相应地设置内容类型。</span><span class="sxs-lookup"><span data-stu-id="262c8-150">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="262c8-151">例如：</span><span class="sxs-lookup"><span data-stu-id="262c8-151">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="262c8-152">页面/缩放</span><span class="sxs-lookup"><span data-stu-id="262c8-152">Page/zoom</span></span>

<span data-ttu-id="262c8-153">"页面" 和 "缩放" 选项可能不适用于所有预览版应用程序, 但如果预览应用支持它, 则会应用。</span><span class="sxs-lookup"><span data-stu-id="262c8-153">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
