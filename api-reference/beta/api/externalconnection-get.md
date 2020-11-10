---
title: 获取连接
description: 检索 externalConnection 的属性和关系。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c32f04e7f373e8955e794d5ce9e4f62a477936cd
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965641"
---
# <a name="get-connection"></a><span data-ttu-id="7f75f-103">获取连接</span><span class="sxs-lookup"><span data-stu-id="7f75f-103">Get connection</span></span>

<span data-ttu-id="7f75f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f75f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f75f-105">检索 [externalConnection](../resources/externalconnection.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7f75f-105">Retrieve the properties and relationships of an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="7f75f-106">权限</span><span class="sxs-lookup"><span data-stu-id="7f75f-106">Permissions</span></span>

<span data-ttu-id="7f75f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f75f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f75f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f75f-109">Permission type</span></span>                        | <span data-ttu-id="7f75f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f75f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7f75f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f75f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f75f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f75f-112">Not supported.</span></span> |
| <span data-ttu-id="7f75f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f75f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f75f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f75f-114">Not supported.</span></span> |
| <span data-ttu-id="7f75f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f75f-115">Application</span></span>                            | <span data-ttu-id="7f75f-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f75f-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f75f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f75f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f75f-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7f75f-118">Optional query parameters</span></span>

<span data-ttu-id="7f75f-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7f75f-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f75f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f75f-120">Request headers</span></span>

| <span data-ttu-id="7f75f-121">名称</span><span class="sxs-lookup"><span data-stu-id="7f75f-121">Name</span></span>          | <span data-ttu-id="7f75f-122">说明</span><span class="sxs-lookup"><span data-stu-id="7f75f-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7f75f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f75f-123">Authorization</span></span> | <span data-ttu-id="7f75f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7f75f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f75f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f75f-126">Request body</span></span>

<span data-ttu-id="7f75f-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7f75f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f75f-128">响应</span><span class="sxs-lookup"><span data-stu-id="7f75f-128">Response</span></span>

<span data-ttu-id="7f75f-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [externalConnection](../resources/externalconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f75f-129">If successful, this method returns a `200 OK` response code and the requested [externalConnection](../resources/externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7f75f-130">示例</span><span class="sxs-lookup"><span data-stu-id="7f75f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7f75f-131">请求</span><span class="sxs-lookup"><span data-stu-id="7f75f-131">Request</span></span>

<span data-ttu-id="7f75f-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7f75f-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f75f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f75f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="7f75f-134">C#</span><span class="sxs-lookup"><span data-stu-id="7f75f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f75f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f75f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f75f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f75f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f75f-137">Java</span><span class="sxs-lookup"><span data-stu-id="7f75f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="7f75f-138">响应</span><span class="sxs-lookup"><span data-stu-id="7f75f-138">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="7f75f-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7f75f-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnection"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system",
  "configuration": {
    "authorizedApps": [
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


