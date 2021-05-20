---
title: 获取 authenticationContextClassReference
description: 检索 authenticationContextClassReference 对象的属性和关系。
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3ca46a2dfff70ed32bc2e960b4f16cdca9ab7da8
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547324"
---
# <a name="get-authenticationcontextclassreference"></a><span data-ttu-id="d9ddf-103">获取 authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="d9ddf-103">Get authenticationContextClassReference</span></span>

<span data-ttu-id="d9ddf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9ddf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9ddf-105">检索 [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d9ddf-105">Retrieve the properties and relationships of a [authenticationContextClassReference](../resources/authenticationcontextclassreference.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9ddf-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d9ddf-106">Permissions</span></span>

<span data-ttu-id="d9ddf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d9ddf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9ddf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9ddf-109">Permission type</span></span>                        | <span data-ttu-id="d9ddf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d9ddf-110">Permissions (from least to most privileged)</span></span>                                       |
|:--------------------------------------|:----------------------------------------------------------------------------------|
|<span data-ttu-id="d9ddf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9ddf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9ddf-112">Policy.Read.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="d9ddf-112">Policy.Read.ConditionalAccess</span></span> |
|<span data-ttu-id="d9ddf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9ddf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9ddf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9ddf-114">Not supported.</span></span> |
|<span data-ttu-id="d9ddf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9ddf-115">Application</span></span>                            | <span data-ttu-id="d9ddf-116">Policy.Read.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="d9ddf-116">Policy.Read.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9ddf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9ddf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/authenticationContextClassReferences/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d9ddf-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d9ddf-118">Optional query parameters</span></span>

<span data-ttu-id="d9ddf-119">此方法不支持自定义响应的可选查询参数。</span><span class="sxs-lookup"><span data-stu-id="d9ddf-119">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9ddf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9ddf-120">Request headers</span></span>

| <span data-ttu-id="d9ddf-121">名称</span><span class="sxs-lookup"><span data-stu-id="d9ddf-121">Name</span></span>      |<span data-ttu-id="d9ddf-122">说明</span><span class="sxs-lookup"><span data-stu-id="d9ddf-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d9ddf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9ddf-123">Authorization</span></span> | <span data-ttu-id="d9ddf-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="d9ddf-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9ddf-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9ddf-125">Request body</span></span>

<span data-ttu-id="d9ddf-126">此方法支持 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d9ddf-126">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="d9ddf-127">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d9ddf-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="response"></a><span data-ttu-id="d9ddf-128">响应</span><span class="sxs-lookup"><span data-stu-id="d9ddf-128">Response</span></span>

<span data-ttu-id="d9ddf-129">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [authenticationContextClassReferences](../resources/\authenticationcontextclassreference.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9ddf-129">If successful, this method returns a `200 OK` response code and the requested [authenticationContextClassReferences](../resources/\authenticationcontextclassreference.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9ddf-130">示例</span><span class="sxs-lookup"><span data-stu-id="d9ddf-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9ddf-131">请求</span><span class="sxs-lookup"><span data-stu-id="d9ddf-131">Request</span></span>

<span data-ttu-id="d9ddf-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d9ddf-132">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_authenticationcontextclassreference"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences/c1
```



### <a name="response"></a><span data-ttu-id="d9ddf-133">响应</span><span class="sxs-lookup"><span data-stu-id="d9ddf-133">Response</span></span>

<span data-ttu-id="d9ddf-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d9ddf-134">The following is an example of the response.</span></span>

> <span data-ttu-id="d9ddf-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d9ddf-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
