---
title: 删除 claimsMappingPolicy
description: 删除 claimsMappingPolicy。
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e4d9a94261d0c4a308eb03c532b954bf18150550
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846246"
---
# <a name="delete-claimsmappingpolicy"></a><span data-ttu-id="5ca94-103">删除 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="5ca94-103">Delete claimsMappingPolicy</span></span>

<span data-ttu-id="5ca94-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ca94-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ca94-105">删除[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5ca94-105">Delete a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ca94-106">权限</span><span class="sxs-lookup"><span data-stu-id="5ca94-106">Permissions</span></span>

<span data-ttu-id="5ca94-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5ca94-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5ca94-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ca94-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ca94-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ca94-109">Permission type</span></span>                        | <span data-ttu-id="5ca94-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5ca94-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5ca94-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ca94-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ca94-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="5ca94-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="5ca94-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ca94-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ca94-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ca94-114">Not supported.</span></span> |
| <span data-ttu-id="5ca94-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ca94-115">Application</span></span>                            | <span data-ttu-id="5ca94-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="5ca94-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ca94-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ca94-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5ca94-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ca94-118">Request headers</span></span>

| <span data-ttu-id="5ca94-119">名称</span><span class="sxs-lookup"><span data-stu-id="5ca94-119">Name</span></span>          | <span data-ttu-id="5ca94-120">说明</span><span class="sxs-lookup"><span data-stu-id="5ca94-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5ca94-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ca94-121">Authorization</span></span> | <span data-ttu-id="5ca94-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="5ca94-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ca94-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ca94-123">Request body</span></span>

<span data-ttu-id="5ca94-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5ca94-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ca94-125">响应</span><span class="sxs-lookup"><span data-stu-id="5ca94-125">Response</span></span>

<span data-ttu-id="5ca94-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5ca94-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5ca94-127">示例</span><span class="sxs-lookup"><span data-stu-id="5ca94-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5ca94-128">请求</span><span class="sxs-lookup"><span data-stu-id="5ca94-128">Request</span></span>

<span data-ttu-id="5ca94-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5ca94-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5ca94-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ca94-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="5ca94-131">响应</span><span class="sxs-lookup"><span data-stu-id="5ca94-131">Response</span></span>

<span data-ttu-id="5ca94-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5ca94-132">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
