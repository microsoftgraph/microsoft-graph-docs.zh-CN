---
title: user： activateServicePlan
description: 为给定用户和给定用户 `servicePlanId` `skuId` 激活服务计划。
author: dkershaw10
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 70849865237a82f4a0bb5fcee22263291627c21d
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578858"
---
# <a name="user-activateserviceplan"></a><span data-ttu-id="ccc01-103">user： activateServicePlan</span><span class="sxs-lookup"><span data-stu-id="ccc01-103">user: activateServicePlan</span></span>

<span data-ttu-id="ccc01-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ccc01-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccc01-105">为给定用户和给定用户 `servicePlanId` `skuId` 激活服务计划。</span><span class="sxs-lookup"><span data-stu-id="ccc01-105">Activate a service plan with a given `servicePlanId` and `skuId` for a given user.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccc01-106">权限</span><span class="sxs-lookup"><span data-stu-id="ccc01-106">Permissions</span></span>

<span data-ttu-id="ccc01-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ccc01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccc01-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ccc01-109">Permission type</span></span>|<span data-ttu-id="ccc01-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ccc01-110">Permissions (from most to least privileged)</span></span>|
| :--- | :--- |
| <span data-ttu-id="ccc01-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ccc01-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ccc01-112">Directory.ReadWrite.All、Directory.ReadWriteAdvanced.All</span><span class="sxs-lookup"><span data-stu-id="ccc01-112">Directory.ReadWrite.All, Directory.ReadWriteAdvanced.All</span></span> |
| <span data-ttu-id="ccc01-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ccc01-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccc01-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccc01-114">Not Supported.</span></span> |
| <span data-ttu-id="ccc01-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ccc01-115">Application</span></span> | <span data-ttu-id="ccc01-116">Directory.ReadWrite.All、Directory.ReadWriteAdvanced.All</span><span class="sxs-lookup"><span data-stu-id="ccc01-116">Directory.ReadWrite.All, Directory.ReadWriteAdvanced.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccc01-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ccc01-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /users/{id | userPrincipalName}/activateServicePlan
```

## <a name="request-headers"></a><span data-ttu-id="ccc01-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ccc01-118">Request headers</span></span>

| <span data-ttu-id="ccc01-119">名称</span><span class="sxs-lookup"><span data-stu-id="ccc01-119">Name</span></span> | <span data-ttu-id="ccc01-120">说明</span><span class="sxs-lookup"><span data-stu-id="ccc01-120">Description</span></span> |
| :--- | :--- |
| <span data-ttu-id="ccc01-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccc01-121">Authorization</span></span> | <span data-ttu-id="ccc01-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ccc01-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ccc01-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ccc01-124">Content-Type</span></span> | <span data-ttu-id="ccc01-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ccc01-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ccc01-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ccc01-127">Request body</span></span>

<span data-ttu-id="ccc01-128">在请求正文中，提供具有以下参数的 JSON 对象：</span><span class="sxs-lookup"><span data-stu-id="ccc01-128">In the request body, provide a JSON object with the following parameter:</span></span>

| <span data-ttu-id="ccc01-129">参数</span><span class="sxs-lookup"><span data-stu-id="ccc01-129">Parameter</span></span> | <span data-ttu-id="ccc01-130">类型</span><span class="sxs-lookup"><span data-stu-id="ccc01-130">Type</span></span> | <span data-ttu-id="ccc01-131">说明</span><span class="sxs-lookup"><span data-stu-id="ccc01-131">Description</span></span> |
| :--- | :--- | :--- |
| <span data-ttu-id="ccc01-132">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="ccc01-132">servicePlanId</span></span> | <span data-ttu-id="ccc01-133">Guid</span><span class="sxs-lookup"><span data-stu-id="ccc01-133">Guid</span></span> | <span data-ttu-id="ccc01-134">要激活的 ServicePlan 的 PlanId。</span><span class="sxs-lookup"><span data-stu-id="ccc01-134">PlanId of the ServicePlan to activate.</span></span> |
| <span data-ttu-id="ccc01-135">skuId</span><span class="sxs-lookup"><span data-stu-id="ccc01-135">skuId</span></span> | <span data-ttu-id="ccc01-136">Guid</span><span class="sxs-lookup"><span data-stu-id="ccc01-136">Guid</span></span> | <span data-ttu-id="ccc01-137">服务计划已打开的 SKU 的 SkuId。</span><span class="sxs-lookup"><span data-stu-id="ccc01-137">SkuId of SKU the service plan is on.</span></span> |

## <a name="response"></a><span data-ttu-id="ccc01-138">响应</span><span class="sxs-lookup"><span data-stu-id="ccc01-138">Response</span></span>

<span data-ttu-id="ccc01-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ccc01-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ccc01-140">示例</span><span class="sxs-lookup"><span data-stu-id="ccc01-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ccc01-141">请求</span><span class="sxs-lookup"><span data-stu-id="ccc01-141">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="ccc01-142">响应</span><span class="sxs-lookup"><span data-stu-id="ccc01-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
