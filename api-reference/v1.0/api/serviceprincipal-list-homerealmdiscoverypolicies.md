---
title: 列出分配的 homeRealmDiscoveryPolicies
description: 列出分配给服务主体的 homeRealmDiscoveryPolicies。
localization_priority: Normal
author: hpsin
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: ff1e9f71145de9dde6ec0c1bccf916e9ae142a70
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134559"
---
# <a name="list-assigned-homerealmdiscoverypolicy"></a><span data-ttu-id="c8cfb-103">列出分配的 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="c8cfb-103">List assigned homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="c8cfb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8cfb-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="c8cfb-105">列出分配给[servicePrincipal](../resources/serviceprincipal.md)的[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c8cfb-105">List the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects that are assigned to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c8cfb-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c8cfb-106">Permissions</span></span>

<span data-ttu-id="c8cfb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8cfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c8cfb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8cfb-109">Permission type</span></span>                        | <span data-ttu-id="c8cfb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c8cfb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c8cfb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8cfb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c8cfb-112">Policy.Read.All 和 Application.ReadWrite.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8cfb-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="c8cfb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8cfb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8cfb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8cfb-114">Not supported.</span></span> |
| <span data-ttu-id="c8cfb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8cfb-115">Application</span></span>                            | <span data-ttu-id="c8cfb-116">Policy.Read.All 和 Application.ReadWrite.OwnedBy、Policy.Read.All 和 Application.ReadWrite.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.OwnedBy、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8cfb-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8cfb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8cfb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="c8cfb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8cfb-118">Request headers</span></span>

| <span data-ttu-id="c8cfb-119">名称</span><span class="sxs-lookup"><span data-stu-id="c8cfb-119">Name</span></span>          | <span data-ttu-id="c8cfb-120">说明</span><span class="sxs-lookup"><span data-stu-id="c8cfb-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c8cfb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8cfb-121">Authorization</span></span> | <span data-ttu-id="c8cfb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c8cfb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c8cfb-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8cfb-124">Request body</span></span>

<span data-ttu-id="c8cfb-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c8cfb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8cfb-126">响应</span><span class="sxs-lookup"><span data-stu-id="c8cfb-126">Response</span></span>

<span data-ttu-id="c8cfb-127">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c8cfb-127">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c8cfb-128">示例</span><span class="sxs-lookup"><span data-stu-id="c8cfb-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c8cfb-129">请求</span><span class="sxs-lookup"><span data-stu-id="c8cfb-129">Request</span></span>

<span data-ttu-id="c8cfb-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c8cfb-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c8cfb-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c8cfb-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_homerealmdiscoverypolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/homeRealmDiscoveryPolicies
```
# <a name="c"></a>[<span data-ttu-id="c8cfb-132">C#</span><span class="sxs-lookup"><span data-stu-id="c8cfb-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-homerealmdiscoverypolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c8cfb-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c8cfb-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-homerealmdiscoverypolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c8cfb-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c8cfb-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-homerealmdiscoverypolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c8cfb-135">Java</span><span class="sxs-lookup"><span data-stu-id="c8cfb-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-homerealmdiscoverypolicies-on-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c8cfb-136">响应</span><span class="sxs-lookup"><span data-stu-id="c8cfb-136">Response</span></span>

<span data-ttu-id="c8cfb-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c8cfb-137">The following is an example of the response.</span></span>

> <span data-ttu-id="c8cfb-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c8cfb-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

