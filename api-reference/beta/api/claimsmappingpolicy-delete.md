---
title: 删除 claimsMappingPolicy
description: 删除 claimsMappingPolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b60c3cc3b49fb486c31d36030b6722347f90f75a
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234160"
---
# <a name="delete-claimsmappingpolicy"></a><span data-ttu-id="85213-103">删除 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="85213-103">Delete claimsMappingPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85213-104">删除[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="85213-104">Delete a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="85213-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="85213-105">Permissions</span></span>

<span data-ttu-id="85213-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85213-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85213-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="85213-108">Permission type</span></span>                        | <span data-ttu-id="85213-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="85213-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="85213-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85213-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="85213-111">ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="85213-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="85213-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85213-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85213-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="85213-113">Not supported.</span></span> |
| <span data-ttu-id="85213-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="85213-114">Application</span></span>                            | <span data-ttu-id="85213-115">ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="85213-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="85213-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85213-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="85213-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="85213-117">Request headers</span></span>

| <span data-ttu-id="85213-118">名称</span><span class="sxs-lookup"><span data-stu-id="85213-118">Name</span></span>          | <span data-ttu-id="85213-119">说明</span><span class="sxs-lookup"><span data-stu-id="85213-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="85213-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="85213-120">Authorization</span></span> | <span data-ttu-id="85213-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="85213-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="85213-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="85213-122">Request body</span></span>

<span data-ttu-id="85213-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="85213-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85213-124">响应</span><span class="sxs-lookup"><span data-stu-id="85213-124">Response</span></span>

<span data-ttu-id="85213-125">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="85213-125">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="85213-126">示例</span><span class="sxs-lookup"><span data-stu-id="85213-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="85213-127">请求</span><span class="sxs-lookup"><span data-stu-id="85213-127">Request</span></span>

<span data-ttu-id="85213-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="85213-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/claimsMappingPolicies/{id}
```

### <a name="response"></a><span data-ttu-id="85213-129">响应</span><span class="sxs-lookup"><span data-stu-id="85213-129">Response</span></span>

<span data-ttu-id="85213-130">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="85213-130">The following is an example of the response.</span></span>

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