---
title: 获取资源
description: 检索文件或图像资源对象的二进制数据。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 2026bb116ee760dfe63ae1f068344c7901634862
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085449"
---
# <a name="get-resource"></a><span data-ttu-id="7f673-103">获取资源</span><span class="sxs-lookup"><span data-stu-id="7f673-103">Get resource</span></span>

<span data-ttu-id="7f673-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f673-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f673-105">检索文件或图像 [资源](../resources/onenoteresource.md) 对象的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="7f673-105">Retrieve the binary data of a file or image [resource](../resources/onenoteresource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7f673-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7f673-106">Permissions</span></span>
<span data-ttu-id="7f673-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f673-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f673-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f673-109">Permission type</span></span>      | <span data-ttu-id="7f673-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f673-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f673-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f673-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7f673-112">请参阅 "注意，"、"注释"、"全部"、"全部"、"写"</span><span class="sxs-lookup"><span data-stu-id="7f673-112">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f673-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f673-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f673-114">注意： Read、Notes。读写</span><span class="sxs-lookup"><span data-stu-id="7f673-114">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="7f673-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f673-115">Application</span></span> | <span data-ttu-id="7f673-116">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f673-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f673-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f673-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="7f673-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f673-118">Request headers</span></span>
| <span data-ttu-id="7f673-119">名称</span><span class="sxs-lookup"><span data-stu-id="7f673-119">Name</span></span>       | <span data-ttu-id="7f673-120">类型</span><span class="sxs-lookup"><span data-stu-id="7f673-120">Type</span></span> | <span data-ttu-id="7f673-121">说明</span><span class="sxs-lookup"><span data-stu-id="7f673-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7f673-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f673-122">Authorization</span></span>  | <span data-ttu-id="7f673-123">string</span><span class="sxs-lookup"><span data-stu-id="7f673-123">string</span></span>  | <span data-ttu-id="7f673-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7f673-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f673-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f673-126">Request body</span></span>
<span data-ttu-id="7f673-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7f673-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f673-128">响应</span><span class="sxs-lookup"><span data-stu-id="7f673-128">Response</span></span>

<span data-ttu-id="7f673-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和图像或文件二进制数据。</span><span class="sxs-lookup"><span data-stu-id="7f673-129">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="7f673-130">注意：图像不会直接在浏览器中呈现，因为它们需要授权才能检索它们，如页面内容的其余部分。</span><span class="sxs-lookup"><span data-stu-id="7f673-130">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="7f673-131">示例</span><span class="sxs-lookup"><span data-stu-id="7f673-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f673-132">请求</span><span class="sxs-lookup"><span data-stu-id="7f673-132">Request</span></span>
<span data-ttu-id="7f673-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7f673-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f673-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f673-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/onenote/resources/{id}/content
```
# <a name="c"></a>[<span data-ttu-id="7f673-135">C#</span><span class="sxs-lookup"><span data-stu-id="7f673-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f673-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f673-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f673-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f673-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7f673-138">响应</span><span class="sxs-lookup"><span data-stu-id="7f673-138">Response</span></span>
<span data-ttu-id="7f673-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7f673-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

...binary data...
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


