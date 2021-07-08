---
title: 'groupLifecyclePolicy: addGroup'
description: 将组添加到生命周期策略。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 07fc0bb3c1d26aedecbc49fd839fe3801c9d6651
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316998"
---
# <a name="grouplifecyclepolicy-addgroup"></a><span data-ttu-id="cd9f1-103">groupLifecyclePolicy: addGroup</span><span class="sxs-lookup"><span data-stu-id="cd9f1-103">groupLifecyclePolicy: addGroup</span></span>

<span data-ttu-id="cd9f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd9f1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd9f1-105">将特定组添加到生命周期策略。</span><span class="sxs-lookup"><span data-stu-id="cd9f1-105">Adds specific groups to a lifecycle policy.</span></span> <span data-ttu-id="cd9f1-106">只有在 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)的 **managedGroupTypes** 属性设置为 时，此操作才将组生命周期策略限制到一组 `Selected` 组。</span><span class="sxs-lookup"><span data-stu-id="cd9f1-106">This action limits the group lifecycle policy to a set of groups only if the **managedGroupTypes** property of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) is set to `Selected`.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd9f1-107">权限</span><span class="sxs-lookup"><span data-stu-id="cd9f1-107">Permissions</span></span>

<span data-ttu-id="cd9f1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cd9f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cd9f1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd9f1-110">Permission type</span></span>      | <span data-ttu-id="cd9f1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cd9f1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd9f1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd9f1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cd9f1-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd9f1-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="cd9f1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd9f1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd9f1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd9f1-115">Not supported.</span></span>    |
|<span data-ttu-id="cd9f1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd9f1-116">Application</span></span> | <span data-ttu-id="cd9f1-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd9f1-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd9f1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd9f1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a><span data-ttu-id="cd9f1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd9f1-119">Request headers</span></span>

| <span data-ttu-id="cd9f1-120">名称</span><span class="sxs-lookup"><span data-stu-id="cd9f1-120">Name</span></span> | <span data-ttu-id="cd9f1-121">说明</span><span class="sxs-lookup"><span data-stu-id="cd9f1-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="cd9f1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd9f1-122">Authorization</span></span> | <span data-ttu-id="cd9f1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cd9f1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cd9f1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd9f1-125">Content-Type</span></span>  | <span data-ttu-id="cd9f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cd9f1-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd9f1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd9f1-127">Request body</span></span>
<span data-ttu-id="cd9f1-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="cd9f1-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cd9f1-129">参数</span><span class="sxs-lookup"><span data-stu-id="cd9f1-129">Parameter</span></span> | <span data-ttu-id="cd9f1-130">类型</span><span class="sxs-lookup"><span data-stu-id="cd9f1-130">Type</span></span> | <span data-ttu-id="cd9f1-131">说明</span><span class="sxs-lookup"><span data-stu-id="cd9f1-131">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cd9f1-132">groupId</span><span class="sxs-lookup"><span data-stu-id="cd9f1-132">groupId</span></span>|<span data-ttu-id="cd9f1-133">String</span><span class="sxs-lookup"><span data-stu-id="cd9f1-133">String</span></span>| <span data-ttu-id="cd9f1-134">要添加到策略的组的标识符。</span><span class="sxs-lookup"><span data-stu-id="cd9f1-134">The identifier of the group to add to the policy.</span></span> |

<span data-ttu-id="cd9f1-135">当 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)的 **managedGroupTypes** 属性设置为 时，您最多可以将 `Selected` 500 个组添加到列表中。</span><span class="sxs-lookup"><span data-stu-id="cd9f1-135">When the **managedGroupTypes** property of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) is set to `Selected`, you can add up to 500 groups to the list.</span></span> <span data-ttu-id="cd9f1-136">如果需要添加 500 多个组 [，groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)的 **managedGroupTypes** 属性必须设置为 `All` 。</span><span class="sxs-lookup"><span data-stu-id="cd9f1-136">If you need to add more than 500 groups, the **managedGroupTypes** property of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) must be set to `All`.</span></span>

<span data-ttu-id="cd9f1-137">每个请求只能添加一个组。</span><span class="sxs-lookup"><span data-stu-id="cd9f1-137">Only one group can be added per request.</span></span>

## <a name="response"></a><span data-ttu-id="cd9f1-138">响应</span><span class="sxs-lookup"><span data-stu-id="cd9f1-138">Response</span></span>

<span data-ttu-id="cd9f1-139">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cd9f1-139">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="cd9f1-140">如果组已添加到策略，响应 `true` 正文中将返回一个值。</span><span class="sxs-lookup"><span data-stu-id="cd9f1-140">If the group is added to the policy, a `true` value is returned in the response body.</span></span> <span data-ttu-id="cd9f1-141">否则， `false` 在响应正文中返回值。</span><span class="sxs-lookup"><span data-stu-id="cd9f1-141">Otherwise, a `false` value is returned in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd9f1-142">示例</span><span class="sxs-lookup"><span data-stu-id="cd9f1-142">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cd9f1-143">请求</span><span class="sxs-lookup"><span data-stu-id="cd9f1-143">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="cd9f1-144">响应</span><span class="sxs-lookup"><span data-stu-id="cd9f1-144">Response</span></span>
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

