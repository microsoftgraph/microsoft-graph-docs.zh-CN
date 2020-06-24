---
title: 创建 claimsMappingPolicy
description: 创建新的 claimsMappingPolicy。
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7d4e96ab4f746d24ad436f1c63568533e9c38790
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846228"
---
# <a name="create-claimsmappingpolicy"></a><span data-ttu-id="cb1bd-103">创建 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="cb1bd-103">Create claimsMappingPolicy</span></span>

<span data-ttu-id="cb1bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb1bd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb1bd-105">创建新的[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cb1bd-105">Create a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb1bd-106">权限</span><span class="sxs-lookup"><span data-stu-id="cb1bd-106">Permissions</span></span>

<span data-ttu-id="cb1bd-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="cb1bd-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="cb1bd-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb1bd-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb1bd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb1bd-109">Permission type</span></span>                        | <span data-ttu-id="cb1bd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cb1bd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cb1bd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb1bd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb1bd-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb1bd-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="cb1bd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb1bd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb1bd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb1bd-114">Not supported.</span></span> |
| <span data-ttu-id="cb1bd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb1bd-115">Application</span></span>                            | <span data-ttu-id="cb1bd-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb1bd-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb1bd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb1bd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="cb1bd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb1bd-118">Request headers</span></span>

| <span data-ttu-id="cb1bd-119">名称</span><span class="sxs-lookup"><span data-stu-id="cb1bd-119">Name</span></span>          | <span data-ttu-id="cb1bd-120">说明</span><span class="sxs-lookup"><span data-stu-id="cb1bd-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cb1bd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb1bd-121">Authorization</span></span> | <span data-ttu-id="cb1bd-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="cb1bd-122">Bearer {token}</span></span> |
| <span data-ttu-id="cb1bd-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="cb1bd-123">Content-type</span></span> | <span data-ttu-id="cb1bd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cb1bd-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb1bd-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb1bd-125">Request body</span></span>

<span data-ttu-id="cb1bd-126">在请求正文中，提供[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb1bd-126">In the request body, supply a JSON representation of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cb1bd-127">响应</span><span class="sxs-lookup"><span data-stu-id="cb1bd-127">Response</span></span>

<span data-ttu-id="cb1bd-128">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cb1bd-128">If successful, this method returns a `201 Created` response code and a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb1bd-129">示例</span><span class="sxs-lookup"><span data-stu-id="cb1bd-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb1bd-130">请求</span><span class="sxs-lookup"><span data-stu-id="cb1bd-130">Request</span></span>

<span data-ttu-id="cb1bd-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cb1bd-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cb1bd-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb1bd-132">HTTP</span></span>](#tab/http)
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

### <a name="response"></a><span data-ttu-id="cb1bd-133">响应</span><span class="sxs-lookup"><span data-stu-id="cb1bd-133">Response</span></span>

<span data-ttu-id="cb1bd-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cb1bd-134">The following is an example of the response.</span></span>

> <span data-ttu-id="cb1bd-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="cb1bd-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cb1bd-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="cb1bd-136">All the properties will be returned from an actual call.</span></span>

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
