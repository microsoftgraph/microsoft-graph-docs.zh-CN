---
title: 获取资源
description: 检索文件或图像 resource 对象的二进制数据。
localization_priority: Normal
ms.openlocfilehash: 1f8150e0449009eef4d1afe2ce014ae848153382
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841256"
---
# <a name="get-resource"></a><span data-ttu-id="ca349-103">获取资源</span><span class="sxs-lookup"><span data-stu-id="ca349-103">Get resource</span></span>

> <span data-ttu-id="ca349-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ca349-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca349-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ca349-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca349-106">检索文件或图像 [resource](../resources/resource.md) 对象的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="ca349-106">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ca349-107">权限</span><span class="sxs-lookup"><span data-stu-id="ca349-107">Permissions</span></span>
<span data-ttu-id="ca349-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca349-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca349-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca349-110">Permission type</span></span>      | <span data-ttu-id="ca349-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca349-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca349-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca349-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ca349-113">Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca349-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ca349-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca349-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca349-115">Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ca349-115">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ca349-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca349-116">Application</span></span> | <span data-ttu-id="ca349-117">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca349-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca349-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca349-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="ca349-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca349-119">Request headers</span></span>
| <span data-ttu-id="ca349-120">名称</span><span class="sxs-lookup"><span data-stu-id="ca349-120">Name</span></span>       | <span data-ttu-id="ca349-121">类型</span><span class="sxs-lookup"><span data-stu-id="ca349-121">Type</span></span> | <span data-ttu-id="ca349-122">说明</span><span class="sxs-lookup"><span data-stu-id="ca349-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ca349-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca349-123">Authorization</span></span>  | <span data-ttu-id="ca349-124">string</span><span class="sxs-lookup"><span data-stu-id="ca349-124">string</span></span>  | <span data-ttu-id="ca349-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca349-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca349-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca349-127">Request body</span></span>
<span data-ttu-id="ca349-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ca349-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca349-129">响应</span><span class="sxs-lookup"><span data-stu-id="ca349-129">Response</span></span>

<span data-ttu-id="ca349-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和图像或文件二进制数据。</span><span class="sxs-lookup"><span data-stu-id="ca349-130">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="ca349-131">注意：图像无法直接在浏览器中呈现，因为与页面内容的其他部分一样，检索它们需要授权。</span><span class="sxs-lookup"><span data-stu-id="ca349-131">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="ca349-132">示例</span><span class="sxs-lookup"><span data-stu-id="ca349-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca349-133">请求</span><span class="sxs-lookup"><span data-stu-id="ca349-133">Request</span></span>
<span data-ttu-id="ca349-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca349-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="ca349-135">响应</span><span class="sxs-lookup"><span data-stu-id="ca349-135">Response</span></span>
<span data-ttu-id="ca349-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ca349-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK

...binary data...
```
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.onenoteResource"
} -->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
