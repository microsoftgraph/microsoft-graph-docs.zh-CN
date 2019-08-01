---
title: 'groupLifecyclePolicy: addGroup'
description: 将组添加到生命周期策略。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b5954d475288dab8d19755150c8510f145836204
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014632"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="7e633-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="7e633-103">groupLifecyclePolicy: addGroup</span></span>

<span data-ttu-id="7e633-104">将组添加到生命周期策略。</span><span class="sxs-lookup"><span data-stu-id="7e633-104">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e633-105">权限</span><span class="sxs-lookup"><span data-stu-id="7e633-105">Permissions</span></span>

<span data-ttu-id="7e633-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e633-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7e633-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e633-108">Permission type</span></span>      | <span data-ttu-id="7e633-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e633-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e633-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e633-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7e633-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e633-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="7e633-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e633-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e633-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e633-113">Not supported.</span></span>    |
|<span data-ttu-id="7e633-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e633-114">Application</span></span> | <span data-ttu-id="7e633-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e633-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e633-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e633-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="7e633-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e633-117">Request headers</span></span>

| <span data-ttu-id="7e633-118">名称</span><span class="sxs-lookup"><span data-stu-id="7e633-118">Name</span></span> | <span data-ttu-id="7e633-119">说明</span><span class="sxs-lookup"><span data-stu-id="7e633-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="7e633-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e633-120">Authorization</span></span> | <span data-ttu-id="7e633-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e633-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7e633-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7e633-123">Content-Type</span></span>  | <span data-ttu-id="7e633-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7e633-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e633-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e633-125">Request body</span></span>
<span data-ttu-id="7e633-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7e633-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7e633-127">参数</span><span class="sxs-lookup"><span data-stu-id="7e633-127">Parameter</span></span> | <span data-ttu-id="7e633-128">类型</span><span class="sxs-lookup"><span data-stu-id="7e633-128">Type</span></span> | <span data-ttu-id="7e633-129">说明</span><span class="sxs-lookup"><span data-stu-id="7e633-129">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7e633-130">groupId</span><span class="sxs-lookup"><span data-stu-id="7e633-130">groupId</span></span>|<span data-ttu-id="7e633-131">Guid</span><span class="sxs-lookup"><span data-stu-id="7e633-131">Guid</span></span>| <span data-ttu-id="7e633-132">要添加到策略的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="7e633-132">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="7e633-133">响应</span><span class="sxs-lookup"><span data-stu-id="7e633-133">Response</span></span>

<span data-ttu-id="7e633-134">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7e633-134">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="7e633-135">如果组已添加到策略，便会在响应正文中返回 **true** 值。</span><span class="sxs-lookup"><span data-stu-id="7e633-135">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="7e633-136">否则，响应正文中返回 **false** 值。</span><span class="sxs-lookup"><span data-stu-id="7e633-136">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="7e633-137">示例</span><span class="sxs-lookup"><span data-stu-id="7e633-137">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7e633-138">请求</span><span class="sxs-lookup"><span data-stu-id="7e633-138">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/addGroup
Content-type: application/json
Content-length: 57

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

#### <a name="response"></a><span data-ttu-id="7e633-139">响应</span><span class="sxs-lookup"><span data-stu-id="7e633-139">Response</span></span>
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
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
