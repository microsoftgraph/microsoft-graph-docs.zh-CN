---
title: 创建 homeRealmDiscoveryPolicy
description: 创建新的 homeRealmDiscoveryPolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac52450c558b709c74d024d30c843679eda239ea
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475768"
---
# <a name="create-homerealmdiscoverypolicy"></a><span data-ttu-id="61777-103">创建 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="61777-103">Create homeRealmDiscoveryPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61777-104">创建新的[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="61777-104">Create a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="61777-105">权限</span><span class="sxs-lookup"><span data-stu-id="61777-105">Permissions</span></span>

<span data-ttu-id="61777-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="61777-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="61777-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="61777-108">Permission type</span></span>                        | <span data-ttu-id="61777-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="61777-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="61777-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61777-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="61777-111">ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="61777-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="61777-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61777-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61777-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="61777-113">Not supported.</span></span> |
| <span data-ttu-id="61777-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="61777-114">Application</span></span>                            | <span data-ttu-id="61777-115">ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="61777-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="61777-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61777-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="61777-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="61777-117">Request headers</span></span>

| <span data-ttu-id="61777-118">名称</span><span class="sxs-lookup"><span data-stu-id="61777-118">Name</span></span>          | <span data-ttu-id="61777-119">说明</span><span class="sxs-lookup"><span data-stu-id="61777-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="61777-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="61777-120">Authorization</span></span> | <span data-ttu-id="61777-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="61777-121">Bearer {token}</span></span> |
| <span data-ttu-id="61777-122">Content-type</span><span class="sxs-lookup"><span data-stu-id="61777-122">Content-type</span></span> | <span data-ttu-id="61777-123">application/json</span><span class="sxs-lookup"><span data-stu-id="61777-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="61777-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="61777-124">Request body</span></span>

<span data-ttu-id="61777-125">在请求正文中，提供[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61777-125">In the request body, supply a JSON representation of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="61777-126">响应</span><span class="sxs-lookup"><span data-stu-id="61777-126">Response</span></span>

<span data-ttu-id="61777-127">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="61777-127">If successful, this method returns a `201 Created` response code and a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="61777-128">示例</span><span class="sxs-lookup"><span data-stu-id="61777-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="61777-129">请求</span><span class="sxs-lookup"><span data-stu-id="61777-129">Request</span></span>

<span data-ttu-id="61777-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="61777-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="61777-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="61777-131">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="61777-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61777-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="61777-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61777-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="61777-134">响应</span><span class="sxs-lookup"><span data-stu-id="61777-134">Response</span></span>

<span data-ttu-id="61777-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="61777-135">The following is an example of the response.</span></span>

> <span data-ttu-id="61777-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="61777-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
