---
title: 删除 conditionalAccessPolicy
description: 删除 conditionalAccessPolicy。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 29e8bc18b4608f08a8285c6b575e2ce96c204fc4
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916508"
---
# <a name="delete-conditionalaccesspolicy"></a><span data-ttu-id="f97b4-103">删除 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="f97b4-103">Delete conditionalAccessPolicy</span></span>

<span data-ttu-id="f97b4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f97b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f97b4-105">删除[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f97b4-105">Delete a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f97b4-106">权限</span><span class="sxs-lookup"><span data-stu-id="f97b4-106">Permissions</span></span>

<span data-ttu-id="f97b4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f97b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f97b4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f97b4-109">Permission type</span></span>                        | <span data-ttu-id="f97b4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f97b4-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="f97b4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f97b4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f97b4-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="f97b4-112">Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="f97b4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f97b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f97b4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f97b4-114">Not supported.</span></span> |
|<span data-ttu-id="f97b4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f97b4-115">Application</span></span>                            | <span data-ttu-id="f97b4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f97b4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f97b4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f97b4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f97b4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f97b4-118">Request headers</span></span>

| <span data-ttu-id="f97b4-119">名称</span><span class="sxs-lookup"><span data-stu-id="f97b4-119">Name</span></span>          | <span data-ttu-id="f97b4-120">说明</span><span class="sxs-lookup"><span data-stu-id="f97b4-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f97b4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f97b4-121">Authorization</span></span> | <span data-ttu-id="f97b4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f97b4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f97b4-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f97b4-124">Request body</span></span>

<span data-ttu-id="f97b4-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f97b4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f97b4-126">响应</span><span class="sxs-lookup"><span data-stu-id="f97b4-126">Response</span></span>

<span data-ttu-id="f97b4-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f97b4-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f97b4-129">示例</span><span class="sxs-lookup"><span data-stu-id="f97b4-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f97b4-130">请求</span><span class="sxs-lookup"><span data-stu-id="f97b4-130">Request</span></span>

<span data-ttu-id="f97b4-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f97b4-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f97b4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f97b4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conditionalaccesspolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}
```
# <a name="c"></a>[<span data-ttu-id="f97b4-133">C#</span><span class="sxs-lookup"><span data-stu-id="f97b4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f97b4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f97b4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f97b4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f97b4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f97b4-136">响应</span><span class="sxs-lookup"><span data-stu-id="f97b4-136">Response</span></span>

<span data-ttu-id="f97b4-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f97b4-137">The following is an example of the response.</span></span>

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
