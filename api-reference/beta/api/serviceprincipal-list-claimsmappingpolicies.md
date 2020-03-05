---
title: 列表已分配 claimsMappingPolicies
description: 列出分配给 servicePrincipal 的 claimsMappingPolicies。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 05fa25261dae265f76980ac38626c78a31b0423e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453434"
---
# <a name="list-assigned-claimsmappingpolicy"></a><span data-ttu-id="0e0ea-103">列表已分配 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="0e0ea-103">List assigned claimsMappingPolicy</span></span>

<span data-ttu-id="0e0ea-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0e0ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e0ea-105">列出分配给[servicePrincipal](../resources/servicePrincipal.md)的[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0e0ea-105">List the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects that are assigned to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0e0ea-106">权限</span><span class="sxs-lookup"><span data-stu-id="0e0ea-106">Permissions</span></span>

<span data-ttu-id="0e0ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e0ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0e0ea-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e0ea-109">Permission type</span></span>                        | <span data-ttu-id="0e0ea-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e0ea-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0e0ea-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e0ea-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e0ea-112">Policy. All 和 Application。所有读写。</span><span class="sxs-lookup"><span data-stu-id="0e0ea-112">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="0e0ea-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e0ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e0ea-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e0ea-114">Not supported.</span></span> |
| <span data-ttu-id="0e0ea-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e0ea-115">Application</span></span>                            | <span data-ttu-id="0e0ea-116">Policy. All 和 Application.readwrite.ownedby，all 和应用程序的 Read. all</span><span class="sxs-lookup"><span data-stu-id="0e0ea-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e0ea-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e0ea-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="0e0ea-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e0ea-118">Request headers</span></span>

| <span data-ttu-id="0e0ea-119">名称</span><span class="sxs-lookup"><span data-stu-id="0e0ea-119">Name</span></span>          | <span data-ttu-id="0e0ea-120">说明</span><span class="sxs-lookup"><span data-stu-id="0e0ea-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0e0ea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e0ea-121">Authorization</span></span> | <span data-ttu-id="0e0ea-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="0e0ea-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e0ea-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e0ea-123">Request body</span></span>

<span data-ttu-id="0e0ea-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0e0ea-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e0ea-125">响应</span><span class="sxs-lookup"><span data-stu-id="0e0ea-125">Response</span></span>

<span data-ttu-id="0e0ea-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和[claimsMappingPolicy](../resources/claimsMappingPolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="0e0ea-126">If successful, this method returns a `200 OK` response code and a collection of [claimsMappingPolicy](../resources/claimsMappingPolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0e0ea-127">示例</span><span class="sxs-lookup"><span data-stu-id="0e0ea-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0e0ea-128">请求</span><span class="sxs-lookup"><span data-stu-id="0e0ea-128">Request</span></span>

<span data-ttu-id="0e0ea-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0e0ea-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0e0ea-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e0ea-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_claimsmappingpolicies_on_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies
```
# <a name="c"></a>[<span data-ttu-id="0e0ea-131">C#</span><span class="sxs-lookup"><span data-stu-id="0e0ea-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-claimsmappingpolicies-on-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e0ea-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e0ea-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-claimsmappingpolicies-on-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e0ea-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e0ea-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-claimsmappingpolicies-on-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0e0ea-134">响应</span><span class="sxs-lookup"><span data-stu-id="0e0ea-134">Response</span></span>

<span data-ttu-id="0e0ea-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0e0ea-135">The following is an example of the response.</span></span>

> <span data-ttu-id="0e0ea-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0e0ea-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assigned claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
