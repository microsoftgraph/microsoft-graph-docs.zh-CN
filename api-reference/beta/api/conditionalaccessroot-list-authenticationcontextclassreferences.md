---
title: 列出 authenticationContextClassReferences
description: 检索 authenticationContextClassReference 对象的列表。
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c5ad949518d8371e18fc1ef10e680f618056b7f5
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547338"
---
# <a name="list-authenticationcontextclassreferences"></a><span data-ttu-id="b9959-103">列出 authenticationContextClassReferences</span><span class="sxs-lookup"><span data-stu-id="b9959-103">List authenticationContextClassReferences</span></span>

<span data-ttu-id="b9959-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9959-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9959-105">检索 [authenticationContextClassReference 对象](../resources/authenticationcontextclassreference.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="b9959-105">Retrieve a list of [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9959-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b9959-106">Permissions</span></span>

<span data-ttu-id="b9959-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9959-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9959-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9959-109">Permission type</span></span>                        | <span data-ttu-id="b9959-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b9959-110">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="b9959-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9959-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9959-112">Policy.Read.ConditionalAccess、Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="b9959-112">Policy.Read.ConditionalAccess, Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="b9959-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9959-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9959-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9959-114">Not supported.</span></span> |
|<span data-ttu-id="b9959-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9959-115">Application</span></span>                            | <span data-ttu-id="b9959-116">Policy.Read.ConditionalAccess、Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="b9959-116">Policy.Read.ConditionalAccess, Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9959-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9959-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/authenticationContextClassReferences
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b9959-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b9959-118">Optional query parameters</span></span>

<span data-ttu-id="b9959-119">此方法支持 `$filter` 和 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b9959-119">This method supports the `$filter` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="b9959-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b9959-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9959-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9959-121">Request headers</span></span>

| <span data-ttu-id="b9959-122">名称</span><span class="sxs-lookup"><span data-stu-id="b9959-122">Name</span></span>      |<span data-ttu-id="b9959-123">说明</span><span class="sxs-lookup"><span data-stu-id="b9959-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b9959-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9959-124">Authorization</span></span> | <span data-ttu-id="b9959-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="b9959-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9959-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9959-126">Request body</span></span>

<span data-ttu-id="b9959-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b9959-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9959-128">响应</span><span class="sxs-lookup"><span data-stu-id="b9959-128">Response</span></span>

<span data-ttu-id="b9959-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [authenticationContextClassReference](..\resources\authenticationcontextclassreference.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b9959-129">If successful, this method returns a `200 OK` response code and a collection of [authenticationContextClassReference](..\resources\authenticationcontextclassreference.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9959-130">示例</span><span class="sxs-lookup"><span data-stu-id="b9959-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b9959-131">请求</span><span class="sxs-lookup"><span data-stu-id="b9959-131">Request</span></span>

<span data-ttu-id="b9959-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b9959-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b9959-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9959-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationcontextclassreference"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences
```



### <a name="response"></a><span data-ttu-id="b9959-134">响应</span><span class="sxs-lookup"><span data-stu-id="b9959-134">Response</span></span>

<span data-ttu-id="b9959-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b9959-135">The following is an example of the response.</span></span>

> <span data-ttu-id="b9959-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b9959-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.authenticationContextClassReference",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#/conditionalAccess/authenticationContextClassReferences",
  "value": [
    {
      "id": "c1",
      "displayName": "Contoso trusted locations",
      "description": "Access is only allowed from trusted locations",
      "isAvailable": true
    }
  ]
}


```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List authenticationContextClassReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
