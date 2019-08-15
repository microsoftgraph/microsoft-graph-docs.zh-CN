---
title: 获取协议
description: 检索协议对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: d35785d557c1f9974c389532f4d31f17070ffaa5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408500"
---
# <a name="get-agreement"></a><span data-ttu-id="c2d07-103">获取协议</span><span class="sxs-lookup"><span data-stu-id="c2d07-103">Get agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2d07-104">检索[协议](../resources/agreement.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c2d07-104">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c2d07-105">权限</span><span class="sxs-lookup"><span data-stu-id="c2d07-105">Permissions</span></span>
<span data-ttu-id="c2d07-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2d07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2d07-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2d07-108">Permission type</span></span>                        | <span data-ttu-id="c2d07-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2d07-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2d07-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2d07-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2d07-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2d07-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="c2d07-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2d07-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2d07-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2d07-113">Not supported.</span></span> |
|<span data-ttu-id="c2d07-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2d07-114">Application</span></span>                            | <span data-ttu-id="c2d07-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2d07-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2d07-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2d07-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements/{id}
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="c2d07-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2d07-117">Request headers</span></span>
| <span data-ttu-id="c2d07-118">名称</span><span class="sxs-lookup"><span data-stu-id="c2d07-118">Name</span></span>         | <span data-ttu-id="c2d07-119">类型</span><span class="sxs-lookup"><span data-stu-id="c2d07-119">Type</span></span>        | <span data-ttu-id="c2d07-120">说明</span><span class="sxs-lookup"><span data-stu-id="c2d07-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c2d07-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2d07-121">Authorization</span></span> | <span data-ttu-id="c2d07-122">string</span><span class="sxs-lookup"><span data-stu-id="c2d07-122">string</span></span> | <span data-ttu-id="c2d07-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="c2d07-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2d07-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2d07-125">Request body</span></span>
<span data-ttu-id="c2d07-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c2d07-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c2d07-127">响应</span><span class="sxs-lookup"><span data-stu-id="c2d07-127">Response</span></span>
<span data-ttu-id="c2d07-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[协议](../resources/agreement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c2d07-128">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2d07-129">示例</span><span class="sxs-lookup"><span data-stu-id="c2d07-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2d07-130">请求</span><span class="sxs-lookup"><span data-stu-id="c2d07-130">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c2d07-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c2d07-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```http
GET https://graph.microsoft.com/beta/agreements/{id}?$expand=files
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2d07-132">C#</span><span class="sxs-lookup"><span data-stu-id="c2d07-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2d07-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2d07-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2d07-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="c2d07-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c2d07-135">响应</span><span class="sxs-lookup"><span data-stu-id="c2d07-135">Response</span></span>
><span data-ttu-id="c2d07-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c2d07-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value",
  "files": [
    {
      "id": "id-value",
      "language": "en",
      "fileName": "TOU.pdf",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
