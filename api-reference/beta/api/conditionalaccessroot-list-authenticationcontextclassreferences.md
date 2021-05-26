---
title: 列出 authenticationContextClassReferences
description: 检索 authenticationContextClassReference 对象的列表。
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e744c182c99d91f668605090f52f0f346cc7c9f4
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52663977"
---
# <a name="list-authenticationcontextclassreferences"></a><span data-ttu-id="b0c87-103">列出 authenticationContextClassReferences</span><span class="sxs-lookup"><span data-stu-id="b0c87-103">List authenticationContextClassReferences</span></span>

<span data-ttu-id="b0c87-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0c87-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0c87-105">检索 [authenticationContextClassReference 对象](../resources/authenticationcontextclassreference.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="b0c87-105">Retrieve a list of [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0c87-106">权限</span><span class="sxs-lookup"><span data-stu-id="b0c87-106">Permissions</span></span>

<span data-ttu-id="b0c87-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0c87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0c87-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0c87-109">Permission type</span></span>                        | <span data-ttu-id="b0c87-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b0c87-110">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="b0c87-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0c87-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b0c87-112">Policy.Read.ConditionalAccess、Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="b0c87-112">Policy.Read.ConditionalAccess, Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="b0c87-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0c87-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0c87-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0c87-114">Not supported.</span></span> |
|<span data-ttu-id="b0c87-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0c87-115">Application</span></span>                            | <span data-ttu-id="b0c87-116">Policy.Read.ConditionalAccess、Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="b0c87-116">Policy.Read.ConditionalAccess, Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0c87-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0c87-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/authenticationContextClassReferences
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b0c87-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b0c87-118">Optional query parameters</span></span>

<span data-ttu-id="b0c87-119">此方法支持 `$filter` 和 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b0c87-119">This method supports the `$filter` and `$select` OData query parameters to help customize the response.</span></span> <span data-ttu-id="b0c87-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b0c87-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0c87-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0c87-121">Request headers</span></span>

| <span data-ttu-id="b0c87-122">名称</span><span class="sxs-lookup"><span data-stu-id="b0c87-122">Name</span></span>      |<span data-ttu-id="b0c87-123">说明</span><span class="sxs-lookup"><span data-stu-id="b0c87-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b0c87-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0c87-124">Authorization</span></span> | <span data-ttu-id="b0c87-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="b0c87-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0c87-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0c87-126">Request body</span></span>

<span data-ttu-id="b0c87-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b0c87-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0c87-128">响应</span><span class="sxs-lookup"><span data-stu-id="b0c87-128">Response</span></span>

<span data-ttu-id="b0c87-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [authenticationContextClassReference](..\resources\authenticationcontextclassreference.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b0c87-129">If successful, this method returns a `200 OK` response code and a collection of [authenticationContextClassReference](..\resources\authenticationcontextclassreference.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b0c87-130">示例</span><span class="sxs-lookup"><span data-stu-id="b0c87-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b0c87-131">请求</span><span class="sxs-lookup"><span data-stu-id="b0c87-131">Request</span></span>

<span data-ttu-id="b0c87-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b0c87-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b0c87-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0c87-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationcontextclassreference"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences
```
# <a name="c"></a>[<span data-ttu-id="b0c87-134">C#</span><span class="sxs-lookup"><span data-stu-id="b0c87-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationcontextclassreference-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0c87-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0c87-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationcontextclassreference-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0c87-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0c87-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationcontextclassreference-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b0c87-137">Java</span><span class="sxs-lookup"><span data-stu-id="b0c87-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-authenticationcontextclassreference-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a><span data-ttu-id="b0c87-138">响应</span><span class="sxs-lookup"><span data-stu-id="b0c87-138">Response</span></span>

<span data-ttu-id="b0c87-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b0c87-139">The following is an example of the response.</span></span>

> <span data-ttu-id="b0c87-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b0c87-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
