---
title: 'groupLifecyclePolicy: removeGroup'
description: 从生命周期策略中删除组。
author: dkershaw10
ms.openlocfilehash: f1fcd8aedc74353d2224b7a670c40b43deb4cd16
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362655"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="cee91-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="cee91-103">groupLifecyclePolicy: removeGroup</span></span>

> <span data-ttu-id="cee91-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cee91-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cee91-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cee91-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cee91-106">从生命周期策略中删除组。</span><span class="sxs-lookup"><span data-stu-id="cee91-106">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="cee91-107">权限</span><span class="sxs-lookup"><span data-stu-id="cee91-107">Permissions</span></span>

<span data-ttu-id="cee91-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cee91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cee91-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cee91-110">Permission type</span></span>      | <span data-ttu-id="cee91-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cee91-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cee91-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cee91-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cee91-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cee91-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="cee91-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cee91-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cee91-115">不支持</span><span class="sxs-lookup"><span data-stu-id="cee91-115">Not supported</span></span> |
|<span data-ttu-id="cee91-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cee91-116">Application</span></span> |  <span data-ttu-id="cee91-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cee91-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cee91-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cee91-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="cee91-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cee91-119">Request headers</span></span>

| <span data-ttu-id="cee91-120">Name</span><span class="sxs-lookup"><span data-stu-id="cee91-120">Name</span></span> | <span data-ttu-id="cee91-121">说明</span><span class="sxs-lookup"><span data-stu-id="cee91-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="cee91-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cee91-122">Authorization</span></span> | <span data-ttu-id="cee91-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cee91-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cee91-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cee91-125">Content-Type</span></span>  | <span data-ttu-id="cee91-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cee91-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cee91-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cee91-127">Request body</span></span>
<span data-ttu-id="cee91-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="cee91-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cee91-129">参数</span><span class="sxs-lookup"><span data-stu-id="cee91-129">Parameter</span></span> | <span data-ttu-id="cee91-130">Type</span><span class="sxs-lookup"><span data-stu-id="cee91-130">Type</span></span> | <span data-ttu-id="cee91-131">说明</span><span class="sxs-lookup"><span data-stu-id="cee91-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cee91-132">groupId</span><span class="sxs-lookup"><span data-stu-id="cee91-132">groupId</span></span>|<span data-ttu-id="cee91-133">Guid</span><span class="sxs-lookup"><span data-stu-id="cee91-133">Guid</span></span>| <span data-ttu-id="cee91-134">要从策略中删除的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="cee91-134">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="cee91-135">响应</span><span class="sxs-lookup"><span data-stu-id="cee91-135">Response</span></span>

<span data-ttu-id="cee91-136">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cee91-136">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="cee91-137">如果已从策略中删除组，响应正文中返回 **true** 值。</span><span class="sxs-lookup"><span data-stu-id="cee91-137">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="cee91-138">否则，响应正文中返回 **false** 值。</span><span class="sxs-lookup"><span data-stu-id="cee91-138">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="cee91-139">示例</span><span class="sxs-lookup"><span data-stu-id="cee91-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cee91-140">请求</span><span class="sxs-lookup"><span data-stu-id="cee91-140">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="cee91-141">响应</span><span class="sxs-lookup"><span data-stu-id="cee91-141">Response</span></span>
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