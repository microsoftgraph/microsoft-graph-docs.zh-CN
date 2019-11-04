---
title: 获取连接
description: 检索 externalConnection 的属性和关系。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 6fbaa527597ebdbda4b8006e8af31da1502422e7
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938665"
---
# <a name="get-connection"></a><span data-ttu-id="3c827-103">获取连接</span><span class="sxs-lookup"><span data-stu-id="3c827-103">Get connection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c827-104">检索[externalConnection](../resources/externalconnection.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3c827-104">Retrieve the properties and relationships of an [externalConnection](../resources/externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3c827-105">权限</span><span class="sxs-lookup"><span data-stu-id="3c827-105">Permissions</span></span>

<span data-ttu-id="3c827-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c827-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3c827-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c827-108">Permission type</span></span>                        | <span data-ttu-id="3c827-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c827-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3c827-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c827-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c827-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c827-111">Not supported.</span></span> |
| <span data-ttu-id="3c827-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c827-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c827-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c827-113">Not supported.</span></span> |
| <span data-ttu-id="3c827-114">Application</span><span class="sxs-lookup"><span data-stu-id="3c827-114">Application</span></span>                            | <span data-ttu-id="3c827-115">ExternalItem</span><span class="sxs-lookup"><span data-stu-id="3c827-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c827-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c827-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c827-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3c827-117">Optional query parameters</span></span>

<span data-ttu-id="3c827-118">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3c827-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c827-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c827-119">Request headers</span></span>

| <span data-ttu-id="3c827-120">名称</span><span class="sxs-lookup"><span data-stu-id="3c827-120">Name</span></span>          | <span data-ttu-id="3c827-121">说明</span><span class="sxs-lookup"><span data-stu-id="3c827-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="3c827-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c827-122">Authorization</span></span> | <span data-ttu-id="3c827-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3c827-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c827-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c827-125">Request body</span></span>

<span data-ttu-id="3c827-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3c827-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c827-127">响应</span><span class="sxs-lookup"><span data-stu-id="3c827-127">Response</span></span>

<span data-ttu-id="3c827-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[externalConnection](../resources/externalconnection.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3c827-128">If successful, this method returns a `200 OK` response code and the requested [externalConnection](../resources/externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c827-129">示例</span><span class="sxs-lookup"><span data-stu-id="3c827-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3c827-130">请求</span><span class="sxs-lookup"><span data-stu-id="3c827-130">Request</span></span>

<span data-ttu-id="3c827-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3c827-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connection"
}-->

```http
GET https://graph.microsoft.com/beta/connections/contosohr
```

<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="3c827-132">响应</span><span class="sxs-lookup"><span data-stu-id="3c827-132">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="3c827-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3c827-133">The following is an example of the response.</span></span>

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
