---
title: 创建 claimsMappingPolicy
description: 创建新的 claimsMappingPolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: badb0bc304d4fa41a4826e7b166308dd80e148c3
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476336"
---
# <a name="create-claimsmappingpolicy"></a><span data-ttu-id="cdb66-103">创建 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="cdb66-103">Create claimsMappingPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdb66-104">创建新的[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cdb66-104">Create a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdb66-105">权限</span><span class="sxs-lookup"><span data-stu-id="cdb66-105">Permissions</span></span>

<span data-ttu-id="cdb66-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cdb66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cdb66-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cdb66-108">Permission type</span></span>                        | <span data-ttu-id="cdb66-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cdb66-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cdb66-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cdb66-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cdb66-111">ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="cdb66-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="cdb66-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cdb66-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdb66-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdb66-113">Not supported.</span></span> |
| <span data-ttu-id="cdb66-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cdb66-114">Application</span></span>                            | <span data-ttu-id="cdb66-115">ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="cdb66-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdb66-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdb66-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="cdb66-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="cdb66-117">Request headers</span></span>

| <span data-ttu-id="cdb66-118">名称</span><span class="sxs-lookup"><span data-stu-id="cdb66-118">Name</span></span>          | <span data-ttu-id="cdb66-119">说明</span><span class="sxs-lookup"><span data-stu-id="cdb66-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cdb66-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdb66-120">Authorization</span></span> | <span data-ttu-id="cdb66-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="cdb66-121">Bearer {token}</span></span> |
| <span data-ttu-id="cdb66-122">Content-type</span><span class="sxs-lookup"><span data-stu-id="cdb66-122">Content-type</span></span> | <span data-ttu-id="cdb66-123">application/json</span><span class="sxs-lookup"><span data-stu-id="cdb66-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cdb66-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="cdb66-124">Request body</span></span>

<span data-ttu-id="cdb66-125">在请求正文中，提供[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cdb66-125">In the request body, supply a JSON representation of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cdb66-126">响应</span><span class="sxs-lookup"><span data-stu-id="cdb66-126">Response</span></span>

<span data-ttu-id="cdb66-127">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cdb66-127">If successful, this method returns a `201 Created` response code and a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cdb66-128">示例</span><span class="sxs-lookup"><span data-stu-id="cdb66-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cdb66-129">请求</span><span class="sxs-lookup"><span data-stu-id="cdb66-129">Request</span></span>

<span data-ttu-id="cdb66-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cdb66-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cdb66-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdb66-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_claimsmappingpolicy_from_claimsmappingpolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/claimsMappingPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cdb66-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdb66-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-claimsmappingpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cdb66-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdb66-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-claimsmappingpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cdb66-134">响应</span><span class="sxs-lookup"><span data-stu-id="cdb66-134">Response</span></span>

<span data-ttu-id="cdb66-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cdb66-135">The following is an example of the response.</span></span>

> <span data-ttu-id="cdb66-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cdb66-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
