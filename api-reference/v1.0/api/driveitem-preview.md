---
title: driveItem： 预览
description: 此操作，可以获取项目的短期嵌入 Url 以便呈现临时预览。
localization_priority: Normal
ms.openlocfilehash: c04a73d514dfb5a92030c4c2016579d469063f9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850769"
---
# <a name="driveitem-preview"></a><span data-ttu-id="97782-103">driveItem： 预览</span><span class="sxs-lookup"><span data-stu-id="97782-103">driveItem: preview</span></span>

<span data-ttu-id="97782-104">此操作，可以获取项目的短期嵌入 Url 以便呈现临时预览。</span><span class="sxs-lookup"><span data-stu-id="97782-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="97782-105">如果您想要获取长生存期嵌入链接，请改用[createLink][] API。</span><span class="sxs-lookup"><span data-stu-id="97782-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="97782-106">**注意：\*\*\*\*预览**操作才当前 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="97782-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="97782-108">权限</span><span class="sxs-lookup"><span data-stu-id="97782-108">Permissions</span></span>

<span data-ttu-id="97782-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97782-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97782-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="97782-111">Permission type</span></span>                        | <span data-ttu-id="97782-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97782-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="97782-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97782-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="97782-114">Files.Read，Files.ReadWrite，Files.ReadWrite.All Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97782-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="97782-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97782-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97782-116">Files.Read，Files.ReadWrite，Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97782-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="97782-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="97782-117">Application</span></span>                            | <span data-ttu-id="97782-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="97782-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="97782-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97782-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="97782-120">请求正文</span><span class="sxs-lookup"><span data-stu-id="97782-120">Request body</span></span>

<span data-ttu-id="97782-121">在请求正文定义嵌入请求您的应用程序的 URL 的属性。</span><span class="sxs-lookup"><span data-stu-id="97782-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="97782-122">请求应为具有以下属性的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="97782-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="97782-123">名称</span><span class="sxs-lookup"><span data-stu-id="97782-123">Name</span></span>      |  <span data-ttu-id="97782-124">类型</span><span class="sxs-lookup"><span data-stu-id="97782-124">Type</span></span>         | <span data-ttu-id="97782-125">说明</span><span class="sxs-lookup"><span data-stu-id="97782-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="97782-126">page</span><span class="sxs-lookup"><span data-stu-id="97782-126">page</span></span>        | <span data-ttu-id="97782-127">字符串/编号</span><span class="sxs-lookup"><span data-stu-id="97782-127">string/number</span></span> | <span data-ttu-id="97782-128">可选。</span><span class="sxs-lookup"><span data-stu-id="97782-128">Optional.</span></span> <span data-ttu-id="97782-129">要启动，如果适用文档的页码。</span><span class="sxs-lookup"><span data-stu-id="97782-129">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="97782-130">指定为字符串的文件类型，如 ZIP 周围的将来使用情况。</span><span class="sxs-lookup"><span data-stu-id="97782-130">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="97782-131">zoom</span><span class="sxs-lookup"><span data-stu-id="97782-131">zoom</span></span>        | <span data-ttu-id="97782-132">数字</span><span class="sxs-lookup"><span data-stu-id="97782-132">number</span></span>        | <span data-ttu-id="97782-133">可选。</span><span class="sxs-lookup"><span data-stu-id="97782-133">Optional.</span></span> <span data-ttu-id="97782-134">如果适用，则缩放级别，从开始。</span><span class="sxs-lookup"><span data-stu-id="97782-134">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="97782-135">响应</span><span class="sxs-lookup"><span data-stu-id="97782-135">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="97782-136">响应将是一个 JSON 对象，包含以下属性：</span><span class="sxs-lookup"><span data-stu-id="97782-136">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="97782-137">名称</span><span class="sxs-lookup"><span data-stu-id="97782-137">Name</span></span>           | <span data-ttu-id="97782-138">类型</span><span class="sxs-lookup"><span data-stu-id="97782-138">Type</span></span>   | <span data-ttu-id="97782-139">Description</span><span class="sxs-lookup"><span data-stu-id="97782-139">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="97782-140">getUrl</span><span class="sxs-lookup"><span data-stu-id="97782-140">getUrl</span></span>         | <span data-ttu-id="97782-141">string</span><span class="sxs-lookup"><span data-stu-id="97782-141">string</span></span> | <span data-ttu-id="97782-142">适用于嵌入使用 HTTP GET （iframe 等） 的 URL</span><span class="sxs-lookup"><span data-stu-id="97782-142">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="97782-143">postUrl</span><span class="sxs-lookup"><span data-stu-id="97782-143">postUrl</span></span>        | <span data-ttu-id="97782-144">string</span><span class="sxs-lookup"><span data-stu-id="97782-144">string</span></span> | <span data-ttu-id="97782-145">适用于嵌入使用 HTTP POST URL （窗体发布，JS 等。）</span><span class="sxs-lookup"><span data-stu-id="97782-145">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="97782-146">postParameters</span><span class="sxs-lookup"><span data-stu-id="97782-146">postParameters</span></span> | <span data-ttu-id="97782-147">string</span><span class="sxs-lookup"><span data-stu-id="97782-147">string</span></span> | <span data-ttu-id="97782-148">如果使用 postUrl 包括 POST 参数</span><span class="sxs-lookup"><span data-stu-id="97782-148">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="97782-149">GetUrl、 postUrl，或同时可能会返回根据嵌入支持指定的选项的当前状态。</span><span class="sxs-lookup"><span data-stu-id="97782-149">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="97782-150">postParameters 是字符串格式设置为`application/x-www-form-urlencoded`，并且应该相应地设置执行 POST 到 postUrl 内容类型。</span><span class="sxs-lookup"><span data-stu-id="97782-150">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="97782-151">例如：</span><span class="sxs-lookup"><span data-stu-id="97782-151">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="97782-152">页/缩放</span><span class="sxs-lookup"><span data-stu-id="97782-152">Page/zoom</span></span>

<span data-ttu-id="97782-153">页面和缩放选项可能适用于所有预览应用程序，但如果预览应用程序支持将应用。</span><span class="sxs-lookup"><span data-stu-id="97782-153">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
