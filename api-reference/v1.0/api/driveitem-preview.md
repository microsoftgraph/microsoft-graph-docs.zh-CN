---
title: driveItem： preview
description: 此操作允许您获取项目的短生存期可嵌入 Url，以呈现临时预览。
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 95466aaeb0cfb9c4127391f4e19a75f58ce2931d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517683"
---
# <a name="driveitem-preview"></a><span data-ttu-id="25b7a-103">driveItem： preview</span><span class="sxs-lookup"><span data-stu-id="25b7a-103">driveItem: preview</span></span>

<span data-ttu-id="25b7a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25b7a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="25b7a-105">此操作允许您获取项目的短生存期可嵌入 Url，以呈现临时预览。</span><span class="sxs-lookup"><span data-stu-id="25b7a-105">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="25b7a-106">如果要获取持续生存期的可嵌入链接，请改用[createLink][] API。</span><span class="sxs-lookup"><span data-stu-id="25b7a-106">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="25b7a-107">**注意：\*\*\*\*预览**操作当前仅适用于 SharePoint 和 OneDrive for business。</span><span class="sxs-lookup"><span data-stu-id="25b7a-107">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="25b7a-109">权限</span><span class="sxs-lookup"><span data-stu-id="25b7a-109">Permissions</span></span>

<span data-ttu-id="25b7a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25b7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="25b7a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="25b7a-112">Permission type</span></span>                        | <span data-ttu-id="25b7a-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="25b7a-113">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="25b7a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25b7a-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="25b7a-115">文件. 读取、文件读写、全部、读写全部。</span><span class="sxs-lookup"><span data-stu-id="25b7a-115">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="25b7a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25b7a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25b7a-117">Read，文件. ReadWrite，全部文件。</span><span class="sxs-lookup"><span data-stu-id="25b7a-117">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="25b7a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="25b7a-118">Application</span></span>                            | <span data-ttu-id="25b7a-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="25b7a-119">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="25b7a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25b7a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="25b7a-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="25b7a-121">Request body</span></span>

<span data-ttu-id="25b7a-122">请求正文定义您的应用程序所请求的可嵌入 URL 的属性。</span><span class="sxs-lookup"><span data-stu-id="25b7a-122">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="25b7a-123">请求应为具有以下属性的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="25b7a-123">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="25b7a-124">名称</span><span class="sxs-lookup"><span data-stu-id="25b7a-124">Name</span></span>      |  <span data-ttu-id="25b7a-125">类型</span><span class="sxs-lookup"><span data-stu-id="25b7a-125">Type</span></span>         | <span data-ttu-id="25b7a-126">说明</span><span class="sxs-lookup"><span data-stu-id="25b7a-126">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="25b7a-127">page</span><span class="sxs-lookup"><span data-stu-id="25b7a-127">page</span></span>        | <span data-ttu-id="25b7a-128">string/number</span><span class="sxs-lookup"><span data-stu-id="25b7a-128">string/number</span></span> | <span data-ttu-id="25b7a-129">可选。</span><span class="sxs-lookup"><span data-stu-id="25b7a-129">Optional.</span></span> <span data-ttu-id="25b7a-130">要从其开始的文档的页码（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="25b7a-130">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="25b7a-131">为在文件类型（如 ZIP）周围的将来用例指定为字符串。</span><span class="sxs-lookup"><span data-stu-id="25b7a-131">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="25b7a-132">zoom</span><span class="sxs-lookup"><span data-stu-id="25b7a-132">zoom</span></span>        | <span data-ttu-id="25b7a-133">number</span><span class="sxs-lookup"><span data-stu-id="25b7a-133">number</span></span>        | <span data-ttu-id="25b7a-134">可选。</span><span class="sxs-lookup"><span data-stu-id="25b7a-134">Optional.</span></span> <span data-ttu-id="25b7a-135">要从其开始的缩放级别（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="25b7a-135">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="25b7a-136">响应</span><span class="sxs-lookup"><span data-stu-id="25b7a-136">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="25b7a-137">响应将是一个包含以下属性的 JSON 对象：</span><span class="sxs-lookup"><span data-stu-id="25b7a-137">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="25b7a-138">名称</span><span class="sxs-lookup"><span data-stu-id="25b7a-138">Name</span></span>           | <span data-ttu-id="25b7a-139">类型</span><span class="sxs-lookup"><span data-stu-id="25b7a-139">Type</span></span>   | <span data-ttu-id="25b7a-140">说明</span><span class="sxs-lookup"><span data-stu-id="25b7a-140">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="25b7a-141">getUrl</span><span class="sxs-lookup"><span data-stu-id="25b7a-141">getUrl</span></span>         | <span data-ttu-id="25b7a-142">字符串</span><span class="sxs-lookup"><span data-stu-id="25b7a-142">string</span></span> | <span data-ttu-id="25b7a-143">适合使用 HTTP GET （iframe 等）进行嵌入的 URL</span><span class="sxs-lookup"><span data-stu-id="25b7a-143">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="25b7a-144">postUrl</span><span class="sxs-lookup"><span data-stu-id="25b7a-144">postUrl</span></span>        | <span data-ttu-id="25b7a-145">字符串</span><span class="sxs-lookup"><span data-stu-id="25b7a-145">string</span></span> | <span data-ttu-id="25b7a-146">适合使用 HTTP POST （窗体 POST、JS 等）嵌入的 URL</span><span class="sxs-lookup"><span data-stu-id="25b7a-146">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="25b7a-147">postParameters</span><span class="sxs-lookup"><span data-stu-id="25b7a-147">postParameters</span></span> | <span data-ttu-id="25b7a-148">字符串</span><span class="sxs-lookup"><span data-stu-id="25b7a-148">string</span></span> | <span data-ttu-id="25b7a-149">如果使用 postUrl，则发布要包括的参数</span><span class="sxs-lookup"><span data-stu-id="25b7a-149">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="25b7a-150">根据指定选项的 embed 支持的当前状态，可能会返回 getUrl、postUrl 或 both。</span><span class="sxs-lookup"><span data-stu-id="25b7a-150">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="25b7a-151">postParameters 是格式为`application/x-www-form-urlencoded`的字符串，如果向 POSTURL 执行 POST，应相应地设置内容类型。</span><span class="sxs-lookup"><span data-stu-id="25b7a-151">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="25b7a-152">例如：</span><span class="sxs-lookup"><span data-stu-id="25b7a-152">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="25b7a-153">页面/缩放</span><span class="sxs-lookup"><span data-stu-id="25b7a-153">Page/zoom</span></span>

<span data-ttu-id="25b7a-154">"页面" 和 "缩放" 选项可能不适用于所有预览版应用程序，但如果预览应用支持它，则会应用。</span><span class="sxs-lookup"><span data-stu-id="25b7a-154">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
