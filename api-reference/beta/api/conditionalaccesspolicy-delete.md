---
title: 删除 conditionalAccessPolicy
description: 删除 conditionalAccessPolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bc4d00975fc92e9e561ebfaa1b403f351b0baf9d
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636769"
---
# <a name="delete-conditionalaccesspolicy"></a><span data-ttu-id="0b07a-103">删除 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="0b07a-103">Delete conditionalAccessPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b07a-104">删除[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b07a-104">Delete a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b07a-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="0b07a-105">Permissions</span></span>

<span data-ttu-id="0b07a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b07a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b07a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b07a-108">Permission type</span></span>                        | <span data-ttu-id="0b07a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b07a-109">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="0b07a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b07a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b07a-111">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="0b07a-111">Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="0b07a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b07a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b07a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b07a-113">Not supported.</span></span> |
|<span data-ttu-id="0b07a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b07a-114">Application</span></span>                            | <span data-ttu-id="0b07a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b07a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b07a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b07a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0b07a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b07a-117">Request headers</span></span>

| <span data-ttu-id="0b07a-118">名称</span><span class="sxs-lookup"><span data-stu-id="0b07a-118">Name</span></span>          | <span data-ttu-id="0b07a-119">说明</span><span class="sxs-lookup"><span data-stu-id="0b07a-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0b07a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b07a-120">Authorization</span></span> | <span data-ttu-id="0b07a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b07a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b07a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b07a-123">Request body</span></span>

<span data-ttu-id="0b07a-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0b07a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b07a-125">响应</span><span class="sxs-lookup"><span data-stu-id="0b07a-125">Response</span></span>

<span data-ttu-id="0b07a-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0b07a-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b07a-128">示例</span><span class="sxs-lookup"><span data-stu-id="0b07a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0b07a-129">请求</span><span class="sxs-lookup"><span data-stu-id="0b07a-129">Request</span></span>

<span data-ttu-id="0b07a-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b07a-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0b07a-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b07a-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conditionalaccesspolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/policies/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b07a-132">C#</span><span class="sxs-lookup"><span data-stu-id="0b07a-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b07a-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b07a-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b07a-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b07a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0b07a-135">响应</span><span class="sxs-lookup"><span data-stu-id="0b07a-135">Response</span></span>

<span data-ttu-id="0b07a-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b07a-136">The following is an example of the response.</span></span>

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
