---
title: 创建 claimsMappingPolicy
description: 创建新的 claimsMappingPolicy。
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1a1570e237c57f565c66afd0c921c31b6b8765f1
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863230"
---
# <a name="create-claimsmappingpolicy"></a><span data-ttu-id="f19cd-103">创建 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="f19cd-103">Create claimsMappingPolicy</span></span>

<span data-ttu-id="f19cd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f19cd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f19cd-105">创建新的[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f19cd-105">Create a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f19cd-106">权限</span><span class="sxs-lookup"><span data-stu-id="f19cd-106">Permissions</span></span>

<span data-ttu-id="f19cd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f19cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f19cd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f19cd-109">Permission type</span></span>                        | <span data-ttu-id="f19cd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f19cd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f19cd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f19cd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f19cd-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f19cd-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="f19cd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f19cd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f19cd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f19cd-114">Not supported.</span></span> |
| <span data-ttu-id="f19cd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f19cd-115">Application</span></span>                            | <span data-ttu-id="f19cd-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f19cd-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="f19cd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f19cd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="f19cd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f19cd-118">Request headers</span></span>

| <span data-ttu-id="f19cd-119">名称</span><span class="sxs-lookup"><span data-stu-id="f19cd-119">Name</span></span>          | <span data-ttu-id="f19cd-120">说明</span><span class="sxs-lookup"><span data-stu-id="f19cd-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f19cd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f19cd-121">Authorization</span></span> | <span data-ttu-id="f19cd-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="f19cd-122">Bearer {token}</span></span> |
| <span data-ttu-id="f19cd-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="f19cd-123">Content-type</span></span> | <span data-ttu-id="f19cd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f19cd-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f19cd-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f19cd-125">Request body</span></span>

<span data-ttu-id="f19cd-126">在请求正文中，提供[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f19cd-126">In the request body, supply a JSON representation of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f19cd-127">响应</span><span class="sxs-lookup"><span data-stu-id="f19cd-127">Response</span></span>

<span data-ttu-id="f19cd-128">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f19cd-128">If successful, this method returns a `201 Created` response code and a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f19cd-129">示例</span><span class="sxs-lookup"><span data-stu-id="f19cd-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f19cd-130">请求</span><span class="sxs-lookup"><span data-stu-id="f19cd-130">Request</span></span>

<span data-ttu-id="f19cd-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f19cd-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f19cd-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f19cd-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f19cd-133">C#</span><span class="sxs-lookup"><span data-stu-id="f19cd-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-claimsmappingpolicy-from-claimsmappingpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f19cd-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f19cd-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-claimsmappingpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f19cd-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f19cd-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-claimsmappingpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f19cd-136">Java</span><span class="sxs-lookup"><span data-stu-id="f19cd-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-claimsmappingpolicy-from-claimsmappingpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f19cd-137">响应</span><span class="sxs-lookup"><span data-stu-id="f19cd-137">Response</span></span>

<span data-ttu-id="f19cd-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f19cd-138">The following is an example of the response.</span></span>

> <span data-ttu-id="f19cd-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f19cd-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
