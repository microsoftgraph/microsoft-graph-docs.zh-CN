---
title: List appliesTo
description: 获取 homeRealmDiscoveryPolicy 对象已应用到的 directoryObject 对象的列表。
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a43f1efba63ddd0121bed16c5110b9f5b06e740f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773618"
---
# <a name="list-appliesto"></a><span data-ttu-id="9dd6a-103">List appliesTo</span><span class="sxs-lookup"><span data-stu-id="9dd6a-103">List appliesTo</span></span>

<span data-ttu-id="9dd6a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9dd6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dd6a-105">获取[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)对象已应用到的[directoryObject](../resources/directoryObject.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="9dd6a-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object has been applied to.</span></span> <span data-ttu-id="9dd6a-106">homeRealmDiscoveryPolicy 只能应用于 [servicePrincipal](../resources/serviceprincipal.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="9dd6a-106">The homeRealmDiscoveryPolicy can only be applied to [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="9dd6a-107">权限</span><span class="sxs-lookup"><span data-stu-id="9dd6a-107">Permissions</span></span>

<span data-ttu-id="9dd6a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9dd6a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9dd6a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9dd6a-110">Permission type</span></span>                        | <span data-ttu-id="9dd6a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9dd6a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9dd6a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9dd6a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="9dd6a-113">Policy.Read.All 和 Application.Read.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9dd6a-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="9dd6a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9dd6a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9dd6a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9dd6a-115">Not supported.</span></span> |
| <span data-ttu-id="9dd6a-116">Application</span><span class="sxs-lookup"><span data-stu-id="9dd6a-116">Application</span></span>                            | <span data-ttu-id="9dd6a-117">Policy.Read.All 和 Application.Read.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9dd6a-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9dd6a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9dd6a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9dd6a-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9dd6a-119">Optional query parameters</span></span>

<span data-ttu-id="9dd6a-120">此方法支持 `$select` 和 `$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9dd6a-120">This method supports the `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="9dd6a-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9dd6a-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9dd6a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="9dd6a-122">Request headers</span></span>

| <span data-ttu-id="9dd6a-123">名称</span><span class="sxs-lookup"><span data-stu-id="9dd6a-123">Name</span></span>      |<span data-ttu-id="9dd6a-124">说明</span><span class="sxs-lookup"><span data-stu-id="9dd6a-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9dd6a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9dd6a-125">Authorization</span></span> | <span data-ttu-id="9dd6a-126">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="9dd6a-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9dd6a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9dd6a-127">Request body</span></span>

<span data-ttu-id="9dd6a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9dd6a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9dd6a-129">响应</span><span class="sxs-lookup"><span data-stu-id="9dd6a-129">Response</span></span>

<span data-ttu-id="9dd6a-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9dd6a-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9dd6a-131">示例</span><span class="sxs-lookup"><span data-stu-id="9dd6a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9dd6a-132">请求</span><span class="sxs-lookup"><span data-stu-id="9dd6a-132">Request</span></span>

<span data-ttu-id="9dd6a-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9dd6a-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9dd6a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9dd6a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```
# <a name="c"></a>[<span data-ttu-id="9dd6a-135">C#</span><span class="sxs-lookup"><span data-stu-id="9dd6a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appliesto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9dd6a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9dd6a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appliesto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9dd6a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9dd6a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appliesto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9dd6a-138">Java</span><span class="sxs-lookup"><span data-stu-id="9dd6a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-appliesto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9dd6a-139">响应</span><span class="sxs-lookup"><span data-stu-id="9dd6a-139">Response</span></span>

<span data-ttu-id="9dd6a-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9dd6a-140">The following is an example of the response.</span></span>

> <span data-ttu-id="9dd6a-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9dd6a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "deletedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

