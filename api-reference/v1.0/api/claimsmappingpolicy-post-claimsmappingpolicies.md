---
title: 创建 claimsMappingPolicy
description: 创建新的 claimsMappingPolicy。
localization_priority: Normal
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f0f22d941c5d7f5ed1e3691e461d6cda25d5b31f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051548"
---
# <a name="create-claimsmappingpolicy"></a><span data-ttu-id="1b196-103">创建 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="1b196-103">Create claimsMappingPolicy</span></span>

<span data-ttu-id="1b196-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b196-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1b196-105">创建新的 [claimsMappingPolicy](../resources/claimsmappingpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1b196-105">Create a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b196-106">权限</span><span class="sxs-lookup"><span data-stu-id="1b196-106">Permissions</span></span>

<span data-ttu-id="1b196-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b196-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1b196-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b196-109">Permission type</span></span>                        | <span data-ttu-id="1b196-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b196-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1b196-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b196-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1b196-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="1b196-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="1b196-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b196-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b196-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b196-114">Not supported.</span></span> |
| <span data-ttu-id="1b196-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b196-115">Application</span></span>                            | <span data-ttu-id="1b196-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="1b196-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b196-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b196-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="1b196-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b196-118">Request headers</span></span>

| <span data-ttu-id="1b196-119">名称</span><span class="sxs-lookup"><span data-stu-id="1b196-119">Name</span></span>          | <span data-ttu-id="1b196-120">说明</span><span class="sxs-lookup"><span data-stu-id="1b196-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1b196-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b196-121">Authorization</span></span> | <span data-ttu-id="1b196-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="1b196-122">Bearer {token}</span></span> |
| <span data-ttu-id="1b196-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="1b196-123">Content-type</span></span> | <span data-ttu-id="1b196-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1b196-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b196-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b196-125">Request body</span></span>

<span data-ttu-id="1b196-126">在请求正文中，提供 [claimsMappingPolicy 对象的](../resources/claimsmappingpolicy.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b196-126">In the request body, supply a JSON representation of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1b196-127">响应</span><span class="sxs-lookup"><span data-stu-id="1b196-127">Response</span></span>

<span data-ttu-id="1b196-128">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [claimsMappingPolicy](../resources/claimsmappingpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1b196-128">If successful, this method returns a `201 Created` response code and a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b196-129">示例</span><span class="sxs-lookup"><span data-stu-id="1b196-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1b196-130">请求</span><span class="sxs-lookup"><span data-stu-id="1b196-130">Request</span></span>

<span data-ttu-id="1b196-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1b196-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b196-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b196-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_claimsmappingpolicy_from_claimsmappingpolicies"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="c"></a>[<span data-ttu-id="1b196-133">C#</span><span class="sxs-lookup"><span data-stu-id="1b196-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-claimsmappingpolicy-from-claimsmappingpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b196-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b196-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-claimsmappingpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b196-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b196-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-claimsmappingpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b196-136">Java</span><span class="sxs-lookup"><span data-stu-id="1b196-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-claimsmappingpolicy-from-claimsmappingpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1b196-137">响应</span><span class="sxs-lookup"><span data-stu-id="1b196-137">Response</span></span>

<span data-ttu-id="1b196-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1b196-138">The following is an example of the response.</span></span>

> <span data-ttu-id="1b196-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1b196-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy"
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
  "description": "Create claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

