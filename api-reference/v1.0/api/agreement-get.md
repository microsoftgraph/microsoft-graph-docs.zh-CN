---
title: 获取协议
description: 检索协议对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 9ef1bf8cd56cd603b685949a28a04e08d4ecb364
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775243"
---
# <a name="get-agreement"></a><span data-ttu-id="0f28c-103">获取协议</span><span class="sxs-lookup"><span data-stu-id="0f28c-103">Get agreement</span></span>

<span data-ttu-id="0f28c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f28c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f28c-105">检索协议对象的属性 [和](../resources/agreement.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="0f28c-105">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0f28c-106">权限</span><span class="sxs-lookup"><span data-stu-id="0f28c-106">Permissions</span></span>
<span data-ttu-id="0f28c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f28c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f28c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f28c-109">Permission type</span></span>                        | <span data-ttu-id="0f28c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0f28c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f28c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f28c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f28c-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f28c-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="0f28c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f28c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f28c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f28c-114">Not supported.</span></span> |
|<span data-ttu-id="0f28c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f28c-115">Application</span></span>                            | <span data-ttu-id="0f28c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f28c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f28c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f28c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0f28c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0f28c-118">Optional query parameters</span></span>
<span data-ttu-id="0f28c-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0f28c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f28c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f28c-120">Request headers</span></span>
| <span data-ttu-id="0f28c-121">名称</span><span class="sxs-lookup"><span data-stu-id="0f28c-121">Name</span></span>         | <span data-ttu-id="0f28c-122">类型</span><span class="sxs-lookup"><span data-stu-id="0f28c-122">Type</span></span>        | <span data-ttu-id="0f28c-123">说明</span><span class="sxs-lookup"><span data-stu-id="0f28c-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0f28c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f28c-124">Authorization</span></span> | <span data-ttu-id="0f28c-125">string</span><span class="sxs-lookup"><span data-stu-id="0f28c-125">string</span></span> | <span data-ttu-id="0f28c-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="0f28c-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0f28c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f28c-128">Request body</span></span>
<span data-ttu-id="0f28c-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0f28c-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0f28c-130">响应</span><span class="sxs-lookup"><span data-stu-id="0f28c-130">Response</span></span>
<span data-ttu-id="0f28c-131">如果成功，此方法在响应 `200 OK` 正文中返回 [响应](../resources/agreement.md) 代码和 agreement 对象。</span><span class="sxs-lookup"><span data-stu-id="0f28c-131">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0f28c-132">示例</span><span class="sxs-lookup"><span data-stu-id="0f28c-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="0f28c-133">请求</span><span class="sxs-lookup"><span data-stu-id="0f28c-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0f28c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f28c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements/093b947f-8363-4979-a47d-4c52b33ee1be?$expand=files
```
# <a name="c"></a>[<span data-ttu-id="0f28c-135">C#</span><span class="sxs-lookup"><span data-stu-id="0f28c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0f28c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f28c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f28c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f28c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0f28c-138">Java</span><span class="sxs-lookup"><span data-stu-id="0f28c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0f28c-139">响应</span><span class="sxs-lookup"><span data-stu-id="0f28c-139">Response</span></span>
><span data-ttu-id="0f28c-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0f28c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
      "id": "093b947f-8363-4979-a47d-4c52b33ee1be",
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
