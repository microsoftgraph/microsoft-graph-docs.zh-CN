---
title: 'groupLifecyclePolicy: addGroup'
description: 将组添加到生命周期策略。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 07ad966a3fbbfd6a44fc5a744366d8e7d754e5be
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446609"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="f4b5d-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="f4b5d-103">groupLifecyclePolicy: addGroup</span></span>

<span data-ttu-id="f4b5d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f4b5d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4b5d-105">将组添加到生命周期策略。</span><span class="sxs-lookup"><span data-stu-id="f4b5d-105">Adds a group to a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4b5d-106">权限</span><span class="sxs-lookup"><span data-stu-id="f4b5d-106">Permissions</span></span>

<span data-ttu-id="f4b5d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4b5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f4b5d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4b5d-109">Permission type</span></span>      | <span data-ttu-id="f4b5d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4b5d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4b5d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4b5d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f4b5d-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4b5d-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="f4b5d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4b5d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4b5d-114">不支持</span><span class="sxs-lookup"><span data-stu-id="f4b5d-114">Not supported</span></span> |
|<span data-ttu-id="f4b5d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4b5d-115">Application</span></span> | <span data-ttu-id="f4b5d-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4b5d-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4b5d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4b5d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="f4b5d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4b5d-118">Request headers</span></span>

| <span data-ttu-id="f4b5d-119">名称</span><span class="sxs-lookup"><span data-stu-id="f4b5d-119">Name</span></span> | <span data-ttu-id="f4b5d-120">说明</span><span class="sxs-lookup"><span data-stu-id="f4b5d-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="f4b5d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4b5d-121">Authorization</span></span> | <span data-ttu-id="f4b5d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f4b5d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f4b5d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f4b5d-124">Content-Type</span></span>  | <span data-ttu-id="f4b5d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4b5d-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4b5d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4b5d-126">Request body</span></span>
<span data-ttu-id="f4b5d-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="f4b5d-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f4b5d-128">参数</span><span class="sxs-lookup"><span data-stu-id="f4b5d-128">Parameter</span></span> | <span data-ttu-id="f4b5d-129">类型</span><span class="sxs-lookup"><span data-stu-id="f4b5d-129">Type</span></span> | <span data-ttu-id="f4b5d-130">说明</span><span class="sxs-lookup"><span data-stu-id="f4b5d-130">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f4b5d-131">groupId</span><span class="sxs-lookup"><span data-stu-id="f4b5d-131">groupId</span></span>|<span data-ttu-id="f4b5d-132">Guid</span><span class="sxs-lookup"><span data-stu-id="f4b5d-132">Guid</span></span>| <span data-ttu-id="f4b5d-133">要添加到策略的组的 ID。</span><span class="sxs-lookup"><span data-stu-id="f4b5d-133">The id of the group to add to the policy.</span></span> |

## <a name="response"></a><span data-ttu-id="f4b5d-134">响应</span><span class="sxs-lookup"><span data-stu-id="f4b5d-134">Response</span></span>

<span data-ttu-id="f4b5d-135">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f4b5d-135">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="f4b5d-136">如果组已添加到策略，便会在响应正文中返回 **true** 值。</span><span class="sxs-lookup"><span data-stu-id="f4b5d-136">If the group is added to the policy, a **true** value is returned in the response body.</span></span> <span data-ttu-id="f4b5d-137">否则，响应正文中返回 **false** 值。</span><span class="sxs-lookup"><span data-stu-id="f4b5d-137">Otherwise, a **false** value is returned in the reponse body.</span></span>

## <a name="example"></a><span data-ttu-id="f4b5d-138">示例</span><span class="sxs-lookup"><span data-stu-id="f4b5d-138">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f4b5d-139">请求</span><span class="sxs-lookup"><span data-stu-id="f4b5d-139">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="f4b5d-140">响应</span><span class="sxs-lookup"><span data-stu-id="f4b5d-140">Response</span></span>
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
  "suppressions": []
}
-->
