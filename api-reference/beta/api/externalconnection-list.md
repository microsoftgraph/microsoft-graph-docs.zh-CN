---
title: 列出连接
description: 检索 externalConnections 的列表。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b70e1fc69c5897e8209633e5b5ce0f35cb7fb41a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965628"
---
# <a name="list-connections"></a><span data-ttu-id="9afc8-103">列出连接</span><span class="sxs-lookup"><span data-stu-id="9afc8-103">List connections</span></span>

<span data-ttu-id="9afc8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9afc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9afc8-105">检索 [externalConnections](../resources/externalconnection.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="9afc8-105">Retrieve a list of [externalConnections](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="9afc8-106">权限</span><span class="sxs-lookup"><span data-stu-id="9afc8-106">Permissions</span></span>

<span data-ttu-id="9afc8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9afc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9afc8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9afc8-109">Permission type</span></span>                        | <span data-ttu-id="9afc8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9afc8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9afc8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9afc8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9afc8-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="9afc8-112">Not supported.</span></span> |
| <span data-ttu-id="9afc8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9afc8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9afc8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9afc8-114">Not supported.</span></span> |
| <span data-ttu-id="9afc8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9afc8-115">Application</span></span>                            | <span data-ttu-id="9afc8-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9afc8-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9afc8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9afc8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9afc8-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9afc8-118">Optional query parameters</span></span>

<span data-ttu-id="9afc8-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9afc8-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9afc8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9afc8-120">Request headers</span></span>

| <span data-ttu-id="9afc8-121">名称</span><span class="sxs-lookup"><span data-stu-id="9afc8-121">Name</span></span>          | <span data-ttu-id="9afc8-122">说明</span><span class="sxs-lookup"><span data-stu-id="9afc8-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9afc8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9afc8-123">Authorization</span></span> | <span data-ttu-id="9afc8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9afc8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9afc8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9afc8-126">Request body</span></span>

<span data-ttu-id="9afc8-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9afc8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9afc8-128">响应</span><span class="sxs-lookup"><span data-stu-id="9afc8-128">Response</span></span>

<span data-ttu-id="9afc8-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [externalConnection](../resources/externalconnection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9afc8-129">If successful, this method returns a `200 OK` response code and a collection of [externalConnection](../resources/externalconnection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9afc8-130">示例</span><span class="sxs-lookup"><span data-stu-id="9afc8-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9afc8-131">请求</span><span class="sxs-lookup"><span data-stu-id="9afc8-131">Request</span></span>

<span data-ttu-id="9afc8-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9afc8-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9afc8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9afc8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connections"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections
```
# <a name="c"></a>[<span data-ttu-id="9afc8-134">C#</span><span class="sxs-lookup"><span data-stu-id="9afc8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9afc8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9afc8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9afc8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9afc8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9afc8-137">Java</span><span class="sxs-lookup"><span data-stu-id="9afc8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="9afc8-138">响应</span><span class="sxs-lookup"><span data-stu-id="9afc8-138">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="9afc8-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9afc8-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnection",
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
      "configuration": {
        "authorizedApps": [
          "d310d35d-72ec-47dd-92f2-fb9c40936555"
        ]
      }
    },
    {
      "id": "contosofinance",
      "name": "Contoso Finance",
      "description": "Connection to index Contoso Finance system",
      "configuration": {
        "authorizedApps": [
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


