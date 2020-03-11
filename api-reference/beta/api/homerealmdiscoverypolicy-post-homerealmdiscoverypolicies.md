---
title: 创建 homeRealmDiscoveryPolicy
description: 创建新的 homeRealmDiscoveryPolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 83fcc68695a55bbfb154386897a61189f7451733
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589948"
---
# <a name="create-homerealmdiscoverypolicy"></a><span data-ttu-id="53210-103">创建 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="53210-103">Create homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="53210-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53210-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53210-105">创建新的[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="53210-105">Create a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="53210-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="53210-106">Permissions</span></span>

<span data-ttu-id="53210-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53210-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53210-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="53210-109">Permission type</span></span>                        | <span data-ttu-id="53210-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53210-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="53210-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53210-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="53210-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="53210-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="53210-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53210-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53210-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="53210-114">Not supported.</span></span> |
| <span data-ttu-id="53210-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="53210-115">Application</span></span>                            | <span data-ttu-id="53210-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="53210-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="53210-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53210-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="53210-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="53210-118">Request headers</span></span>

| <span data-ttu-id="53210-119">名称</span><span class="sxs-lookup"><span data-stu-id="53210-119">Name</span></span>          | <span data-ttu-id="53210-120">说明</span><span class="sxs-lookup"><span data-stu-id="53210-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="53210-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="53210-121">Authorization</span></span> | <span data-ttu-id="53210-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="53210-122">Bearer {token}</span></span> |
| <span data-ttu-id="53210-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="53210-123">Content-type</span></span> | <span data-ttu-id="53210-124">application/json</span><span class="sxs-lookup"><span data-stu-id="53210-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="53210-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="53210-125">Request body</span></span>

<span data-ttu-id="53210-126">在请求正文中，提供[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53210-126">In the request body, supply a JSON representation of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="53210-127">响应</span><span class="sxs-lookup"><span data-stu-id="53210-127">Response</span></span>

<span data-ttu-id="53210-128">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="53210-128">If successful, this method returns a `201 Created` response code and a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53210-129">示例</span><span class="sxs-lookup"><span data-stu-id="53210-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="53210-130">请求</span><span class="sxs-lookup"><span data-stu-id="53210-130">Request</span></span>

<span data-ttu-id="53210-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="53210-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="53210-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="53210-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_homerealmdiscoverypolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="53210-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53210-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53210-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53210-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="53210-135">C#</span><span class="sxs-lookup"><span data-stu-id="53210-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="53210-136">响应</span><span class="sxs-lookup"><span data-stu-id="53210-136">Response</span></span>

<span data-ttu-id="53210-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="53210-137">The following is an example of the response.</span></span>

> <span data-ttu-id="53210-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="53210-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
