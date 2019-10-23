---
title: 删除 conditionalAccessPolicy
description: 删除 conditionalAccessPolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 97f9741040f2aa858b0c3d02116e780201830e3b
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638412"
---
# <a name="delete-conditionalaccesspolicy"></a><span data-ttu-id="44dc7-103">删除 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="44dc7-103">Delete conditionalAccessPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44dc7-104">删除[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="44dc7-104">Delete a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="44dc7-105">权限</span><span class="sxs-lookup"><span data-stu-id="44dc7-105">Permissions</span></span>

<span data-ttu-id="44dc7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44dc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44dc7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="44dc7-108">Permission type</span></span>                        | <span data-ttu-id="44dc7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44dc7-109">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="44dc7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44dc7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="44dc7-111">ConditionalAccess 和 Directory.accessasuser.all 的所有</span><span class="sxs-lookup"><span data-stu-id="44dc7-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="44dc7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44dc7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44dc7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="44dc7-113">Not supported.</span></span> |
|<span data-ttu-id="44dc7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="44dc7-114">Application</span></span>                            | <span data-ttu-id="44dc7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="44dc7-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="44dc7-116">此 API 需要多个权限。</span><span class="sxs-lookup"><span data-stu-id="44dc7-116">This API requires multiple permissions.</span></span> <span data-ttu-id="44dc7-117">有关详细信息，请参阅[已知问题](/graph/known-issues#conditional-access-policies-and-named-locations)。</span><span class="sxs-lookup"><span data-stu-id="44dc7-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="44dc7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44dc7-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="44dc7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="44dc7-119">Request headers</span></span>

| <span data-ttu-id="44dc7-120">名称</span><span class="sxs-lookup"><span data-stu-id="44dc7-120">Name</span></span>          | <span data-ttu-id="44dc7-121">说明</span><span class="sxs-lookup"><span data-stu-id="44dc7-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="44dc7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="44dc7-122">Authorization</span></span> | <span data-ttu-id="44dc7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="44dc7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44dc7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="44dc7-125">Request body</span></span>

<span data-ttu-id="44dc7-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="44dc7-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44dc7-127">响应</span><span class="sxs-lookup"><span data-stu-id="44dc7-127">Response</span></span>

<span data-ttu-id="44dc7-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="44dc7-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="44dc7-130">示例</span><span class="sxs-lookup"><span data-stu-id="44dc7-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="44dc7-131">请求</span><span class="sxs-lookup"><span data-stu-id="44dc7-131">Request</span></span>

<span data-ttu-id="44dc7-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="44dc7-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conditionalaccesspolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/policies/{id}
```

### <a name="response"></a><span data-ttu-id="44dc7-133">响应</span><span class="sxs-lookup"><span data-stu-id="44dc7-133">Response</span></span>

<span data-ttu-id="44dc7-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="44dc7-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conditionalAccessPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
