---
title: 获取架构
description: 检索 externalConnection 架构的属性。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: de4e793a224466738773f959892a31b002737f92
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453763"
---
# <a name="get-schema"></a><span data-ttu-id="52bb0-103">获取架构</span><span class="sxs-lookup"><span data-stu-id="52bb0-103">Get schema</span></span>

<span data-ttu-id="52bb0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52bb0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52bb0-105">检索[externalConnection](../resources/externalconnection.md)[架构](../resources/schema.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="52bb0-105">Retrieve the properties of a [schema](../resources/schema.md) for an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="52bb0-106">权限</span><span class="sxs-lookup"><span data-stu-id="52bb0-106">Permissions</span></span>

<span data-ttu-id="52bb0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="52bb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="52bb0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="52bb0-109">Permission type</span></span>                        | <span data-ttu-id="52bb0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="52bb0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="52bb0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="52bb0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="52bb0-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="52bb0-112">Not supported.</span></span> |
| <span data-ttu-id="52bb0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="52bb0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52bb0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="52bb0-114">Not supported.</span></span> |
| <span data-ttu-id="52bb0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="52bb0-115">Application</span></span>                            | <span data-ttu-id="52bb0-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52bb0-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="52bb0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="52bb0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}/schema
```

## <a name="optional-query-parameters"></a><span data-ttu-id="52bb0-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="52bb0-118">Optional query parameters</span></span>

<span data-ttu-id="52bb0-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="52bb0-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="52bb0-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="52bb0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="52bb0-121">请求头</span><span class="sxs-lookup"><span data-stu-id="52bb0-121">Request headers</span></span>

| <span data-ttu-id="52bb0-122">名称</span><span class="sxs-lookup"><span data-stu-id="52bb0-122">Name</span></span>          | <span data-ttu-id="52bb0-123">说明</span><span class="sxs-lookup"><span data-stu-id="52bb0-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="52bb0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="52bb0-124">Authorization</span></span> | <span data-ttu-id="52bb0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="52bb0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52bb0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="52bb0-127">Request body</span></span>

<span data-ttu-id="52bb0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="52bb0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52bb0-129">响应</span><span class="sxs-lookup"><span data-stu-id="52bb0-129">Response</span></span>

<span data-ttu-id="52bb0-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[架构](../resources/schema.md)对象。</span><span class="sxs-lookup"><span data-stu-id="52bb0-130">If successful, this method returns a `200 OK` response code and the requested [schema](../resources/schema.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="52bb0-131">示例</span><span class="sxs-lookup"><span data-stu-id="52bb0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="52bb0-132">请求</span><span class="sxs-lookup"><span data-stu-id="52bb0-132">Request</span></span>

<span data-ttu-id="52bb0-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="52bb0-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52bb0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="52bb0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schema"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections/contosohr/schema
```
# <a name="c"></a>[<span data-ttu-id="52bb0-135">C#</span><span class="sxs-lookup"><span data-stu-id="52bb0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52bb0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52bb0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52bb0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52bb0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="52bb0-138">响应</span><span class="sxs-lookup"><span data-stu-id="52bb0-138">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="52bb0-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="52bb0-139">The following is an example of the response.</span></span>

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
      "name": "title",
      "type": "String",
      "isSearchable": true,
      "isRetrievable": true
    },
    {
      "name": "priority",
      "type": "String",
      "isQueryable": true,
      "isRetrievable": true
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
