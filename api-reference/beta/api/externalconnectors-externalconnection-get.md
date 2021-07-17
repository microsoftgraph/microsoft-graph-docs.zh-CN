---
title: 获取连接
description: 检索 externalConnection 的属性和关系。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 5f545343bc67b20fab59d48cce21077769c2960a
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467585"
---
# <a name="get-connection"></a><span data-ttu-id="c5750-103">获取连接</span><span class="sxs-lookup"><span data-stu-id="c5750-103">Get connection</span></span>

<span data-ttu-id="c5750-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="c5750-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5750-105">检索 [externalConnection 的属性和关系](../resources/externalconnectors-externalconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="c5750-105">Retrieve the properties and relationships of an [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c5750-106">权限</span><span class="sxs-lookup"><span data-stu-id="c5750-106">Permissions</span></span>

<span data-ttu-id="c5750-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5750-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c5750-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5750-109">Permission type</span></span>                        | <span data-ttu-id="c5750-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5750-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c5750-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5750-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c5750-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5750-112">Not supported.</span></span> |
| <span data-ttu-id="c5750-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5750-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5750-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5750-114">Not supported.</span></span> |
| <span data-ttu-id="c5750-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5750-115">Application</span></span>                            | <span data-ttu-id="c5750-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="c5750-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5750-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5750-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c5750-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c5750-118">Optional query parameters</span></span>

<span data-ttu-id="c5750-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c5750-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5750-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5750-120">Request headers</span></span>

| <span data-ttu-id="c5750-121">名称</span><span class="sxs-lookup"><span data-stu-id="c5750-121">Name</span></span>          | <span data-ttu-id="c5750-122">说明</span><span class="sxs-lookup"><span data-stu-id="c5750-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c5750-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5750-123">Authorization</span></span> | <span data-ttu-id="c5750-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5750-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5750-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5750-126">Request body</span></span>

<span data-ttu-id="c5750-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c5750-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5750-128">响应</span><span class="sxs-lookup"><span data-stu-id="c5750-128">Response</span></span>

<span data-ttu-id="c5750-129">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [externalConnection](../resources/externalconnectors-externalconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c5750-129">If successful, this method returns a `200 OK` response code and the requested [externalConnection](../resources/externalconnectors-externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c5750-130">示例</span><span class="sxs-lookup"><span data-stu-id="c5750-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c5750-131">请求</span><span class="sxs-lookup"><span data-stu-id="c5750-131">Request</span></span>

<span data-ttu-id="c5750-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c5750-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c5750-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c5750-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="c5750-134">C#</span><span class="sxs-lookup"><span data-stu-id="c5750-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c5750-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c5750-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c5750-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c5750-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c5750-137">Java</span><span class="sxs-lookup"><span data-stu-id="c5750-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="c5750-138">响应</span><span class="sxs-lookup"><span data-stu-id="c5750-138">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="c5750-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c5750-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get connection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
