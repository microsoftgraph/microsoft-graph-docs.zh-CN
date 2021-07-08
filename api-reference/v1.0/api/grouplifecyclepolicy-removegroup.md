---
title: 'groupLifecyclePolicy: removeGroup'
description: 从生命周期策略中删除组。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3e6ff89d43b92694a912d9f550e578b3c338501d
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317047"
---
# <a name="grouplifecyclepolicy-removegroup"></a><span data-ttu-id="73af1-103">groupLifecyclePolicy: removeGroup</span><span class="sxs-lookup"><span data-stu-id="73af1-103">groupLifecyclePolicy: removeGroup</span></span>

<span data-ttu-id="73af1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73af1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73af1-105">从生命周期策略中删除组。</span><span class="sxs-lookup"><span data-stu-id="73af1-105">Removes a group from a lifecycle policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="73af1-106">权限</span><span class="sxs-lookup"><span data-stu-id="73af1-106">Permissions</span></span>

<span data-ttu-id="73af1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73af1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73af1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="73af1-109">Permission type</span></span>      | <span data-ttu-id="73af1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73af1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73af1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73af1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="73af1-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73af1-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="73af1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73af1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73af1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="73af1-114">Not supported.</span></span>    |
|<span data-ttu-id="73af1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="73af1-115">Application</span></span> | <span data-ttu-id="73af1-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73af1-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73af1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73af1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/removeGroup
```

## <a name="request-headers"></a><span data-ttu-id="73af1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="73af1-118">Request headers</span></span>

| <span data-ttu-id="73af1-119">名称</span><span class="sxs-lookup"><span data-stu-id="73af1-119">Name</span></span> | <span data-ttu-id="73af1-120">说明</span><span class="sxs-lookup"><span data-stu-id="73af1-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="73af1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="73af1-121">Authorization</span></span> | <span data-ttu-id="73af1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73af1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73af1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73af1-124">Content-Type</span></span>  | <span data-ttu-id="73af1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73af1-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="73af1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="73af1-126">Request body</span></span>
<span data-ttu-id="73af1-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="73af1-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="73af1-128">参数</span><span class="sxs-lookup"><span data-stu-id="73af1-128">Parameter</span></span> | <span data-ttu-id="73af1-129">类型</span><span class="sxs-lookup"><span data-stu-id="73af1-129">Type</span></span> | <span data-ttu-id="73af1-130">说明</span><span class="sxs-lookup"><span data-stu-id="73af1-130">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="73af1-131">groupId</span><span class="sxs-lookup"><span data-stu-id="73af1-131">groupId</span></span>|<span data-ttu-id="73af1-132">String</span><span class="sxs-lookup"><span data-stu-id="73af1-132">String</span></span>| <span data-ttu-id="73af1-133">要从策略中删除的组的标识符。</span><span class="sxs-lookup"><span data-stu-id="73af1-133">The identifier of the group to remove from the policy.</span></span>|

## <a name="response"></a><span data-ttu-id="73af1-134">响应</span><span class="sxs-lookup"><span data-stu-id="73af1-134">Response</span></span>

<span data-ttu-id="73af1-135">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="73af1-135">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="73af1-136">如果从策略中删除组，响应 `true` 正文中将返回一个值。</span><span class="sxs-lookup"><span data-stu-id="73af1-136">If the group is removed from the policy, a `true` value is returned in the response body.</span></span> <span data-ttu-id="73af1-137">否则， `false` 在响应正文中返回值。</span><span class="sxs-lookup"><span data-stu-id="73af1-137">Otherwise, a `false` value is returned in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73af1-138">示例</span><span class="sxs-lookup"><span data-stu-id="73af1-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="73af1-139">请求</span><span class="sxs-lookup"><span data-stu-id="73af1-139">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="73af1-140">响应</span><span class="sxs-lookup"><span data-stu-id="73af1-140">Response</span></span>
<!-- { "blockType": "response" } -->

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

