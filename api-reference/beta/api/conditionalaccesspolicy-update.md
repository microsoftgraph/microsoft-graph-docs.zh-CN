---
title: 更新 conditionalAccessPolicy
description: 更新 conditionalAccessPolicy 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7716697d6dd5cdb852c0851c301dba00b28f3fe8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437957"
---
# <a name="update-conditionalaccesspolicy"></a><span data-ttu-id="17005-103">更新 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="17005-103">Update conditionalAccessPolicy</span></span>

<span data-ttu-id="17005-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="17005-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17005-105">更新[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="17005-105">Update the properties of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="17005-106">权限</span><span class="sxs-lookup"><span data-stu-id="17005-106">Permissions</span></span>

<span data-ttu-id="17005-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17005-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17005-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="17005-109">Permission type</span></span>                        | <span data-ttu-id="17005-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17005-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="17005-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17005-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="17005-112">ConditionalAccess 和应用程序的读取。 All</span><span class="sxs-lookup"><span data-stu-id="17005-112">Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
|<span data-ttu-id="17005-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17005-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17005-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="17005-114">Not supported.</span></span> |
|<span data-ttu-id="17005-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="17005-115">Application</span></span>                            | <span data-ttu-id="17005-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="17005-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="17005-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17005-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="17005-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="17005-118">Request headers</span></span>

| <span data-ttu-id="17005-119">名称</span><span class="sxs-lookup"><span data-stu-id="17005-119">Name</span></span>          | <span data-ttu-id="17005-120">说明</span><span class="sxs-lookup"><span data-stu-id="17005-120">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="17005-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="17005-121">Authorization</span></span> | <span data-ttu-id="17005-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="17005-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="17005-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="17005-124">Content-Type</span></span>  | <span data-ttu-id="17005-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="17005-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17005-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="17005-127">Request body</span></span>

<span data-ttu-id="17005-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="17005-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="17005-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="17005-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="17005-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="17005-130">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="17005-131">有关属性的列表，请参阅[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="17005-131">For the list of properties, see [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span></span>

## <a name="response"></a><span data-ttu-id="17005-132">响应</span><span class="sxs-lookup"><span data-stu-id="17005-132">Response</span></span>

<span data-ttu-id="17005-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="17005-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="17005-135">示例</span><span class="sxs-lookup"><span data-stu-id="17005-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="17005-136">请求</span><span class="sxs-lookup"><span data-stu-id="17005-136">Request</span></span>

<span data-ttu-id="17005-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="17005-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="17005-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="17005-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="17005-139">C#</span><span class="sxs-lookup"><span data-stu-id="17005-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17005-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17005-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17005-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17005-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="17005-142">响应</span><span class="sxs-lookup"><span data-stu-id="17005-142">Response</span></span>

<span data-ttu-id="17005-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="17005-143">The following is an example of the response.</span></span>

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
