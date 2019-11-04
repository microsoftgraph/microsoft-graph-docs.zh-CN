---
title: 更新 conditionalAccessPolicy
description: 更新 conditionalAccessPolicy 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c290faff53b98e28dc9876b9fd76abac8a813196
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936707"
---
# <a name="update-conditionalaccesspolicy"></a><span data-ttu-id="657b5-103">更新 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="657b5-103">Update conditionalAccessPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="657b5-104">更新[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="657b5-104">Update the properties of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="657b5-105">权限</span><span class="sxs-lookup"><span data-stu-id="657b5-105">Permissions</span></span>

<span data-ttu-id="657b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="657b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="657b5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="657b5-108">Permission type</span></span>                        | <span data-ttu-id="657b5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="657b5-109">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="657b5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="657b5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="657b5-111">ConditionalAccess 和 Directory.accessasuser.all 的所有</span><span class="sxs-lookup"><span data-stu-id="657b5-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="657b5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="657b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="657b5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="657b5-113">Not supported.</span></span> |
|<span data-ttu-id="657b5-114">Application</span><span class="sxs-lookup"><span data-stu-id="657b5-114">Application</span></span>                            | <span data-ttu-id="657b5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="657b5-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="657b5-116">此 API 需要多个权限。</span><span class="sxs-lookup"><span data-stu-id="657b5-116">This API requires multiple permissions.</span></span> <span data-ttu-id="657b5-117">有关详细信息，请参阅[已知问题](/graph/known-issues#conditional-access-policies-and-named-locations)。</span><span class="sxs-lookup"><span data-stu-id="657b5-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="657b5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="657b5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="657b5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="657b5-119">Request headers</span></span>

| <span data-ttu-id="657b5-120">名称</span><span class="sxs-lookup"><span data-stu-id="657b5-120">Name</span></span>          | <span data-ttu-id="657b5-121">说明</span><span class="sxs-lookup"><span data-stu-id="657b5-121">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="657b5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="657b5-122">Authorization</span></span> | <span data-ttu-id="657b5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="657b5-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="657b5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="657b5-125">Content-Type</span></span>  | <span data-ttu-id="657b5-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="657b5-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="657b5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="657b5-128">Request body</span></span>

<span data-ttu-id="657b5-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="657b5-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="657b5-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="657b5-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="657b5-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="657b5-131">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="657b5-132">有关属性的列表，请参阅[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="657b5-132">For the list of properties, see [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span></span>

## <a name="response"></a><span data-ttu-id="657b5-133">响应</span><span class="sxs-lookup"><span data-stu-id="657b5-133">Response</span></span>

<span data-ttu-id="657b5-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="657b5-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="657b5-136">示例</span><span class="sxs-lookup"><span data-stu-id="657b5-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="657b5-137">请求</span><span class="sxs-lookup"><span data-stu-id="657b5-137">Request</span></span>

<span data-ttu-id="657b5-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="657b5-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="657b5-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="657b5-139">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="657b5-140">C#</span><span class="sxs-lookup"><span data-stu-id="657b5-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="657b5-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="657b5-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="657b5-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="657b5-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="657b5-143">响应</span><span class="sxs-lookup"><span data-stu-id="657b5-143">Response</span></span>

<span data-ttu-id="657b5-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="657b5-144">The following is an example of the response.</span></span>

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
