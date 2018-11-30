---
title: 'groupLifecyclePolicy: renewGroup'
description: 续订组以更新到期时间。 续订后，组的有效期就会延长策略中定义的天数。
ms.openlocfilehash: 13e1713d3d00e7feac0b23eae8a314e55341e20e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044257"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="d4090-104">groupLifecyclePolicy: renewGroup</span><span class="sxs-lookup"><span data-stu-id="d4090-104">groupLifecyclePolicy: renewGroup</span></span>

> <span data-ttu-id="d4090-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d4090-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4090-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d4090-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4090-107">续订组以更新到期时间。</span><span class="sxs-lookup"><span data-stu-id="d4090-107">Renews a group's expiration.</span></span> <span data-ttu-id="d4090-108">续订后，组的有效期就会延长策略中定义的天数。</span><span class="sxs-lookup"><span data-stu-id="d4090-108">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="d4090-109">**注意：** 在 V1.0，可[使用 group 资源，以使续订请求](/graph/api/group-renew?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="d4090-109">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="d4090-110">权限</span><span class="sxs-lookup"><span data-stu-id="d4090-110">Permissions</span></span>

<span data-ttu-id="d4090-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4090-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="d4090-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4090-113">Permission type</span></span>      | <span data-ttu-id="d4090-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d4090-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4090-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4090-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d4090-116">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4090-116">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="d4090-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4090-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4090-118">不支持</span><span class="sxs-lookup"><span data-stu-id="d4090-118">Not supported</span></span> |
|<span data-ttu-id="d4090-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4090-119">Application</span></span> | <span data-ttu-id="d4090-120">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4090-120">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4090-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4090-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="d4090-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4090-122">Request headers</span></span>

| <span data-ttu-id="d4090-123">名称</span><span class="sxs-lookup"><span data-stu-id="d4090-123">Name</span></span> | <span data-ttu-id="d4090-124">说明</span><span class="sxs-lookup"><span data-stu-id="d4090-124">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d4090-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4090-125">Authorization</span></span> | <span data-ttu-id="d4090-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d4090-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d4090-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d4090-128">Content-Type</span></span>  | <span data-ttu-id="d4090-129">application/json</span><span class="sxs-lookup"><span data-stu-id="d4090-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4090-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4090-130">Request body</span></span>
<span data-ttu-id="d4090-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d4090-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d4090-132">参数</span><span class="sxs-lookup"><span data-stu-id="d4090-132">Parameter</span></span> | <span data-ttu-id="d4090-133">类型</span><span class="sxs-lookup"><span data-stu-id="d4090-133">Type</span></span> | <span data-ttu-id="d4090-134">说明</span><span class="sxs-lookup"><span data-stu-id="d4090-134">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d4090-135">groupId</span><span class="sxs-lookup"><span data-stu-id="d4090-135">groupId</span></span>|<span data-ttu-id="d4090-136">Guid</span><span class="sxs-lookup"><span data-stu-id="d4090-136">Guid</span></span>| <span data-ttu-id="d4090-137">要更新的组 id。</span><span class="sxs-lookup"><span data-stu-id="d4090-137">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="d4090-138">响应</span><span class="sxs-lookup"><span data-stu-id="d4090-138">Response</span></span>

<span data-ttu-id="d4090-p106">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d4090-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4090-141">示例</span><span class="sxs-lookup"><span data-stu-id="d4090-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d4090-142">请求</span><span class="sxs-lookup"><span data-stu-id="d4090-142">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="d4090-143">响应</span><span class="sxs-lookup"><span data-stu-id="d4090-143">Response</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: renewgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->