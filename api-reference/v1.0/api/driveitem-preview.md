---
title: driveItem： preview
description: 此操作允许您获取项目的短生存期可嵌入 Url，以呈现临时预览。
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: 5fea16ce14e2df4b87ddc2b3f9246dfe758ec5b1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073262"
---
# <a name="driveitem-preview"></a><span data-ttu-id="0b6fd-103">driveItem： preview</span><span class="sxs-lookup"><span data-stu-id="0b6fd-103">driveItem: preview</span></span>

<span data-ttu-id="0b6fd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b6fd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b6fd-105">此操作允许您获取项目的短生存期可嵌入 URL，以便呈现临时预览。</span><span class="sxs-lookup"><span data-stu-id="0b6fd-105">This action allows you to obtain a short-lived embeddable URL for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="0b6fd-106">如果要获取持续生存期的可嵌入链接，请改用 [createLink][] API。</span><span class="sxs-lookup"><span data-stu-id="0b6fd-106">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="0b6fd-107">**注意：\*\*\*\*预览**操作当前仅适用于 SharePoint 和 OneDrive for business。</span><span class="sxs-lookup"><span data-stu-id="0b6fd-107">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="0b6fd-109">权限</span><span class="sxs-lookup"><span data-stu-id="0b6fd-109">Permissions</span></span>

<span data-ttu-id="0b6fd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b6fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b6fd-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b6fd-112">Permission type</span></span>                        | <span data-ttu-id="0b6fd-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b6fd-113">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="0b6fd-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b6fd-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b6fd-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b6fd-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="0b6fd-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b6fd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b6fd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b6fd-117">Not supported.</span></span>
| <span data-ttu-id="0b6fd-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b6fd-118">Application</span></span>                            | <span data-ttu-id="0b6fd-119">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b6fd-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="0b6fd-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b6fd-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="0b6fd-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b6fd-121">Request body</span></span>

<span data-ttu-id="0b6fd-122">请求正文定义您的应用程序所请求的可嵌入 URL 的属性。</span><span class="sxs-lookup"><span data-stu-id="0b6fd-122">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="0b6fd-123">请求应为具有以下属性的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="0b6fd-123">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="0b6fd-124">名称</span><span class="sxs-lookup"><span data-stu-id="0b6fd-124">Name</span></span>      |  <span data-ttu-id="0b6fd-125">类型</span><span class="sxs-lookup"><span data-stu-id="0b6fd-125">Type</span></span>         | <span data-ttu-id="0b6fd-126">说明</span><span class="sxs-lookup"><span data-stu-id="0b6fd-126">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="0b6fd-127">page</span><span class="sxs-lookup"><span data-stu-id="0b6fd-127">page</span></span>        | <span data-ttu-id="0b6fd-128">string/number</span><span class="sxs-lookup"><span data-stu-id="0b6fd-128">string/number</span></span> | <span data-ttu-id="0b6fd-129">可选。</span><span class="sxs-lookup"><span data-stu-id="0b6fd-129">Optional.</span></span> <span data-ttu-id="0b6fd-130">要从其开始的文档的页码（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="0b6fd-130">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="0b6fd-131">为在文件类型（如 ZIP）周围的将来用例指定为字符串。</span><span class="sxs-lookup"><span data-stu-id="0b6fd-131">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="0b6fd-132">zoom</span><span class="sxs-lookup"><span data-stu-id="0b6fd-132">zoom</span></span>        | <span data-ttu-id="0b6fd-133">number</span><span class="sxs-lookup"><span data-stu-id="0b6fd-133">number</span></span>        | <span data-ttu-id="0b6fd-134">可选。</span><span class="sxs-lookup"><span data-stu-id="0b6fd-134">Optional.</span></span> <span data-ttu-id="0b6fd-135">要从其开始的缩放级别（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="0b6fd-135">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="0b6fd-136">响应</span><span class="sxs-lookup"><span data-stu-id="0b6fd-136">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="0b6fd-137">响应将是一个包含以下属性的 JSON 对象：</span><span class="sxs-lookup"><span data-stu-id="0b6fd-137">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="0b6fd-138">名称</span><span class="sxs-lookup"><span data-stu-id="0b6fd-138">Name</span></span>           | <span data-ttu-id="0b6fd-139">类型</span><span class="sxs-lookup"><span data-stu-id="0b6fd-139">Type</span></span>   | <span data-ttu-id="0b6fd-140">说明</span><span class="sxs-lookup"><span data-stu-id="0b6fd-140">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="0b6fd-141">getUrl</span><span class="sxs-lookup"><span data-stu-id="0b6fd-141">getUrl</span></span>         | <span data-ttu-id="0b6fd-142">string</span><span class="sxs-lookup"><span data-stu-id="0b6fd-142">string</span></span> | <span data-ttu-id="0b6fd-143">适用于使用 HTTP GET (iframe 等嵌入的 URL ) </span><span class="sxs-lookup"><span data-stu-id="0b6fd-143">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="0b6fd-144">postUrl</span><span class="sxs-lookup"><span data-stu-id="0b6fd-144">postUrl</span></span>        | <span data-ttu-id="0b6fd-145">string</span><span class="sxs-lookup"><span data-stu-id="0b6fd-145">string</span></span> | <span data-ttu-id="0b6fd-146">适合使用 HTTP POST (表单 post、JS 等进行嵌入的 URL ) </span><span class="sxs-lookup"><span data-stu-id="0b6fd-146">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="0b6fd-147">postParameters</span><span class="sxs-lookup"><span data-stu-id="0b6fd-147">postParameters</span></span> | <span data-ttu-id="0b6fd-148">string</span><span class="sxs-lookup"><span data-stu-id="0b6fd-148">string</span></span> | <span data-ttu-id="0b6fd-149">如果使用 postUrl，则发布要包括的参数</span><span class="sxs-lookup"><span data-stu-id="0b6fd-149">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="0b6fd-150">根据指定选项的 embed 支持的当前状态，可能会返回 getUrl、postUrl 或 both。</span><span class="sxs-lookup"><span data-stu-id="0b6fd-150">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="0b6fd-151">postParameters 是格式为的字符串 `application/x-www-form-urlencoded` ，如果向 postUrl 执行 POST，应相应地设置内容类型。</span><span class="sxs-lookup"><span data-stu-id="0b6fd-151">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="0b6fd-152">例如：</span><span class="sxs-lookup"><span data-stu-id="0b6fd-152">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="0b6fd-153">页面/缩放</span><span class="sxs-lookup"><span data-stu-id="0b6fd-153">Page/zoom</span></span>

<span data-ttu-id="0b6fd-154">"页面" 和 "缩放" 选项可能不适用于所有预览版应用程序，但如果预览应用支持它，则会应用。</span><span class="sxs-lookup"><span data-stu-id="0b6fd-154">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>

