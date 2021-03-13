---
title: user： activateServicePlan
description: 为给定用户和给定用户 `servicePlanId` `skuId` 激活服务计划。
author: dkershaw10
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: a90dd6cd8cce6b33fb74369e4d42c26c03ffe38a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775042"
---
# <a name="user-activateserviceplan"></a><span data-ttu-id="73d24-103">user： activateServicePlan</span><span class="sxs-lookup"><span data-stu-id="73d24-103">user: activateServicePlan</span></span>

<span data-ttu-id="73d24-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73d24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73d24-105">为给定用户和给定用户 `servicePlanId` `skuId` 激活服务计划。</span><span class="sxs-lookup"><span data-stu-id="73d24-105">Activate a service plan with a given `servicePlanId` and `skuId` for a given user.</span></span>

## <a name="permissions"></a><span data-ttu-id="73d24-106">权限</span><span class="sxs-lookup"><span data-stu-id="73d24-106">Permissions</span></span>

<span data-ttu-id="73d24-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73d24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73d24-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="73d24-109">Permission type</span></span>|<span data-ttu-id="73d24-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="73d24-110">Permissions (from most to least privileged)</span></span>|
| :--- | :--- |
| <span data-ttu-id="73d24-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73d24-111">Delegated (work or school account)</span></span> | <span data-ttu-id="73d24-112">Directory.ReadWrite.All、Directory.ReadWriteAdvanced.All</span><span class="sxs-lookup"><span data-stu-id="73d24-112">Directory.ReadWrite.All, Directory.ReadWriteAdvanced.All</span></span> |
| <span data-ttu-id="73d24-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73d24-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73d24-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="73d24-114">Not Supported.</span></span> |
| <span data-ttu-id="73d24-115">Application</span><span class="sxs-lookup"><span data-stu-id="73d24-115">Application</span></span> | <span data-ttu-id="73d24-116">Directory.ReadWrite.All、Directory.ReadWriteAdvanced.All</span><span class="sxs-lookup"><span data-stu-id="73d24-116">Directory.ReadWrite.All, Directory.ReadWriteAdvanced.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73d24-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73d24-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /users/{id | userPrincipalName}/activateServicePlan
```

## <a name="request-headers"></a><span data-ttu-id="73d24-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="73d24-118">Request headers</span></span>

| <span data-ttu-id="73d24-119">名称</span><span class="sxs-lookup"><span data-stu-id="73d24-119">Name</span></span> | <span data-ttu-id="73d24-120">说明</span><span class="sxs-lookup"><span data-stu-id="73d24-120">Description</span></span> |
| :--- | :--- |
| <span data-ttu-id="73d24-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="73d24-121">Authorization</span></span> | <span data-ttu-id="73d24-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73d24-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73d24-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73d24-124">Content-Type</span></span> | <span data-ttu-id="73d24-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="73d24-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73d24-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="73d24-127">Request body</span></span>

<span data-ttu-id="73d24-128">在请求正文中，提供具有以下参数的 JSON 对象：</span><span class="sxs-lookup"><span data-stu-id="73d24-128">In the request body, provide a JSON object with the following parameter:</span></span>

| <span data-ttu-id="73d24-129">参数</span><span class="sxs-lookup"><span data-stu-id="73d24-129">Parameter</span></span> | <span data-ttu-id="73d24-130">类型</span><span class="sxs-lookup"><span data-stu-id="73d24-130">Type</span></span> | <span data-ttu-id="73d24-131">说明</span><span class="sxs-lookup"><span data-stu-id="73d24-131">Description</span></span> |
| :--- | :--- | :--- |
| <span data-ttu-id="73d24-132">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="73d24-132">servicePlanId</span></span> | <span data-ttu-id="73d24-133">Guid</span><span class="sxs-lookup"><span data-stu-id="73d24-133">Guid</span></span> | <span data-ttu-id="73d24-134">要激活的 ServicePlan 的 PlanId。</span><span class="sxs-lookup"><span data-stu-id="73d24-134">PlanId of the ServicePlan to activate.</span></span> |
| <span data-ttu-id="73d24-135">skuId</span><span class="sxs-lookup"><span data-stu-id="73d24-135">skuId</span></span> | <span data-ttu-id="73d24-136">Guid</span><span class="sxs-lookup"><span data-stu-id="73d24-136">Guid</span></span> | <span data-ttu-id="73d24-137">服务计划已打开的 SKU 的 SkuId。</span><span class="sxs-lookup"><span data-stu-id="73d24-137">SkuId of SKU the service plan is on.</span></span> |

## <a name="response"></a><span data-ttu-id="73d24-138">响应</span><span class="sxs-lookup"><span data-stu-id="73d24-138">Response</span></span>

<span data-ttu-id="73d24-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="73d24-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="73d24-140">示例</span><span class="sxs-lookup"><span data-stu-id="73d24-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73d24-141">请求</span><span class="sxs-lookup"><span data-stu-id="73d24-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="73d24-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="73d24-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_activateserviceplan"
}
-->

``` http
POST https://graph.microsoft.com/beta/me/activateServicePlan
Content-type: application/json
Content-length: 115

{
  "servicePlanId": "28f42d6f-8034-4a0f-9d8a-a218a63b3299",
  "skuId": "465a2a90-5e59-456d-a7b8-127b9fb2e484"
}
```
# <a name="c"></a>[<span data-ttu-id="73d24-143">C#</span><span class="sxs-lookup"><span data-stu-id="73d24-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-activateserviceplan-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73d24-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73d24-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-activateserviceplan-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73d24-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73d24-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-activateserviceplan-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73d24-146">Java</span><span class="sxs-lookup"><span data-stu-id="73d24-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-activateserviceplan-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="73d24-147">响应</span><span class="sxs-lookup"><span data-stu-id="73d24-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
