---
title: 'groupLifecyclePolicy: renewGroup'
description: 续订组以更新到期时间。 续订后，组的有效期就会延长策略中定义的天数。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ac779d2d84619a0bfd4f4480ac2f1dda600bde22
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953295"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="063ac-104">groupLifecyclePolicy: renewGroup</span><span class="sxs-lookup"><span data-stu-id="063ac-104">groupLifecyclePolicy: renewGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="063ac-105">续订组以更新到期时间。</span><span class="sxs-lookup"><span data-stu-id="063ac-105">Renews a group's expiration.</span></span> <span data-ttu-id="063ac-106">续订后，组的有效期就会延长策略中定义的天数。</span><span class="sxs-lookup"><span data-stu-id="063ac-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="063ac-107">**注意:** 在1.0 版中,[使用组资源发出续订请求](/graph/api/group-renew?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="063ac-107">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="063ac-108">权限</span><span class="sxs-lookup"><span data-stu-id="063ac-108">Permissions</span></span>

<span data-ttu-id="063ac-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="063ac-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="063ac-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="063ac-111">Permission type</span></span>      | <span data-ttu-id="063ac-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="063ac-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="063ac-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="063ac-113">Delegated (work or school account)</span></span> | <span data-ttu-id="063ac-114">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="063ac-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="063ac-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="063ac-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="063ac-116">不支持</span><span class="sxs-lookup"><span data-stu-id="063ac-116">Not supported</span></span> |
|<span data-ttu-id="063ac-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="063ac-117">Application</span></span> | <span data-ttu-id="063ac-118">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="063ac-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="063ac-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="063ac-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="063ac-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="063ac-120">Request headers</span></span>

| <span data-ttu-id="063ac-121">名称</span><span class="sxs-lookup"><span data-stu-id="063ac-121">Name</span></span> | <span data-ttu-id="063ac-122">说明</span><span class="sxs-lookup"><span data-stu-id="063ac-122">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="063ac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="063ac-123">Authorization</span></span> | <span data-ttu-id="063ac-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="063ac-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="063ac-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="063ac-126">Content-Type</span></span>  | <span data-ttu-id="063ac-127">application/json</span><span class="sxs-lookup"><span data-stu-id="063ac-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="063ac-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="063ac-128">Request body</span></span>
<span data-ttu-id="063ac-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="063ac-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="063ac-130">参数</span><span class="sxs-lookup"><span data-stu-id="063ac-130">Parameter</span></span> | <span data-ttu-id="063ac-131">类型</span><span class="sxs-lookup"><span data-stu-id="063ac-131">Type</span></span> | <span data-ttu-id="063ac-132">说明</span><span class="sxs-lookup"><span data-stu-id="063ac-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="063ac-133">groupId</span><span class="sxs-lookup"><span data-stu-id="063ac-133">groupId</span></span>|<span data-ttu-id="063ac-134">Guid</span><span class="sxs-lookup"><span data-stu-id="063ac-134">Guid</span></span>| <span data-ttu-id="063ac-135">要续订的组的 id。</span><span class="sxs-lookup"><span data-stu-id="063ac-135">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="063ac-136">响应</span><span class="sxs-lookup"><span data-stu-id="063ac-136">Response</span></span>

<span data-ttu-id="063ac-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="063ac-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="063ac-139">示例</span><span class="sxs-lookup"><span data-stu-id="063ac-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="063ac-140">请求</span><span class="sxs-lookup"><span data-stu-id="063ac-140">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="063ac-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="063ac-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="063ac-142">C#</span><span class="sxs-lookup"><span data-stu-id="063ac-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/grouplifecyclepolicy-renewgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="063ac-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="063ac-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/grouplifecyclepolicy-renewgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="063ac-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="063ac-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/grouplifecyclepolicy-renewgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="063ac-145">Java</span><span class="sxs-lookup"><span data-stu-id="063ac-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/grouplifecyclepolicy-renewgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="063ac-146">响应</span><span class="sxs-lookup"><span data-stu-id="063ac-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
