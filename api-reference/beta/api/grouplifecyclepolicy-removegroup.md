---
title: 'groupLifecyclePolicy: removeGroup'
description: 从生命周期策略中删除组。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8043119b2480f0116566d668b440e4d493ebbeb5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953309"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="18f97-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="18f97-103">groupLifecyclePolicy: removeGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18f97-104">从生命周期策略中删除组。</span><span class="sxs-lookup"><span data-stu-id="18f97-104">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="18f97-105">权限</span><span class="sxs-lookup"><span data-stu-id="18f97-105">Permissions</span></span>

<span data-ttu-id="18f97-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18f97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="18f97-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="18f97-108">Permission type</span></span>      | <span data-ttu-id="18f97-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18f97-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18f97-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18f97-110">Delegated (work or school account)</span></span> | <span data-ttu-id="18f97-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18f97-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="18f97-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18f97-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18f97-113">不支持</span><span class="sxs-lookup"><span data-stu-id="18f97-113">Not supported</span></span> |
|<span data-ttu-id="18f97-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="18f97-114">Application</span></span> |  <span data-ttu-id="18f97-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18f97-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18f97-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18f97-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="18f97-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="18f97-117">Request headers</span></span>

| <span data-ttu-id="18f97-118">名称</span><span class="sxs-lookup"><span data-stu-id="18f97-118">Name</span></span> | <span data-ttu-id="18f97-119">说明</span><span class="sxs-lookup"><span data-stu-id="18f97-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="18f97-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="18f97-120">Authorization</span></span> | <span data-ttu-id="18f97-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="18f97-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18f97-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18f97-123">Content-Type</span></span>  | <span data-ttu-id="18f97-124">application/json</span><span class="sxs-lookup"><span data-stu-id="18f97-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="18f97-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="18f97-125">Request body</span></span>
<span data-ttu-id="18f97-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="18f97-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="18f97-127">参数</span><span class="sxs-lookup"><span data-stu-id="18f97-127">Parameter</span></span> | <span data-ttu-id="18f97-128">类型</span><span class="sxs-lookup"><span data-stu-id="18f97-128">Type</span></span> | <span data-ttu-id="18f97-129">说明</span><span class="sxs-lookup"><span data-stu-id="18f97-129">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="18f97-130">groupId</span><span class="sxs-lookup"><span data-stu-id="18f97-130">groupId</span></span>|<span data-ttu-id="18f97-131">Guid</span><span class="sxs-lookup"><span data-stu-id="18f97-131">Guid</span></span>| <span data-ttu-id="18f97-132">要从策略中删除的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="18f97-132">The id of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="18f97-133">响应</span><span class="sxs-lookup"><span data-stu-id="18f97-133">Response</span></span>

<span data-ttu-id="18f97-134">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="18f97-134">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="18f97-135">如果已从策略中删除组，响应正文中返回 **true** 值。</span><span class="sxs-lookup"><span data-stu-id="18f97-135">If the group is removed from the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="18f97-136">否则，响应正文中返回 **false** 值。</span><span class="sxs-lookup"><span data-stu-id="18f97-136">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="18f97-137">示例</span><span class="sxs-lookup"><span data-stu-id="18f97-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="18f97-138">请求</span><span class="sxs-lookup"><span data-stu-id="18f97-138">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="18f97-139">响应</span><span class="sxs-lookup"><span data-stu-id="18f97-139">Response</span></span>
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
