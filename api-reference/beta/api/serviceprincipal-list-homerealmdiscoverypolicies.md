---
title: 列出分配的 homeRealmDiscoveryPolicies
description: 列出分配给 servicePrincipal 的 homeRealmDiscoveryPolicies。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 5cebe83b8104ad2e00b2af30ec8124d14d24b7f4
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134328"
---
# <a name="list-assigned-homerealmdiscoverypolicy"></a><span data-ttu-id="1e6e7-103">列出分配的 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="1e6e7-103">List assigned homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="1e6e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e6e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e6e7-105">列出分配给[servicePrincipal](../resources/servicePrincipal.md)的[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1e6e7-105">List the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects that are assigned to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1e6e7-106">权限</span><span class="sxs-lookup"><span data-stu-id="1e6e7-106">Permissions</span></span>

<span data-ttu-id="1e6e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e6e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1e6e7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e6e7-109">Permission type</span></span>                        | <span data-ttu-id="1e6e7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e6e7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1e6e7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e6e7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1e6e7-112">Policy.Read.All 和 Application.ReadWrite.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e6e7-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="1e6e7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e6e7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e6e7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e6e7-114">Not supported.</span></span> |
| <span data-ttu-id="1e6e7-115">Application</span><span class="sxs-lookup"><span data-stu-id="1e6e7-115">Application</span></span>                            | <span data-ttu-id="1e6e7-116">Policy.Read.All 和 Application.ReadWrite.OwnedBy、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.OwnedBy、Policy.Read.All 和 Application.ReadWrite.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e6e7-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e6e7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e6e7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="1e6e7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e6e7-118">Request headers</span></span>

| <span data-ttu-id="1e6e7-119">名称</span><span class="sxs-lookup"><span data-stu-id="1e6e7-119">Name</span></span>          | <span data-ttu-id="1e6e7-120">说明</span><span class="sxs-lookup"><span data-stu-id="1e6e7-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1e6e7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e6e7-121">Authorization</span></span> | <span data-ttu-id="1e6e7-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="1e6e7-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e6e7-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e6e7-123">Request body</span></span>

<span data-ttu-id="1e6e7-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1e6e7-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e6e7-125">响应</span><span class="sxs-lookup"><span data-stu-id="1e6e7-125">Response</span></span>

<span data-ttu-id="1e6e7-126">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [homeRealmDiscoveryPolicy](../resources/homeRealmDiscoveryPolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1e6e7-126">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homeRealmDiscoveryPolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e6e7-127">示例</span><span class="sxs-lookup"><span data-stu-id="1e6e7-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e6e7-128">请求</span><span class="sxs-lookup"><span data-stu-id="1e6e7-128">Request</span></span>

<span data-ttu-id="1e6e7-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1e6e7-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1e6e7-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e6e7-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_homerealmdiscoverypolicies_on_serviceprincipal"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/homeRealmDiscoveryPolicies
```
# <a name="c"></a>[<span data-ttu-id="1e6e7-131">C#</span><span class="sxs-lookup"><span data-stu-id="1e6e7-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-homerealmdiscoverypolicies-on-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1e6e7-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e6e7-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-homerealmdiscoverypolicies-on-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1e6e7-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1e6e7-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-homerealmdiscoverypolicies-on-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1e6e7-134">Java</span><span class="sxs-lookup"><span data-stu-id="1e6e7-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-homerealmdiscoverypolicies-on-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1e6e7-135">响应</span><span class="sxs-lookup"><span data-stu-id="1e6e7-135">Response</span></span>

<span data-ttu-id="1e6e7-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1e6e7-136">The following is an example of the response.</span></span>

> <span data-ttu-id="1e6e7-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1e6e7-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
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
  "description": "List assigned homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



