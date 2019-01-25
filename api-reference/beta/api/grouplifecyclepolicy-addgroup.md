---
title: 'groupLifecyclePolicy: addGroup'
description: 将组添加到生命周期策略。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f5aee25421dea76b5bdb10f141d4e640c2196b94
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515508"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="8f182-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="8f182-103">groupLifecyclePolicy: addGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f182-104">将组添加到生命周期策略。</span><span class="sxs-lookup"><span data-stu-id="8f182-104">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f182-105">权限</span><span class="sxs-lookup"><span data-stu-id="8f182-105">Permissions</span></span>

<span data-ttu-id="8f182-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f182-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8f182-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f182-108">Permission type</span></span>      | <span data-ttu-id="8f182-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f182-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f182-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f182-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8f182-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f182-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="8f182-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f182-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f182-113">不支持</span><span class="sxs-lookup"><span data-stu-id="8f182-113">Not supported</span></span> |
|<span data-ttu-id="8f182-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f182-114">Application</span></span> | <span data-ttu-id="8f182-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f182-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f182-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f182-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="8f182-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f182-117">Request headers</span></span>

| <span data-ttu-id="8f182-118">名称</span><span class="sxs-lookup"><span data-stu-id="8f182-118">Name</span></span> | <span data-ttu-id="8f182-119">说明</span><span class="sxs-lookup"><span data-stu-id="8f182-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="8f182-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f182-120">Authorization</span></span> | <span data-ttu-id="8f182-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f182-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f182-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f182-123">Content-Type</span></span>  | <span data-ttu-id="8f182-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8f182-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f182-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f182-125">Request body</span></span>
<span data-ttu-id="8f182-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="8f182-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8f182-127">参数</span><span class="sxs-lookup"><span data-stu-id="8f182-127">Parameter</span></span> | <span data-ttu-id="8f182-128">类型</span><span class="sxs-lookup"><span data-stu-id="8f182-128">Type</span></span> | <span data-ttu-id="8f182-129">说明</span><span class="sxs-lookup"><span data-stu-id="8f182-129">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8f182-130">groupId</span><span class="sxs-lookup"><span data-stu-id="8f182-130">groupId</span></span>|<span data-ttu-id="8f182-131">Guid</span><span class="sxs-lookup"><span data-stu-id="8f182-131">Guid</span></span>| <span data-ttu-id="8f182-132">要添加到策略的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="8f182-132">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="8f182-133">响应</span><span class="sxs-lookup"><span data-stu-id="8f182-133">Response</span></span>

<span data-ttu-id="8f182-134">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8f182-134">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="8f182-135">如果组已添加到策略，便会在响应正文中返回 **true** 值。</span><span class="sxs-lookup"><span data-stu-id="8f182-135">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="8f182-136">否则，响应正文中返回 **false** 值。</span><span class="sxs-lookup"><span data-stu-id="8f182-136">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="8f182-137">示例</span><span class="sxs-lookup"><span data-stu-id="8f182-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8f182-138">请求</span><span class="sxs-lookup"><span data-stu-id="8f182-138">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}/addGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

#### <a name="response"></a><span data-ttu-id="8f182-139">响应</span><span class="sxs-lookup"><span data-stu-id="8f182-139">Response</span></span>
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 21

{
  "value": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-addgroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
