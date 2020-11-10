---
title: 获取架构
description: 检索 externalConnection 架构的属性。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: d27457c3aab9876bc26d95ad2e5f52a1b11bdb79
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975335"
---
# <a name="get-schema"></a><span data-ttu-id="5354e-103">获取架构</span><span class="sxs-lookup"><span data-stu-id="5354e-103">Get schema</span></span>

<span data-ttu-id="5354e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5354e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5354e-105">检索[externalConnection](../resources/externalconnection.md)[架构](../resources/schema.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="5354e-105">Retrieve the properties of a [schema](../resources/schema.md) for an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="5354e-106">权限</span><span class="sxs-lookup"><span data-stu-id="5354e-106">Permissions</span></span>

<span data-ttu-id="5354e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5354e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5354e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5354e-109">Permission type</span></span>                        | <span data-ttu-id="5354e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5354e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5354e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5354e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5354e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="5354e-112">Not supported.</span></span> |
| <span data-ttu-id="5354e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5354e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5354e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5354e-114">Not supported.</span></span> |
| <span data-ttu-id="5354e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5354e-115">Application</span></span>                            | <span data-ttu-id="5354e-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5354e-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5354e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5354e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}/schema
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5354e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5354e-118">Optional query parameters</span></span>

<span data-ttu-id="5354e-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5354e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5354e-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5354e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5354e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5354e-121">Request headers</span></span>

| <span data-ttu-id="5354e-122">名称</span><span class="sxs-lookup"><span data-stu-id="5354e-122">Name</span></span>          | <span data-ttu-id="5354e-123">说明</span><span class="sxs-lookup"><span data-stu-id="5354e-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5354e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5354e-124">Authorization</span></span> | <span data-ttu-id="5354e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5354e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5354e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5354e-127">Request body</span></span>

<span data-ttu-id="5354e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5354e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5354e-129">响应</span><span class="sxs-lookup"><span data-stu-id="5354e-129">Response</span></span>

<span data-ttu-id="5354e-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [架构](../resources/schema.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5354e-130">If successful, this method returns a `200 OK` response code and the requested [schema](../resources/schema.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5354e-131">示例</span><span class="sxs-lookup"><span data-stu-id="5354e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5354e-132">请求</span><span class="sxs-lookup"><span data-stu-id="5354e-132">Request</span></span>

<span data-ttu-id="5354e-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5354e-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5354e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5354e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schema"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections/contosohr/schema
```
# <a name="c"></a>[<span data-ttu-id="5354e-135">C#</span><span class="sxs-lookup"><span data-stu-id="5354e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5354e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5354e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5354e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5354e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5354e-138">Java</span><span class="sxs-lookup"><span data-stu-id="5354e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="5354e-139">响应</span><span class="sxs-lookup"><span data-stu-id="5354e-139">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="5354e-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5354e-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schema"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "baseType": "microsoft.graph.externalItem",
  "properties": [
    {
      "name": "ticketTitle",
      "type": "String",
      "isSearchable": true,
      "isRetrievable": true,
      "labels": [
        "title"
      ]
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": true,
      "isRetrievable": true,
      "isRefinable": true,
      "isSearchable": false
    },
    {
      "name": "assignee",
      "type": "String",
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


