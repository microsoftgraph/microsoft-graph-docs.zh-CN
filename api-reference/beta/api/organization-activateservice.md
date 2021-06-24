---
title: organization： activateService
description: 为组织激活服务。
author: dkershaw10
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6008b7f5a597af5ac65b349af22879b9db1255f4
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109160"
---
# <a name="organization-activateservice"></a><span data-ttu-id="75359-103">organization： activateService</span><span class="sxs-lookup"><span data-stu-id="75359-103">organization: activateService</span></span>

<span data-ttu-id="75359-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75359-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75359-105">为组织激活服务。</span><span class="sxs-lookup"><span data-stu-id="75359-105">Activate a service for an organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="75359-106">权限</span><span class="sxs-lookup"><span data-stu-id="75359-106">Permissions</span></span>
<span data-ttu-id="75359-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75359-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="75359-109">若要为组织激活服务，请求者需要具有以下权限的公司管理员角色。 </span><span class="sxs-lookup"><span data-stu-id="75359-109">In order to activate a service for an organization the requestor needs to have the _Company Administrator_ role with the following permissions.</span></span>

|<span data-ttu-id="75359-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="75359-110">Permission type</span></span>|<span data-ttu-id="75359-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="75359-111">Permissions (from least to most privileged)</span></span>|
| :--- | :--- |
| <span data-ttu-id="75359-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75359-112">Delegated (work or school account)</span></span> | <span data-ttu-id="75359-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75359-113">Directory.ReadWrite.All</span></span>|
| <span data-ttu-id="75359-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75359-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75359-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="75359-115">Not Supported.</span></span> |
| <span data-ttu-id="75359-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="75359-116">Application</span></span> | <span data-ttu-id="75359-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75359-117">Directory.ReadWrite.All</span></span>|


## <a name="http-request"></a><span data-ttu-id="75359-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75359-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/activateService
```

## <a name="request-headers"></a><span data-ttu-id="75359-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="75359-119">Request headers</span></span>
|<span data-ttu-id="75359-120">名称</span><span class="sxs-lookup"><span data-stu-id="75359-120">Name</span></span>|<span data-ttu-id="75359-121">说明</span><span class="sxs-lookup"><span data-stu-id="75359-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="75359-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="75359-122">Authorization</span></span>|<span data-ttu-id="75359-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="75359-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="75359-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="75359-125">Content-Type</span></span>|<span data-ttu-id="75359-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="75359-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75359-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="75359-128">Request body</span></span>
<span data-ttu-id="75359-129">在请求正文中，提供 [activateService](../resources/activateService.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75359-129">In the request body, supply a JSON representation of the [activateService](../resources/activateService.md) object.</span></span>
<span data-ttu-id="75359-130">必须定义 **service 或 (** **servicePlanId** _和_ **skuId**) 此操作有效。</span><span class="sxs-lookup"><span data-stu-id="75359-130">You must define **service** or (**servicePlanId** _and_ **skuId**) for this action to be valid.</span></span>

| <span data-ttu-id="75359-131">属性</span><span class="sxs-lookup"><span data-stu-id="75359-131">Property</span></span>         | <span data-ttu-id="75359-132">类型</span><span class="sxs-lookup"><span data-stu-id="75359-132">Type</span></span>         | <span data-ttu-id="75359-133">说明</span><span class="sxs-lookup"><span data-stu-id="75359-133">Description</span></span>                           |
| ----------------- | ------------ | ------------------------------------- |
| <span data-ttu-id="75359-134">service</span><span class="sxs-lookup"><span data-stu-id="75359-134">service</span></span>| <span data-ttu-id="75359-135">String</span><span class="sxs-lookup"><span data-stu-id="75359-135">String</span></span> | <span data-ttu-id="75359-136">要激活的服务的名称。</span><span class="sxs-lookup"><span data-stu-id="75359-136">The name of the service to activate.</span></span> |
| <span data-ttu-id="75359-137">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="75359-137">servicePlanId</span></span> | <span data-ttu-id="75359-138">Guid</span><span class="sxs-lookup"><span data-stu-id="75359-138">Guid</span></span> | <span data-ttu-id="75359-139">要激活的服务计划的计划标识符。</span><span class="sxs-lookup"><span data-stu-id="75359-139">The plan identifier of the service plan to activate.</span></span> |
| <span data-ttu-id="75359-140">skuId</span><span class="sxs-lookup"><span data-stu-id="75359-140">skuId</span></span> | <span data-ttu-id="75359-141">Guid</span><span class="sxs-lookup"><span data-stu-id="75359-141">Guid</span></span> | <span data-ttu-id="75359-142">服务计划的 SKU 标识符。</span><span class="sxs-lookup"><span data-stu-id="75359-142">The SKU identifier of the service plan.</span></span> |

## <a name="response"></a><span data-ttu-id="75359-143">响应</span><span class="sxs-lookup"><span data-stu-id="75359-143">Response</span></span>

<span data-ttu-id="75359-144">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="75359-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="75359-145">示例</span><span class="sxs-lookup"><span data-stu-id="75359-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="75359-146">请求</span><span class="sxs-lookup"><span data-stu-id="75359-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "organization_activateservice"
}
-->
``` http
POST https://graph.microsoft.com/beta/organization/{:organizationId}/activateService
Content-Type: application/json

{
    "skuId": "6fd2c87f-b296-42f0-b197-1e91e994b900",
    "servicePlanId": "a23b959c-7ce8-4e57-9140-b90eb88a9e97"
}
```

### <a name="response"></a><span data-ttu-id="75359-147">响应</span><span class="sxs-lookup"><span data-stu-id="75359-147">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```