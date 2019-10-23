---
title: 更新 conditionalAccessPolicy
description: 更新 conditionalAccessPolicy 对象的属性。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9ef732cbc58028a8665172cec87a2d079f55925a
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638426"
---
# <a name="update-conditionalaccesspolicy"></a><span data-ttu-id="d602a-103">更新 conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="d602a-103">Update conditionalAccessPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d602a-104">更新[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d602a-104">Update the properties of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d602a-105">权限</span><span class="sxs-lookup"><span data-stu-id="d602a-105">Permissions</span></span>

<span data-ttu-id="d602a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d602a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d602a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d602a-108">Permission type</span></span>                        | <span data-ttu-id="d602a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d602a-109">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="d602a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d602a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d602a-111">ConditionalAccess 和 Directory.accessasuser.all 的所有</span><span class="sxs-lookup"><span data-stu-id="d602a-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="d602a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d602a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d602a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d602a-113">Not supported.</span></span> |
|<span data-ttu-id="d602a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d602a-114">Application</span></span>                            | <span data-ttu-id="d602a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d602a-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="d602a-116">此 API 需要多个权限。</span><span class="sxs-lookup"><span data-stu-id="d602a-116">This API requires multiple permissions.</span></span> <span data-ttu-id="d602a-117">有关详细信息，请参阅[已知问题](/graph/known-issues#conditional-access-policies-and-named-locations)。</span><span class="sxs-lookup"><span data-stu-id="d602a-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="d602a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d602a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d602a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d602a-119">Request headers</span></span>

| <span data-ttu-id="d602a-120">名称</span><span class="sxs-lookup"><span data-stu-id="d602a-120">Name</span></span>          | <span data-ttu-id="d602a-121">说明</span><span class="sxs-lookup"><span data-stu-id="d602a-121">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="d602a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d602a-122">Authorization</span></span> | <span data-ttu-id="d602a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d602a-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d602a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d602a-125">Content-Type</span></span>  | <span data-ttu-id="d602a-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d602a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d602a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d602a-128">Request body</span></span>

<span data-ttu-id="d602a-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="d602a-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d602a-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="d602a-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d602a-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d602a-131">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="d602a-132">有关属性的列表，请参阅[conditionalAccessPolicy](../resources/conditionalaccesspolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="d602a-132">For the list of properties, see [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md).</span></span>

## <a name="response"></a><span data-ttu-id="d602a-133">响应</span><span class="sxs-lookup"><span data-stu-id="d602a-133">Response</span></span>

<span data-ttu-id="d602a-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d602a-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d602a-136">示例</span><span class="sxs-lookup"><span data-stu-id="d602a-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d602a-137">请求</span><span class="sxs-lookup"><span data-stu-id="d602a-137">Request</span></span>

<span data-ttu-id="d602a-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d602a-138">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d602a-139">响应</span><span class="sxs-lookup"><span data-stu-id="d602a-139">Response</span></span>

<span data-ttu-id="d602a-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d602a-140">The following is an example of the response.</span></span>

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
