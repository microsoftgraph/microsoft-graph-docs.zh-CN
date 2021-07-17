---
title: 列出连接
description: 检索 externalConnections 列表。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 5237fd7450bb2c289247a1343b8fd16dba1e8ae5
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467584"
---
# <a name="list-connections"></a><span data-ttu-id="16b85-103">列出连接</span><span class="sxs-lookup"><span data-stu-id="16b85-103">List connections</span></span>

<span data-ttu-id="16b85-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="16b85-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16b85-105">检索 [externalConnections 的列表](../resources/externalconnectors-externalconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="16b85-105">Retrieve a list of [externalConnections](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="16b85-106">权限</span><span class="sxs-lookup"><span data-stu-id="16b85-106">Permissions</span></span>

<span data-ttu-id="16b85-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="16b85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="16b85-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="16b85-109">Permission type</span></span>                        | <span data-ttu-id="16b85-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="16b85-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="16b85-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16b85-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="16b85-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="16b85-112">Not supported.</span></span> |
| <span data-ttu-id="16b85-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16b85-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16b85-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="16b85-114">Not supported.</span></span> |
| <span data-ttu-id="16b85-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="16b85-115">Application</span></span>                            | <span data-ttu-id="16b85-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="16b85-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="16b85-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16b85-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16b85-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="16b85-118">Optional query parameters</span></span>

<span data-ttu-id="16b85-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="16b85-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16b85-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="16b85-120">Request headers</span></span>

| <span data-ttu-id="16b85-121">名称</span><span class="sxs-lookup"><span data-stu-id="16b85-121">Name</span></span>          | <span data-ttu-id="16b85-122">说明</span><span class="sxs-lookup"><span data-stu-id="16b85-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="16b85-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="16b85-123">Authorization</span></span> | <span data-ttu-id="16b85-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="16b85-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16b85-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="16b85-126">Request body</span></span>

<span data-ttu-id="16b85-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="16b85-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16b85-128">响应</span><span class="sxs-lookup"><span data-stu-id="16b85-128">Response</span></span>

<span data-ttu-id="16b85-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [externalConnection](../resources/externalconnectors-externalconnection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="16b85-129">If successful, this method returns a `200 OK` response code and a collection of [externalConnection](../resources/externalconnectors-externalconnection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="16b85-130">示例</span><span class="sxs-lookup"><span data-stu-id="16b85-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="16b85-131">请求</span><span class="sxs-lookup"><span data-stu-id="16b85-131">Request</span></span>

<span data-ttu-id="16b85-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="16b85-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="16b85-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="16b85-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connections"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections
```
# <a name="c"></a>[<span data-ttu-id="16b85-134">C#</span><span class="sxs-lookup"><span data-stu-id="16b85-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16b85-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16b85-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16b85-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16b85-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16b85-137">Java</span><span class="sxs-lookup"><span data-stu-id="16b85-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="16b85-138">响应</span><span class="sxs-lookup"><span data-stu-id="16b85-138">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="16b85-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="16b85-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contosohr",
      "name": "Contoso HR",
      "description": "Connection to index Contoso HR system",
      "state": "ready",
      "configuration": {
        "authorizedAppIds": [
          "d310d35d-72ec-47dd-92f2-fb9c40936555"
        ]
      }
    },
    {
      "id": "contosofinance",
      "name": "Contoso Finance",
      "description": "Connection to index Contoso Finance system",
      "state": "ready",
      "configuration": {
        "authorizedAppIds": [
          "fbdc7d4e-07f4-4143-8258-e5a2fcebeadb"
        ]
      }
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List connections",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
