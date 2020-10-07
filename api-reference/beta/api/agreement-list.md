---
title: 列出协议
description: 检索协议对象的列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: cb32bfbacbc5f8148343873f8ae6b67cd817ca5d
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48371195"
---
# <a name="list-agreements"></a><span data-ttu-id="801d4-103">列出协议</span><span class="sxs-lookup"><span data-stu-id="801d4-103">List agreements</span></span>

<span data-ttu-id="801d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="801d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="801d4-105">检索 [协议](../resources/agreement.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="801d4-105">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="801d4-106">权限</span><span class="sxs-lookup"><span data-stu-id="801d4-106">Permissions</span></span>
<span data-ttu-id="801d4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="801d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="801d4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="801d4-109">Permission type</span></span>                        | <span data-ttu-id="801d4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="801d4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="801d4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="801d4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="801d4-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="801d4-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="801d4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="801d4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="801d4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="801d4-114">Not supported.</span></span> |
|<span data-ttu-id="801d4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="801d4-115">Application</span></span>                            | <span data-ttu-id="801d4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="801d4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="801d4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="801d4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="801d4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="801d4-118">Request headers</span></span>
| <span data-ttu-id="801d4-119">名称</span><span class="sxs-lookup"><span data-stu-id="801d4-119">Name</span></span>         | <span data-ttu-id="801d4-120">类型</span><span class="sxs-lookup"><span data-stu-id="801d4-120">Type</span></span>        | <span data-ttu-id="801d4-121">说明</span><span class="sxs-lookup"><span data-stu-id="801d4-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="801d4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="801d4-122">Authorization</span></span> | <span data-ttu-id="801d4-123">string</span><span class="sxs-lookup"><span data-stu-id="801d4-123">string</span></span> | <span data-ttu-id="801d4-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="801d4-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="801d4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="801d4-126">Request body</span></span>
<span data-ttu-id="801d4-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="801d4-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="801d4-128">响应</span><span class="sxs-lookup"><span data-stu-id="801d4-128">Response</span></span>
<span data-ttu-id="801d4-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [协议](../resources/agreement.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="801d4-129">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="801d4-130">示例</span><span class="sxs-lookup"><span data-stu-id="801d4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="801d4-131">请求</span><span class="sxs-lookup"><span data-stu-id="801d4-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="801d4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="801d4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/agreements
```
# <a name="c"></a>[<span data-ttu-id="801d4-133">C#</span><span class="sxs-lookup"><span data-stu-id="801d4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="801d4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="801d4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="801d4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="801d4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="801d4-136">响应</span><span class="sxs-lookup"><span data-stu-id="801d4-136">Response</span></span>
><span data-ttu-id="801d4-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="801d4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "value": [
    {
      "displayName": "displayName-value",
      "isViewingBeforeAcceptanceRequired": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
