---
title: 'groupLifecyclePolicy: removeGroup'
description: 从生命周期策略中删除组。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3f609681f13f1e0503b3bff723f15869c7e25704
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001839"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="e7857-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="e7857-103">groupLifecyclePolicy: removeGroup</span></span>

<span data-ttu-id="e7857-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7857-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7857-105">从生命周期策略中删除组。</span><span class="sxs-lookup"><span data-stu-id="e7857-105">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7857-106">权限</span><span class="sxs-lookup"><span data-stu-id="e7857-106">Permissions</span></span>

<span data-ttu-id="e7857-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7857-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e7857-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7857-109">Permission type</span></span>      | <span data-ttu-id="e7857-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e7857-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7857-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7857-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e7857-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7857-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="e7857-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7857-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7857-114">不支持</span><span class="sxs-lookup"><span data-stu-id="e7857-114">Not supported</span></span> |
|<span data-ttu-id="e7857-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7857-115">Application</span></span> |  <span data-ttu-id="e7857-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7857-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7857-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7857-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="e7857-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7857-118">Request headers</span></span>

| <span data-ttu-id="e7857-119">名称</span><span class="sxs-lookup"><span data-stu-id="e7857-119">Name</span></span> | <span data-ttu-id="e7857-120">说明</span><span class="sxs-lookup"><span data-stu-id="e7857-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e7857-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7857-121">Authorization</span></span> | <span data-ttu-id="e7857-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e7857-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e7857-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e7857-124">Content-Type</span></span>  | <span data-ttu-id="e7857-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7857-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7857-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7857-126">Request body</span></span>
<span data-ttu-id="e7857-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e7857-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e7857-128">参数</span><span class="sxs-lookup"><span data-stu-id="e7857-128">Parameter</span></span> | <span data-ttu-id="e7857-129">类型</span><span class="sxs-lookup"><span data-stu-id="e7857-129">Type</span></span> | <span data-ttu-id="e7857-130">说明</span><span class="sxs-lookup"><span data-stu-id="e7857-130">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e7857-131">groupId</span><span class="sxs-lookup"><span data-stu-id="e7857-131">groupId</span></span>|<span data-ttu-id="e7857-132">Guid</span><span class="sxs-lookup"><span data-stu-id="e7857-132">Guid</span></span>| <span data-ttu-id="e7857-133">要从策略中删除的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="e7857-133">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="e7857-134">响应</span><span class="sxs-lookup"><span data-stu-id="e7857-134">Response</span></span>

<span data-ttu-id="e7857-135">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e7857-135">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="e7857-136">如果已从策略中删除组，响应正文中返回 **true** 值。</span><span class="sxs-lookup"><span data-stu-id="e7857-136">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="e7857-137">否则，响应正文中返回 **false** 值。</span><span class="sxs-lookup"><span data-stu-id="e7857-137">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="e7857-138">示例</span><span class="sxs-lookup"><span data-stu-id="e7857-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e7857-139">请求</span><span class="sxs-lookup"><span data-stu-id="e7857-139">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_removegroup"
} -->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}/removeGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="e7857-140">响应</span><span class="sxs-lookup"><span data-stu-id="e7857-140">Response</span></span>
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
  "description": "groupLifecyclePolicy: removegroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


