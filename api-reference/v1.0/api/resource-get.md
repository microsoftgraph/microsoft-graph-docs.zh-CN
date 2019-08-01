---
title: 获取资源
description: 检索文件或图像资源对象的二进制数据。
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 97926fe5545b84acf1851643a13ab4cd837d7de8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021608"
---
# <a name="get-resource"></a><span data-ttu-id="7eb78-103">获取资源</span><span class="sxs-lookup"><span data-stu-id="7eb78-103">Get resource</span></span>

<span data-ttu-id="7eb78-104">检索文件或图像[资源](../resources/resource.md)对象的二进制数据。</span><span class="sxs-lookup"><span data-stu-id="7eb78-104">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7eb78-105">权限</span><span class="sxs-lookup"><span data-stu-id="7eb78-105">Permissions</span></span>
<span data-ttu-id="7eb78-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7eb78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7eb78-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7eb78-108">Permission type</span></span>      | <span data-ttu-id="7eb78-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7eb78-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7eb78-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7eb78-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7eb78-111">请参阅 "注意,"、"注释"、"全部"、"全部"、"写"</span><span class="sxs-lookup"><span data-stu-id="7eb78-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="7eb78-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7eb78-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7eb78-113">注意: Read、Notes。读写</span><span class="sxs-lookup"><span data-stu-id="7eb78-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="7eb78-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7eb78-114">Application</span></span> | <span data-ttu-id="7eb78-115">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7eb78-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7eb78-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7eb78-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="7eb78-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7eb78-117">Request headers</span></span>
| <span data-ttu-id="7eb78-118">名称</span><span class="sxs-lookup"><span data-stu-id="7eb78-118">Name</span></span>       | <span data-ttu-id="7eb78-119">类型</span><span class="sxs-lookup"><span data-stu-id="7eb78-119">Type</span></span> | <span data-ttu-id="7eb78-120">说明</span><span class="sxs-lookup"><span data-stu-id="7eb78-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7eb78-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7eb78-121">Authorization</span></span>  | <span data-ttu-id="7eb78-122">string</span><span class="sxs-lookup"><span data-stu-id="7eb78-122">string</span></span>  | <span data-ttu-id="7eb78-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7eb78-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7eb78-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7eb78-125">Request body</span></span>
<span data-ttu-id="7eb78-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7eb78-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7eb78-127">响应</span><span class="sxs-lookup"><span data-stu-id="7eb78-127">Response</span></span>

<span data-ttu-id="7eb78-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和图像或文件二进制数据。</span><span class="sxs-lookup"><span data-stu-id="7eb78-128">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="7eb78-129">注意: 图像不会直接在浏览器中呈现, 因为它们需要授权才能检索它们, 如页面内容的其余部分。</span><span class="sxs-lookup"><span data-stu-id="7eb78-129">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="7eb78-130">示例</span><span class="sxs-lookup"><span data-stu-id="7eb78-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7eb78-131">请求</span><span class="sxs-lookup"><span data-stu-id="7eb78-131">Request</span></span>
<span data-ttu-id="7eb78-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7eb78-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7eb78-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="7eb78-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7eb78-134">C#</span><span class="sxs-lookup"><span data-stu-id="7eb78-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7eb78-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="7eb78-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7eb78-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="7eb78-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7eb78-137">Java</span><span class="sxs-lookup"><span data-stu-id="7eb78-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-resource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7eb78-138">响应</span><span class="sxs-lookup"><span data-stu-id="7eb78-138">Response</span></span>
<span data-ttu-id="7eb78-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7eb78-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.Stream"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

...binary data...
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
