---
title: 获取架构
description: 检索 externalConnection 架构的属性。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: e8efc13fe7cb96b0a820f80974710f5086f1349d
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53466974"
---
# <a name="get-schema"></a><span data-ttu-id="f8346-103">获取架构</span><span class="sxs-lookup"><span data-stu-id="f8346-103">Get schema</span></span>

<span data-ttu-id="f8346-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="f8346-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8346-105">检索[externalConnection](../resources/externalconnectors-externalconnection.md)[架构](../resources/externalconnectors-schema.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="f8346-105">Retrieve the properties of a [schema](../resources/externalconnectors-schema.md) for an [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8346-106">权限</span><span class="sxs-lookup"><span data-stu-id="f8346-106">Permissions</span></span>

<span data-ttu-id="f8346-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8346-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8346-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8346-109">Permission type</span></span>                        | <span data-ttu-id="f8346-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8346-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f8346-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8346-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8346-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8346-112">Not supported.</span></span> |
| <span data-ttu-id="f8346-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8346-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8346-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8346-114">Not supported.</span></span> |
| <span data-ttu-id="f8346-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8346-115">Application</span></span>                            | <span data-ttu-id="f8346-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="f8346-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8346-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8346-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}/schema
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f8346-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f8346-118">Optional query parameters</span></span>

<span data-ttu-id="f8346-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f8346-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f8346-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f8346-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8346-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8346-121">Request headers</span></span>

| <span data-ttu-id="f8346-122">名称</span><span class="sxs-lookup"><span data-stu-id="f8346-122">Name</span></span>          | <span data-ttu-id="f8346-123">说明</span><span class="sxs-lookup"><span data-stu-id="f8346-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f8346-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8346-124">Authorization</span></span> | <span data-ttu-id="f8346-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8346-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8346-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8346-127">Request body</span></span>

<span data-ttu-id="f8346-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f8346-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8346-129">响应</span><span class="sxs-lookup"><span data-stu-id="f8346-129">Response</span></span>

<span data-ttu-id="f8346-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和[](../resources/externalconnectors-schema.md)请求的架构对象。</span><span class="sxs-lookup"><span data-stu-id="f8346-130">If successful, this method returns a `200 OK` response code and the requested [schema](../resources/externalconnectors-schema.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f8346-131">示例</span><span class="sxs-lookup"><span data-stu-id="f8346-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f8346-132">请求</span><span class="sxs-lookup"><span data-stu-id="f8346-132">Request</span></span>

<span data-ttu-id="f8346-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f8346-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f8346-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8346-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schema"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections/contosohr/schema
```
# <a name="c"></a>[<span data-ttu-id="f8346-135">C#</span><span class="sxs-lookup"><span data-stu-id="f8346-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8346-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8346-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8346-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8346-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f8346-138">Java</span><span class="sxs-lookup"><span data-stu-id="f8346-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="f8346-139">响应</span><span class="sxs-lookup"><span data-stu-id="f8346-139">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="f8346-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f8346-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.schema"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "ticketTitle",
      "type": "string",
      "isSearchable": true,
      "isRetrievable": true,
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "string",
      "isQueryable": true,
      "isRetrievable": true,
      "isRefinable": true,
      "isSearchable": false
    },
    {
      "name": "assignee",
      "type": "string",
      "isRetrievable": true
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get schema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


