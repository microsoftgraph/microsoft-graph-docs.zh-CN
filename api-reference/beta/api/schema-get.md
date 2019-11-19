---
title: 获取架构
description: 检索 externalConnection 架构的属性。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: da42ecae79e7e0a81a77edf510a082bb8d3990c2
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703719"
---
# <a name="get-schema"></a><span data-ttu-id="b2849-103">获取架构</span><span class="sxs-lookup"><span data-stu-id="b2849-103">Get schema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2849-104">检索[externalConnection](../resources/externalconnection.md)[架构](../resources/schema.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="b2849-104">Retrieve the properties of a [schema](../resources/schema.md) for an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="b2849-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="b2849-105">Permissions</span></span>

<span data-ttu-id="b2849-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2849-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b2849-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2849-108">Permission type</span></span>                        | <span data-ttu-id="b2849-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2849-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b2849-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2849-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b2849-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2849-111">Not supported.</span></span> |
| <span data-ttu-id="b2849-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2849-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2849-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2849-113">Not supported.</span></span> |
| <span data-ttu-id="b2849-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2849-114">Application</span></span>                            | <span data-ttu-id="b2849-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2849-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2849-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2849-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}/schema
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b2849-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b2849-117">Optional query parameters</span></span>

<span data-ttu-id="b2849-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b2849-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b2849-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b2849-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b2849-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2849-120">Request headers</span></span>

| <span data-ttu-id="b2849-121">名称</span><span class="sxs-lookup"><span data-stu-id="b2849-121">Name</span></span>          | <span data-ttu-id="b2849-122">说明</span><span class="sxs-lookup"><span data-stu-id="b2849-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b2849-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2849-123">Authorization</span></span> | <span data-ttu-id="b2849-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2849-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2849-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2849-126">Request body</span></span>

<span data-ttu-id="b2849-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b2849-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2849-128">响应</span><span class="sxs-lookup"><span data-stu-id="b2849-128">Response</span></span>

<span data-ttu-id="b2849-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[架构](../resources/schema.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b2849-129">If successful, this method returns a `200 OK` response code and the requested [schema](../resources/schema.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b2849-130">示例</span><span class="sxs-lookup"><span data-stu-id="b2849-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b2849-131">请求</span><span class="sxs-lookup"><span data-stu-id="b2849-131">Request</span></span>

<span data-ttu-id="b2849-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b2849-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b2849-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2849-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schema"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections/contosohr/schema
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b2849-134">C#</span><span class="sxs-lookup"><span data-stu-id="b2849-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b2849-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2849-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b2849-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b2849-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="b2849-137">响应</span><span class="sxs-lookup"><span data-stu-id="b2849-137">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="b2849-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b2849-138">The following is an example of the response.</span></span>

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
