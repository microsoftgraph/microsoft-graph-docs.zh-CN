---
title: 获取架构
description: 检索 externalConnection 架构的属性。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 6cf448a92f7ff1277f866beb23753e83de8f2ffd
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938392"
---
# <a name="get-schema"></a><span data-ttu-id="f630d-103">获取架构</span><span class="sxs-lookup"><span data-stu-id="f630d-103">Get schema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f630d-104">检索[externalConnection](../resources/externalconnection.md)[架构](../resources/schema.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="f630d-104">Retrieve the properties of a [schema](../resources/schema.md) for an [externalConnection](../resources/externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f630d-105">权限</span><span class="sxs-lookup"><span data-stu-id="f630d-105">Permissions</span></span>

<span data-ttu-id="f630d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f630d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f630d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f630d-108">Permission type</span></span>                        | <span data-ttu-id="f630d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f630d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f630d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f630d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f630d-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="f630d-111">Not supported.</span></span> |
| <span data-ttu-id="f630d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f630d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f630d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f630d-113">Not supported.</span></span> |
| <span data-ttu-id="f630d-114">Application</span><span class="sxs-lookup"><span data-stu-id="f630d-114">Application</span></span>                            | <span data-ttu-id="f630d-115">ExternalItem</span><span class="sxs-lookup"><span data-stu-id="f630d-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f630d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f630d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}/schema
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f630d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f630d-117">Optional query parameters</span></span>

<span data-ttu-id="f630d-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f630d-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f630d-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f630d-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f630d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f630d-120">Request headers</span></span>

| <span data-ttu-id="f630d-121">名称</span><span class="sxs-lookup"><span data-stu-id="f630d-121">Name</span></span>          | <span data-ttu-id="f630d-122">说明</span><span class="sxs-lookup"><span data-stu-id="f630d-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f630d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f630d-123">Authorization</span></span> | <span data-ttu-id="f630d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f630d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f630d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f630d-126">Request body</span></span>

<span data-ttu-id="f630d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f630d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f630d-128">响应</span><span class="sxs-lookup"><span data-stu-id="f630d-128">Response</span></span>

<span data-ttu-id="f630d-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[架构](../resources/schema.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f630d-129">If successful, this method returns a `200 OK` response code and the requested [schema](../resources/schema.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f630d-130">示例</span><span class="sxs-lookup"><span data-stu-id="f630d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f630d-131">请求</span><span class="sxs-lookup"><span data-stu-id="f630d-131">Request</span></span>

<span data-ttu-id="f630d-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f630d-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schema"
}-->

```http
GET https://graph.microsoft.com/beta/external/connections/contosohr/schema
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="f630d-133">响应</span><span class="sxs-lookup"><span data-stu-id="f630d-133">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="f630d-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f630d-134">The following is an example of the response.</span></span>

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
