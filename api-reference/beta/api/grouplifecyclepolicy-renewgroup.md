---
title: 'groupLifecyclePolicy: renewGroup'
description: 续订组以更新到期时间。 续订后，组的有效期就会延长策略中定义的天数。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 7eb0ef44a5e07c8c293ba804cc8ec31a8312576d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520870"
---
# <a name="grouplifecyclepolicy-renewgroup"></a><span data-ttu-id="c4563-104">groupLifecyclePolicy: renewGroup</span><span class="sxs-lookup"><span data-stu-id="c4563-104">groupLifecyclePolicy: renewGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4563-105">续订组以更新到期时间。</span><span class="sxs-lookup"><span data-stu-id="c4563-105">Renews a group's expiration.</span></span> <span data-ttu-id="c4563-106">续订后，组的有效期就会延长策略中定义的天数。</span><span class="sxs-lookup"><span data-stu-id="c4563-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

> <span data-ttu-id="c4563-107">**注意：** 在 V1.0，可[使用 group 资源，以使续订请求](/graph/api/group-renew?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="c4563-107">**Note:** In V1.0, [use the group resource to make renew requests](/graph/api/group-renew?view=graph-rest-1.0).</span></span>

## <a name="permissions"></a><span data-ttu-id="c4563-108">权限</span><span class="sxs-lookup"><span data-stu-id="c4563-108">Permissions</span></span>

<span data-ttu-id="c4563-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4563-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="c4563-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4563-111">Permission type</span></span>      | <span data-ttu-id="c4563-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4563-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4563-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4563-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c4563-114">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4563-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="c4563-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4563-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4563-116">不支持</span><span class="sxs-lookup"><span data-stu-id="c4563-116">Not supported</span></span> |
|<span data-ttu-id="c4563-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4563-117">Application</span></span> | <span data-ttu-id="c4563-118">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4563-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4563-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4563-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/renewGroup

```

## <a name="request-headers"></a><span data-ttu-id="c4563-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4563-120">Request headers</span></span>

| <span data-ttu-id="c4563-121">名称</span><span class="sxs-lookup"><span data-stu-id="c4563-121">Name</span></span> | <span data-ttu-id="c4563-122">说明</span><span class="sxs-lookup"><span data-stu-id="c4563-122">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="c4563-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4563-123">Authorization</span></span> | <span data-ttu-id="c4563-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4563-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c4563-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4563-126">Content-Type</span></span>  | <span data-ttu-id="c4563-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c4563-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4563-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4563-128">Request body</span></span>
<span data-ttu-id="c4563-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c4563-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c4563-130">参数</span><span class="sxs-lookup"><span data-stu-id="c4563-130">Parameter</span></span> | <span data-ttu-id="c4563-131">类型</span><span class="sxs-lookup"><span data-stu-id="c4563-131">Type</span></span> | <span data-ttu-id="c4563-132">说明</span><span class="sxs-lookup"><span data-stu-id="c4563-132">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c4563-133">groupId</span><span class="sxs-lookup"><span data-stu-id="c4563-133">groupId</span></span>|<span data-ttu-id="c4563-134">Guid</span><span class="sxs-lookup"><span data-stu-id="c4563-134">Guid</span></span>| <span data-ttu-id="c4563-135">要更新的组 id。</span><span class="sxs-lookup"><span data-stu-id="c4563-135">The id of the group to renew.</span></span> |

## <a name="response"></a><span data-ttu-id="c4563-136">响应</span><span class="sxs-lookup"><span data-stu-id="c4563-136">Response</span></span>

<span data-ttu-id="c4563-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c4563-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4563-139">示例</span><span class="sxs-lookup"><span data-stu-id="c4563-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c4563-140">请求</span><span class="sxs-lookup"><span data-stu-id="c4563-140">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="c4563-141">响应</span><span class="sxs-lookup"><span data-stu-id="c4563-141">Response</span></span>

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
    "Error: /api-reference/beta/api/grouplifecyclepolicy-renewgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
