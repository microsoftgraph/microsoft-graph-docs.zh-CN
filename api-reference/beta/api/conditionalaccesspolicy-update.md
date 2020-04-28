---
title: 更新 conditionalAccessPolicy
description: 更新 conditionalAccessPolicy 对象的属性。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bed88872a69164e48cba80b1ab3925328b24b7c0
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916467"
---
# <a name="update-conditionalaccesspolicy"></a><span data-ttu-id="f52bd-103">更新 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="f52bd-103">Update conditionalAccessPolicy</span></span>

<span data-ttu-id="f52bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f52bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f52bd-105">更新[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f52bd-105">Update the properties of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f52bd-106">权限</span><span class="sxs-lookup"><span data-stu-id="f52bd-106">Permissions</span></span>

<span data-ttu-id="f52bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f52bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f52bd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f52bd-109">Permission type</span></span>                        | <span data-ttu-id="f52bd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f52bd-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="f52bd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f52bd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f52bd-112">Policy. All、ConditionalAccess 和 Application。 Read. All</span><span class="sxs-lookup"><span data-stu-id="f52bd-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess and Application.Read.All</span></span> |
|<span data-ttu-id="f52bd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f52bd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f52bd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f52bd-114">Not supported.</span></span> |
|<span data-ttu-id="f52bd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f52bd-115">Application</span></span>                            | <span data-ttu-id="f52bd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f52bd-116">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="f52bd-117">此 API 存在与权限相关的[已知问题](/graph/known-issues#permissions)。</span><span class="sxs-lookup"><span data-stu-id="f52bd-117">This API has a [known issue](/graph/known-issues#permissions) related to permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="f52bd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f52bd-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f52bd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f52bd-119">Request headers</span></span>

| <span data-ttu-id="f52bd-120">名称</span><span class="sxs-lookup"><span data-stu-id="f52bd-120">Name</span></span>          | <span data-ttu-id="f52bd-121">说明</span><span class="sxs-lookup"><span data-stu-id="f52bd-121">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="f52bd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f52bd-122">Authorization</span></span> | <span data-ttu-id="f52bd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f52bd-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="f52bd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f52bd-125">Content-Type</span></span>  | <span data-ttu-id="f52bd-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f52bd-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f52bd-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f52bd-128">Request body</span></span>

<span data-ttu-id="f52bd-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="f52bd-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f52bd-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="f52bd-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f52bd-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="f52bd-131">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="f52bd-132">有关属性的列表，请参阅[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="f52bd-132">For the list of properties, see [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span></span>

## <a name="response"></a><span data-ttu-id="f52bd-133">响应</span><span class="sxs-lookup"><span data-stu-id="f52bd-133">Response</span></span>

<span data-ttu-id="f52bd-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f52bd-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f52bd-136">示例</span><span class="sxs-lookup"><span data-stu-id="f52bd-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f52bd-137">请求</span><span class="sxs-lookup"><span data-stu-id="f52bd-137">Request</span></span>

<span data-ttu-id="f52bd-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f52bd-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f52bd-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="f52bd-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_conditionalaccesspolicy"
}-->

```http
PATCH https://graph.microsoft.com/beta/identity/conditionalAccess/policies/{id}
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
# <a name="c"></a>[<span data-ttu-id="f52bd-140">C#</span><span class="sxs-lookup"><span data-stu-id="f52bd-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f52bd-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f52bd-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f52bd-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f52bd-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f52bd-143">响应</span><span class="sxs-lookup"><span data-stu-id="f52bd-143">Response</span></span>

<span data-ttu-id="f52bd-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f52bd-144">The following is an example of the response.</span></span>

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
