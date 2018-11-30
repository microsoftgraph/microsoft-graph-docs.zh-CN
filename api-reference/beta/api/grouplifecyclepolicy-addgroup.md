---
title: 'groupLifecyclePolicy: addGroup'
description: 将组添加到生命周期策略。
ms.openlocfilehash: 59f49429f65112488f42727cdbb46fc0a4b87800
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046612"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="6c8f6-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="6c8f6-103">groupLifecyclePolicy: addGroup</span></span>

> <span data-ttu-id="6c8f6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6c8f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c8f6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6c8f6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c8f6-106">将组添加到生命周期策略。</span><span class="sxs-lookup"><span data-stu-id="6c8f6-106">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c8f6-107">权限</span><span class="sxs-lookup"><span data-stu-id="6c8f6-107">Permissions</span></span>

<span data-ttu-id="6c8f6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c8f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6c8f6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c8f6-110">Permission type</span></span>      | <span data-ttu-id="6c8f6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6c8f6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c8f6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c8f6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6c8f6-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c8f6-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="6c8f6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c8f6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c8f6-115">不支持</span><span class="sxs-lookup"><span data-stu-id="6c8f6-115">Not supported</span></span> |
|<span data-ttu-id="6c8f6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c8f6-116">Application</span></span> | <span data-ttu-id="6c8f6-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c8f6-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c8f6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c8f6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="6c8f6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c8f6-119">Request headers</span></span>

| <span data-ttu-id="6c8f6-120">名称</span><span class="sxs-lookup"><span data-stu-id="6c8f6-120">Name</span></span> | <span data-ttu-id="6c8f6-121">说明</span><span class="sxs-lookup"><span data-stu-id="6c8f6-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="6c8f6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c8f6-122">Authorization</span></span> | <span data-ttu-id="6c8f6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6c8f6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6c8f6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c8f6-125">Content-Type</span></span>  | <span data-ttu-id="6c8f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c8f6-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c8f6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c8f6-127">Request body</span></span>
<span data-ttu-id="6c8f6-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6c8f6-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6c8f6-129">参数</span><span class="sxs-lookup"><span data-stu-id="6c8f6-129">Parameter</span></span> | <span data-ttu-id="6c8f6-130">类型</span><span class="sxs-lookup"><span data-stu-id="6c8f6-130">Type</span></span> | <span data-ttu-id="6c8f6-131">说明</span><span class="sxs-lookup"><span data-stu-id="6c8f6-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6c8f6-132">groupId</span><span class="sxs-lookup"><span data-stu-id="6c8f6-132">groupId</span></span>|<span data-ttu-id="6c8f6-133">Guid</span><span class="sxs-lookup"><span data-stu-id="6c8f6-133">Guid</span></span>| <span data-ttu-id="6c8f6-134">要添加到策略的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="6c8f6-134">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="6c8f6-135">响应</span><span class="sxs-lookup"><span data-stu-id="6c8f6-135">Response</span></span>

<span data-ttu-id="6c8f6-136">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6c8f6-136">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="6c8f6-137">如果组已添加到策略，便会在响应正文中返回 **true** 值。</span><span class="sxs-lookup"><span data-stu-id="6c8f6-137">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="6c8f6-138">否则，响应正文中返回 **false** 值。</span><span class="sxs-lookup"><span data-stu-id="6c8f6-138">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="6c8f6-139">示例</span><span class="sxs-lookup"><span data-stu-id="6c8f6-139">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6c8f6-140">请求</span><span class="sxs-lookup"><span data-stu-id="6c8f6-140">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="6c8f6-141">响应</span><span class="sxs-lookup"><span data-stu-id="6c8f6-141">Response</span></span>
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