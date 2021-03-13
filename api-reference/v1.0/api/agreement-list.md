---
title: 列出协议
description: 检索协议对象的列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 90d4421342a74b6d89bae2e02c9a61535ce40a29
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775211"
---
# <a name="list-agreements"></a><span data-ttu-id="38de5-103">列出协议</span><span class="sxs-lookup"><span data-stu-id="38de5-103">List agreements</span></span>

<span data-ttu-id="38de5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38de5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="38de5-105">检索协议 [对象](../resources/agreement.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="38de5-105">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="38de5-106">权限</span><span class="sxs-lookup"><span data-stu-id="38de5-106">Permissions</span></span>
<span data-ttu-id="38de5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38de5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38de5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="38de5-109">Permission type</span></span>                        | <span data-ttu-id="38de5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38de5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="38de5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38de5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="38de5-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="38de5-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="38de5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38de5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38de5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="38de5-114">Not supported.</span></span> |
|<span data-ttu-id="38de5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="38de5-115">Application</span></span>                            | <span data-ttu-id="38de5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="38de5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="38de5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38de5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38de5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="38de5-118">Optional query parameters</span></span>
<span data-ttu-id="38de5-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="38de5-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38de5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="38de5-120">Request headers</span></span>
| <span data-ttu-id="38de5-121">名称</span><span class="sxs-lookup"><span data-stu-id="38de5-121">Name</span></span>         | <span data-ttu-id="38de5-122">类型</span><span class="sxs-lookup"><span data-stu-id="38de5-122">Type</span></span>        | <span data-ttu-id="38de5-123">说明</span><span class="sxs-lookup"><span data-stu-id="38de5-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="38de5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="38de5-124">Authorization</span></span> | <span data-ttu-id="38de5-125">string</span><span class="sxs-lookup"><span data-stu-id="38de5-125">string</span></span> | <span data-ttu-id="38de5-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="38de5-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38de5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="38de5-128">Request body</span></span>
<span data-ttu-id="38de5-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="38de5-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="38de5-130">响应</span><span class="sxs-lookup"><span data-stu-id="38de5-130">Response</span></span>
<span data-ttu-id="38de5-131">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码 [和 agreement](../resources/agreement.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="38de5-131">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="38de5-132">示例</span><span class="sxs-lookup"><span data-stu-id="38de5-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="38de5-133">请求</span><span class="sxs-lookup"><span data-stu-id="38de5-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="38de5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="38de5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements
```
# <a name="c"></a>[<span data-ttu-id="38de5-135">C#</span><span class="sxs-lookup"><span data-stu-id="38de5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38de5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38de5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38de5-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38de5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38de5-138">Java</span><span class="sxs-lookup"><span data-stu-id="38de5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="38de5-139">响应</span><span class="sxs-lookup"><span data-stu-id="38de5-139">Response</span></span>
><span data-ttu-id="38de5-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="38de5-140">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
      "displayName": "Sample ToU",
      "isViewingBeforeAcceptanceRequired": true,
      "id": "093b947f-8363-4979-a47d-4c52b33ee1be"
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
