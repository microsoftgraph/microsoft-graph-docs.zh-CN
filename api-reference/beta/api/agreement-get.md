---
title: 获取协议
description: 检索协议对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 39d99236ec59b38a72a98524bc3211aa616f0bce
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773996"
---
# <a name="get-agreement"></a><span data-ttu-id="814e1-103">获取协议</span><span class="sxs-lookup"><span data-stu-id="814e1-103">Get agreement</span></span>

<span data-ttu-id="814e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="814e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="814e1-105">检索协议对象的属性 [和](../resources/agreement.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="814e1-105">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="814e1-106">权限</span><span class="sxs-lookup"><span data-stu-id="814e1-106">Permissions</span></span>
<span data-ttu-id="814e1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="814e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="814e1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="814e1-109">Permission type</span></span>                        | <span data-ttu-id="814e1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="814e1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="814e1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="814e1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="814e1-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="814e1-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="814e1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="814e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="814e1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="814e1-114">Not supported.</span></span> |
|<span data-ttu-id="814e1-115">Application</span><span class="sxs-lookup"><span data-stu-id="814e1-115">Application</span></span>                            | <span data-ttu-id="814e1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="814e1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="814e1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="814e1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements/{id}
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="814e1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="814e1-118">Request headers</span></span>
| <span data-ttu-id="814e1-119">名称</span><span class="sxs-lookup"><span data-stu-id="814e1-119">Name</span></span>         | <span data-ttu-id="814e1-120">类型</span><span class="sxs-lookup"><span data-stu-id="814e1-120">Type</span></span>        | <span data-ttu-id="814e1-121">说明</span><span class="sxs-lookup"><span data-stu-id="814e1-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="814e1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="814e1-122">Authorization</span></span> | <span data-ttu-id="814e1-123">string</span><span class="sxs-lookup"><span data-stu-id="814e1-123">string</span></span> | <span data-ttu-id="814e1-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="814e1-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="814e1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="814e1-126">Request body</span></span>
<span data-ttu-id="814e1-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="814e1-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="814e1-128">响应</span><span class="sxs-lookup"><span data-stu-id="814e1-128">Response</span></span>
<span data-ttu-id="814e1-129">如果成功，此方法在响应 `200 OK` 正文中返回 [响应](../resources/agreement.md) 代码和 agreement 对象。</span><span class="sxs-lookup"><span data-stu-id="814e1-129">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="814e1-130">示例</span><span class="sxs-lookup"><span data-stu-id="814e1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="814e1-131">请求</span><span class="sxs-lookup"><span data-stu-id="814e1-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="814e1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="814e1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/{id}?$expand=files
```
# <a name="c"></a>[<span data-ttu-id="814e1-133">C#</span><span class="sxs-lookup"><span data-stu-id="814e1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="814e1-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="814e1-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="814e1-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="814e1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="814e1-136">Java</span><span class="sxs-lookup"><span data-stu-id="814e1-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="814e1-137">响应</span><span class="sxs-lookup"><span data-stu-id="814e1-137">Response</span></span>
><span data-ttu-id="814e1-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="814e1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
