---
title: 获取 authenticationContextClassReference
description: 检索 authenticationContextClassReference 对象的属性和关系。
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 38d63cf4422332502d0595b3e00fed2f305c02c6
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664522"
---
# <a name="get-authenticationcontextclassreference"></a><span data-ttu-id="6906b-103">获取 authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="6906b-103">Get authenticationContextClassReference</span></span>

<span data-ttu-id="6906b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6906b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6906b-105">检索 [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6906b-105">Retrieve the properties and relationships of a [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6906b-106">权限</span><span class="sxs-lookup"><span data-stu-id="6906b-106">Permissions</span></span>

<span data-ttu-id="6906b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6906b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6906b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6906b-109">Permission type</span></span>                        | <span data-ttu-id="6906b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6906b-110">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="6906b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6906b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6906b-112">Policy.Read.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="6906b-112">Policy.Read.ConditionalAccess</span></span> |
|<span data-ttu-id="6906b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6906b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6906b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6906b-114">Not supported.</span></span> |
|<span data-ttu-id="6906b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6906b-115">Application</span></span>                            | <span data-ttu-id="6906b-116">Policy.Read.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="6906b-116">Policy.Read.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="6906b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6906b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/authenticationContextClassReferences/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6906b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6906b-118">Optional query parameters</span></span>

<span data-ttu-id="6906b-119">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="6906b-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6906b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6906b-120">Request headers</span></span>

| <span data-ttu-id="6906b-121">名称</span><span class="sxs-lookup"><span data-stu-id="6906b-121">Name</span></span>      |<span data-ttu-id="6906b-122">说明</span><span class="sxs-lookup"><span data-stu-id="6906b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6906b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6906b-123">Authorization</span></span> | <span data-ttu-id="6906b-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="6906b-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6906b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6906b-125">Request body</span></span>

<span data-ttu-id="6906b-126">此方法支持 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6906b-126">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="6906b-127">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6906b-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="response"></a><span data-ttu-id="6906b-128">响应</span><span class="sxs-lookup"><span data-stu-id="6906b-128">Response</span></span>

<span data-ttu-id="6906b-129">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [authenticationContextClassReferences](../resources/\authenticationcontextclassreference.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6906b-129">If successful, this method returns a `200 OK` response code and the requested [authenticationContextClassReferences](../resources/\authenticationcontextclassreference.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6906b-130">示例</span><span class="sxs-lookup"><span data-stu-id="6906b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6906b-131">请求</span><span class="sxs-lookup"><span data-stu-id="6906b-131">Request</span></span>

<span data-ttu-id="6906b-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6906b-132">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="6906b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6906b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationcontextclassreference"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences/c1
```
# <a name="c"></a>[<span data-ttu-id="6906b-134">C#</span><span class="sxs-lookup"><span data-stu-id="6906b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationcontextclassreference-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6906b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6906b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationcontextclassreference-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6906b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6906b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationcontextclassreference-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6906b-137">Java</span><span class="sxs-lookup"><span data-stu-id="6906b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-authenticationcontextclassreference-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a><span data-ttu-id="6906b-138">响应</span><span class="sxs-lookup"><span data-stu-id="6906b-138">Response</span></span>

<span data-ttu-id="6906b-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6906b-139">The following is an example of the response.</span></span>

> <span data-ttu-id="6906b-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6906b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationContextClassReference"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/authenticationContextClassReferences/$entity",
    "id": "c1",
    "displayName": "Contoso medium",
    "description": "Medium protection level defined for Contoso policy",
    "isAvailable": false
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get authenticationContextClassReference",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
