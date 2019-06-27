---
title: 'groupLifecyclePolicy: renewGroup'
description: 续订组以更新到期时间。 续订后，组的有效期就会延长策略中定义的天数。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: d07025b076e78193f1c712d70892bd5a262ea2a2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262732"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="3dc73-104">groupLifecyclePolicy: renewGroup</span><span class="sxs-lookup"><span data-stu-id="3dc73-104">groupLifecyclePolicy: renewGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dc73-105">续订组以更新到期时间。</span><span class="sxs-lookup"><span data-stu-id="3dc73-105">Renews a group's expiration.</span></span> <span data-ttu-id="3dc73-106">续订后，组的有效期就会延长策略中定义的天数。</span><span class="sxs-lookup"><span data-stu-id="3dc73-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="3dc73-107">**注意:** 在1.0 版中,[使用组资源发出续订请求](/graph/api/group-renew?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="3dc73-107">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="3dc73-108">权限</span><span class="sxs-lookup"><span data-stu-id="3dc73-108">Permissions</span></span>

<span data-ttu-id="3dc73-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3dc73-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="3dc73-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3dc73-111">Permission type</span></span>      | <span data-ttu-id="3dc73-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3dc73-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3dc73-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3dc73-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3dc73-114">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dc73-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="3dc73-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3dc73-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3dc73-116">不支持</span><span class="sxs-lookup"><span data-stu-id="3dc73-116">Not supported</span></span> |
|<span data-ttu-id="3dc73-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3dc73-117">Application</span></span> | <span data-ttu-id="3dc73-118">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dc73-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3dc73-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3dc73-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="3dc73-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3dc73-120">Request headers</span></span>

| <span data-ttu-id="3dc73-121">名称</span><span class="sxs-lookup"><span data-stu-id="3dc73-121">Name</span></span> | <span data-ttu-id="3dc73-122">说明</span><span class="sxs-lookup"><span data-stu-id="3dc73-122">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="3dc73-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3dc73-123">Authorization</span></span> | <span data-ttu-id="3dc73-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3dc73-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3dc73-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3dc73-126">Content-Type</span></span>  | <span data-ttu-id="3dc73-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3dc73-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3dc73-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3dc73-128">Request body</span></span>
<span data-ttu-id="3dc73-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3dc73-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3dc73-130">参数</span><span class="sxs-lookup"><span data-stu-id="3dc73-130">Parameter</span></span> | <span data-ttu-id="3dc73-131">类型</span><span class="sxs-lookup"><span data-stu-id="3dc73-131">Type</span></span> | <span data-ttu-id="3dc73-132">说明</span><span class="sxs-lookup"><span data-stu-id="3dc73-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3dc73-133">groupId</span><span class="sxs-lookup"><span data-stu-id="3dc73-133">groupId</span></span>|<span data-ttu-id="3dc73-134">Guid</span><span class="sxs-lookup"><span data-stu-id="3dc73-134">Guid</span></span>| <span data-ttu-id="3dc73-135">要续订的组的 id。</span><span class="sxs-lookup"><span data-stu-id="3dc73-135">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="3dc73-136">响应</span><span class="sxs-lookup"><span data-stu-id="3dc73-136">Response</span></span>

<span data-ttu-id="3dc73-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3dc73-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dc73-139">示例</span><span class="sxs-lookup"><span data-stu-id="3dc73-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3dc73-140">请求</span><span class="sxs-lookup"><span data-stu-id="3dc73-140">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "grouplifecyclepolicy_renewgroup"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/renewGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="3dc73-141">响应</span><span class="sxs-lookup"><span data-stu-id="3dc73-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3dc73-142">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3dc73-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3dc73-143">C#</span><span class="sxs-lookup"><span data-stu-id="3dc73-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/grouplifecyclepolicy_renewgroup-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3dc73-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="3dc73-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/grouplifecyclepolicy_renewgroup-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3dc73-145">目标-C</span><span class="sxs-lookup"><span data-stu-id="3dc73-145">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/grouplifecyclepolicy_renewgroup-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: renewgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-renewgroup.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/grouplifecyclepolicy-renewgroup.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/grouplifecyclepolicy-renewgroup.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
