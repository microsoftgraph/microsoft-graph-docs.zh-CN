---
title: groupLifecyclePolicy：renewGroup
description: 续订组的过期时间。 续订后，组的有效期就会延长策略中定义的天数。
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: be7f1222933b5923b475d55c0b7c6b8a4bcf24aa
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681111"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="6d1a8-104">groupLifecyclePolicy：renewGroup</span><span class="sxs-lookup"><span data-stu-id="6d1a8-104">groupLifecyclePolicy: renewGroup</span></span>

<span data-ttu-id="6d1a8-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d1a8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d1a8-106">续订组的过期时间。</span><span class="sxs-lookup"><span data-stu-id="6d1a8-106">Renew a group's expiration.</span></span> <span data-ttu-id="6d1a8-107">续订后，组的有效期就会延长策略中定义的天数。</span><span class="sxs-lookup"><span data-stu-id="6d1a8-107">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="6d1a8-108">**注意：** 调用 v1.0 终结点时，请使用 [Renew 组](/graph/api/group-renew?view=graph-rest-1.0&preserve-view=true) 方法。</span><span class="sxs-lookup"><span data-stu-id="6d1a8-108">**Note:** When calling the v1.0 endpoint, use the [Renew group](/graph/api/group-renew?view=graph-rest-1.0&preserve-view=true) method.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d1a8-109">权限</span><span class="sxs-lookup"><span data-stu-id="6d1a8-109">Permissions</span></span>

<span data-ttu-id="6d1a8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d1a8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="6d1a8-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d1a8-112">Permission type</span></span>      | <span data-ttu-id="6d1a8-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6d1a8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d1a8-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d1a8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6d1a8-115">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d1a8-115">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="6d1a8-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d1a8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d1a8-117">不支持</span><span class="sxs-lookup"><span data-stu-id="6d1a8-117">Not supported</span></span> |
|<span data-ttu-id="6d1a8-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d1a8-118">Application</span></span> | <span data-ttu-id="6d1a8-119">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d1a8-119">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d1a8-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d1a8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="6d1a8-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d1a8-121">Request headers</span></span>

| <span data-ttu-id="6d1a8-122">名称</span><span class="sxs-lookup"><span data-stu-id="6d1a8-122">Name</span></span> | <span data-ttu-id="6d1a8-123">说明</span><span class="sxs-lookup"><span data-stu-id="6d1a8-123">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="6d1a8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d1a8-124">Authorization</span></span> | <span data-ttu-id="6d1a8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6d1a8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6d1a8-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d1a8-127">Content-Type</span></span>  | <span data-ttu-id="6d1a8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="6d1a8-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d1a8-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d1a8-129">Request body</span></span>
<span data-ttu-id="6d1a8-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6d1a8-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6d1a8-131">参数</span><span class="sxs-lookup"><span data-stu-id="6d1a8-131">Parameter</span></span> | <span data-ttu-id="6d1a8-132">类型</span><span class="sxs-lookup"><span data-stu-id="6d1a8-132">Type</span></span> | <span data-ttu-id="6d1a8-133">说明</span><span class="sxs-lookup"><span data-stu-id="6d1a8-133">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6d1a8-134">groupId</span><span class="sxs-lookup"><span data-stu-id="6d1a8-134">groupId</span></span>|<span data-ttu-id="6d1a8-135">Guid</span><span class="sxs-lookup"><span data-stu-id="6d1a8-135">Guid</span></span>| <span data-ttu-id="6d1a8-136">要续订的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="6d1a8-136">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="6d1a8-137">响应</span><span class="sxs-lookup"><span data-stu-id="6d1a8-137">Response</span></span>

<span data-ttu-id="6d1a8-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6d1a8-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d1a8-140">示例</span><span class="sxs-lookup"><span data-stu-id="6d1a8-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6d1a8-141">请求</span><span class="sxs-lookup"><span data-stu-id="6d1a8-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6d1a8-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d1a8-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6d1a8-143">C#</span><span class="sxs-lookup"><span data-stu-id="6d1a8-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/grouplifecyclepolicy-renewgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d1a8-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d1a8-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/grouplifecyclepolicy-renewgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d1a8-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d1a8-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/grouplifecyclepolicy-renewgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6d1a8-146">Java</span><span class="sxs-lookup"><span data-stu-id="6d1a8-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/grouplifecyclepolicy-renewgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6d1a8-147">响应</span><span class="sxs-lookup"><span data-stu-id="6d1a8-147">Response</span></span>

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
