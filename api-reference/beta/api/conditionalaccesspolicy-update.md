---
title: 更新 conditionalAccessPolicy
description: 更新 conditionalAccessPolicy 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b55e492f7fae576c9026588205eae2bafa99c178
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636762"
---
# <a name="update-conditionalaccesspolicy"></a><span data-ttu-id="178b4-103">更新 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="178b4-103">Update conditionalAccessPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="178b4-104">更新[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="178b4-104">Update the properties of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="178b4-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="178b4-105">Permissions</span></span>

<span data-ttu-id="178b4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="178b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="178b4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="178b4-108">Permission type</span></span>                        | <span data-ttu-id="178b4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="178b4-109">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="178b4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="178b4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="178b4-111">ConditionalAccess 和应用程序的读取。 All</span><span class="sxs-lookup"><span data-stu-id="178b4-111">Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
|<span data-ttu-id="178b4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="178b4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="178b4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="178b4-113">Not supported.</span></span> |
|<span data-ttu-id="178b4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="178b4-114">Application</span></span>                            | <span data-ttu-id="178b4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="178b4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="178b4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="178b4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="178b4-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="178b4-117">Request headers</span></span>

| <span data-ttu-id="178b4-118">名称</span><span class="sxs-lookup"><span data-stu-id="178b4-118">Name</span></span>          | <span data-ttu-id="178b4-119">说明</span><span class="sxs-lookup"><span data-stu-id="178b4-119">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="178b4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="178b4-120">Authorization</span></span> | <span data-ttu-id="178b4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="178b4-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="178b4-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="178b4-123">Content-Type</span></span>  | <span data-ttu-id="178b4-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="178b4-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="178b4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="178b4-126">Request body</span></span>

<span data-ttu-id="178b4-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="178b4-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="178b4-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="178b4-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="178b4-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="178b4-129">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="178b4-130">有关属性的列表，请参阅[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="178b4-130">For the list of properties, see [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span></span>

## <a name="response"></a><span data-ttu-id="178b4-131">响应</span><span class="sxs-lookup"><span data-stu-id="178b4-131">Response</span></span>

<span data-ttu-id="178b4-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="178b4-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="178b4-134">示例</span><span class="sxs-lookup"><span data-stu-id="178b4-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="178b4-135">请求</span><span class="sxs-lookup"><span data-stu-id="178b4-135">Request</span></span>

<span data-ttu-id="178b4-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="178b4-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="178b4-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="178b4-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_conditionalaccesspolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/conditionalAccess/policies/{id}
Content-type: application/json

{
    "conditions": {
        "signInRiskLevels": [
            "high",
            "medium",
            "low",
        ]
    }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="178b4-138">C#</span><span class="sxs-lookup"><span data-stu-id="178b4-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="178b4-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="178b4-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="178b4-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="178b4-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="178b4-141">响应</span><span class="sxs-lookup"><span data-stu-id="178b4-141">Response</span></span>

<span data-ttu-id="178b4-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="178b4-142">The following is an example of the response.</span></span>

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
  "description": "Update conditionalaccesspolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
