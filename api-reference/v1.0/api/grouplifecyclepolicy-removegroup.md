---
title: 'groupLifecyclePolicy: removeGroup'
description: 从生命周期策略中删除组。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 33e5900c93801f54f4f705f59d25895e32da797d
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124628"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="69169-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="69169-103">groupLifecyclePolicy: removeGroup</span></span>

<span data-ttu-id="69169-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69169-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69169-105">从生命周期策略中删除组。</span><span class="sxs-lookup"><span data-stu-id="69169-105">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="69169-106">权限</span><span class="sxs-lookup"><span data-stu-id="69169-106">Permissions</span></span>

<span data-ttu-id="69169-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69169-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69169-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="69169-109">Permission type</span></span>      | <span data-ttu-id="69169-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69169-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69169-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69169-111">Delegated (work or school account)</span></span> | <span data-ttu-id="69169-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69169-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="69169-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69169-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69169-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="69169-114">Not supported.</span></span>    |
|<span data-ttu-id="69169-115">Application</span><span class="sxs-lookup"><span data-stu-id="69169-115">Application</span></span> | <span data-ttu-id="69169-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69169-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69169-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69169-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="69169-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="69169-118">Request headers</span></span>

| <span data-ttu-id="69169-119">名称</span><span class="sxs-lookup"><span data-stu-id="69169-119">Name</span></span> | <span data-ttu-id="69169-120">说明</span><span class="sxs-lookup"><span data-stu-id="69169-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="69169-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="69169-121">Authorization</span></span> | <span data-ttu-id="69169-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="69169-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="69169-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="69169-124">Content-Type</span></span>  | <span data-ttu-id="69169-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69169-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="69169-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="69169-126">Request body</span></span>
<span data-ttu-id="69169-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="69169-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="69169-128">参数</span><span class="sxs-lookup"><span data-stu-id="69169-128">Parameter</span></span> | <span data-ttu-id="69169-129">类型</span><span class="sxs-lookup"><span data-stu-id="69169-129">Type</span></span> | <span data-ttu-id="69169-130">说明</span><span class="sxs-lookup"><span data-stu-id="69169-130">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="69169-131">groupId</span><span class="sxs-lookup"><span data-stu-id="69169-131">groupId</span></span>|<span data-ttu-id="69169-132">Guid</span><span class="sxs-lookup"><span data-stu-id="69169-132">Guid</span></span>| <span data-ttu-id="69169-133">要从策略中删除的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="69169-133">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="69169-134">响应</span><span class="sxs-lookup"><span data-stu-id="69169-134">Response</span></span>

<span data-ttu-id="69169-135">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="69169-135">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="69169-136">如果已从策略中删除组，响应正文中返回 **true** 值。</span><span class="sxs-lookup"><span data-stu-id="69169-136">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="69169-137">否则，响应正文中返回 **false** 值。</span><span class="sxs-lookup"><span data-stu-id="69169-137">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="69169-138">示例</span><span class="sxs-lookup"><span data-stu-id="69169-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="69169-139">请求</span><span class="sxs-lookup"><span data-stu-id="69169-139">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_removegroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/removeGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

##### <a name="response"></a><span data-ttu-id="69169-140">响应</span><span class="sxs-lookup"><span data-stu-id="69169-140">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: removegroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
