---
title: 列表已分配 homeRealmDiscoveryPolicies
description: 列出分配给服务主体的 homeRealmDiscoveryPolicies。
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c4e200e01ff36db17bbeb51c5d42da95c32f414c
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846244"
---
# <a name="list-assigned-homerealmdiscoverypolicy"></a><span data-ttu-id="62248-103">列表已分配 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="62248-103">List assigned homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="62248-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62248-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="62248-105">列出分配给[servicePrincipal](../resources/serviceprincipal.md)的[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="62248-105">List the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects that are assigned to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="62248-106">权限</span><span class="sxs-lookup"><span data-stu-id="62248-106">Permissions</span></span>

<span data-ttu-id="62248-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="62248-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="62248-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62248-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62248-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="62248-109">Permission type</span></span>                        | <span data-ttu-id="62248-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62248-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="62248-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62248-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="62248-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="62248-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="62248-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62248-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62248-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="62248-114">Not supported.</span></span> |
| <span data-ttu-id="62248-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="62248-115">Application</span></span>                            | <span data-ttu-id="62248-116">Policy. All 和 Application.readwrite.ownedby、Application.readwrite.ownedby、ApplicationConfiguration 和、、ApplicationConfiguration 和应用程序的、、和和的所有应用程序中的</span><span class="sxs-lookup"><span data-stu-id="62248-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="62248-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62248-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /servicePrincipals/{id}/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="62248-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="62248-118">Request headers</span></span>

| <span data-ttu-id="62248-119">名称</span><span class="sxs-lookup"><span data-stu-id="62248-119">Name</span></span>          | <span data-ttu-id="62248-120">说明</span><span class="sxs-lookup"><span data-stu-id="62248-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="62248-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="62248-121">Authorization</span></span> | <span data-ttu-id="62248-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="62248-122">Bearer {token}.</span></span> <span data-ttu-id="62248-123">Required.</span><span class="sxs-lookup"><span data-stu-id="62248-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="62248-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="62248-124">Request body</span></span>

<span data-ttu-id="62248-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="62248-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62248-126">响应</span><span class="sxs-lookup"><span data-stu-id="62248-126">Response</span></span>

<span data-ttu-id="62248-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="62248-127">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="62248-128">示例</span><span class="sxs-lookup"><span data-stu-id="62248-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="62248-129">请求</span><span class="sxs-lookup"><span data-stu-id="62248-129">Request</span></span>

<span data-ttu-id="62248-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="62248-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="62248-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="62248-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_homerealmdiscoverypolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/homeRealmDiscoveryPolicies
```

### <a name="response"></a><span data-ttu-id="62248-132">响应</span><span class="sxs-lookup"><span data-stu-id="62248-132">Response</span></span>

<span data-ttu-id="62248-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="62248-133">The following is an example of the response.</span></span>

> <span data-ttu-id="62248-134">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="62248-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="62248-135">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="62248-135">All the properties will be returned from an actual call.</span></span>

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
