---
title: managementActionTenantDeploymentStatus： changeDeploymentStatus
description: 更改管理操作租户级别的部署状态。 此信息用于提供对特定状态中的管理操作的见解。 例如，可能有一个计划对管理员应用需要多重身份验证，因此最好将状态更改为计划状态以反映相应的状态。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 4d8c5acacee4eb31e8d014820466eae69534232f
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402313"
---
# <a name="managementactiontenantdeploymentstatus-changedeploymentstatus"></a><span data-ttu-id="c53df-105">managementActionTenantDeploymentStatus： changeDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="c53df-105">managementActionTenantDeploymentStatus: changeDeploymentStatus</span></span>
<span data-ttu-id="c53df-106">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="c53df-106">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c53df-107">更改管理操作租户级别的部署状态。</span><span class="sxs-lookup"><span data-stu-id="c53df-107">Changes the tenant level deployment status for the management action.</span></span> <span data-ttu-id="c53df-108">此信息用于提供对特定状态中的管理操作的见解。</span><span class="sxs-lookup"><span data-stu-id="c53df-108">This information is used to provide insights into what management actions are in a specific state.</span></span> <span data-ttu-id="c53df-109">例如，可能有一个计划对管理员应用需要多重身份验证，因此最好将状态更改为计划状态以反映相应的状态。</span><span class="sxs-lookup"><span data-stu-id="c53df-109">As example there might be a plan to apply the require multi-factor authentication for admins, so it would be ideal to change the status to planned to reflect the appropriate status.</span></span>

## <a name="permissions"></a><span data-ttu-id="c53df-110">权限</span><span class="sxs-lookup"><span data-stu-id="c53df-110">Permissions</span></span>
<span data-ttu-id="c53df-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c53df-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c53df-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c53df-113">Permission type</span></span>|<span data-ttu-id="c53df-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c53df-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c53df-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c53df-115">Delegated (work or school account)</span></span>|<span data-ttu-id="c53df-116">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c53df-116">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="c53df-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c53df-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c53df-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c53df-118">Not supported.</span></span>|
|<span data-ttu-id="c53df-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="c53df-119">Application</span></span>|<span data-ttu-id="c53df-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="c53df-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c53df-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c53df-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/changeDeploymentStatus
```

## <a name="request-headers"></a><span data-ttu-id="c53df-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c53df-122">Request headers</span></span>
|<span data-ttu-id="c53df-123">名称</span><span class="sxs-lookup"><span data-stu-id="c53df-123">Name</span></span>|<span data-ttu-id="c53df-124">说明</span><span class="sxs-lookup"><span data-stu-id="c53df-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c53df-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c53df-125">Authorization</span></span>|<span data-ttu-id="c53df-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c53df-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c53df-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c53df-128">Content-Type</span></span>|<span data-ttu-id="c53df-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c53df-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c53df-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c53df-131">Request body</span></span>
<span data-ttu-id="c53df-132">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c53df-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c53df-133">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="c53df-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c53df-134">参数</span><span class="sxs-lookup"><span data-stu-id="c53df-134">Parameter</span></span>|<span data-ttu-id="c53df-135">类型</span><span class="sxs-lookup"><span data-stu-id="c53df-135">Type</span></span>|<span data-ttu-id="c53df-136">说明</span><span class="sxs-lookup"><span data-stu-id="c53df-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c53df-137">tenantGroupId</span><span class="sxs-lookup"><span data-stu-id="c53df-137">tenantGroupId</span></span>|<span data-ttu-id="c53df-138">String</span><span class="sxs-lookup"><span data-stu-id="c53df-138">String</span></span>|<span data-ttu-id="c53df-139">租户组的标识符。</span><span class="sxs-lookup"><span data-stu-id="c53df-139">The identifier for the tenant group.</span></span>|
|<span data-ttu-id="c53df-140">tenantId</span><span class="sxs-lookup"><span data-stu-id="c53df-140">tenantId</span></span>|<span data-ttu-id="c53df-141">String</span><span class="sxs-lookup"><span data-stu-id="c53df-141">String</span></span>|<span data-ttu-id="c53df-142">托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。</span><span class="sxs-lookup"><span data-stu-id="c53df-142">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|
|<span data-ttu-id="c53df-143">managementActionId</span><span class="sxs-lookup"><span data-stu-id="c53df-143">managementActionId</span></span>|<span data-ttu-id="c53df-144">String</span><span class="sxs-lookup"><span data-stu-id="c53df-144">String</span></span>|<span data-ttu-id="c53df-145">管理操作 [的标识符](../resources/managedtenants-managementaction.md)。</span><span class="sxs-lookup"><span data-stu-id="c53df-145">The identifier for the [management action](../resources/managedtenants-managementaction.md).</span></span>|
|<span data-ttu-id="c53df-146">managementTemplateId</span><span class="sxs-lookup"><span data-stu-id="c53df-146">managementTemplateId</span></span>|<span data-ttu-id="c53df-147">String</span><span class="sxs-lookup"><span data-stu-id="c53df-147">String</span></span>|<span data-ttu-id="c53df-148">管理模板 [的标识符](../resources/managedtenants-managementtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="c53df-148">The identifier for the [management template](../resources/managedtenants-managementtemplate.md).</span></span>|
|<span data-ttu-id="c53df-149">状态</span><span class="sxs-lookup"><span data-stu-id="c53df-149">status</span></span>|<span data-ttu-id="c53df-150">String</span><span class="sxs-lookup"><span data-stu-id="c53df-150">String</span></span>|<span data-ttu-id="c53df-151">管理操作租户 [部署的新](../resources/managedtenants-managementaction.md) 状态。</span><span class="sxs-lookup"><span data-stu-id="c53df-151">The new status for the [management action](../resources/managedtenants-managementaction.md) tenant deployment.</span></span>|

## <a name="response"></a><span data-ttu-id="c53df-152">响应</span><span class="sxs-lookup"><span data-stu-id="c53df-152">Response</span></span>

<span data-ttu-id="c53df-153">如果成功，此操作在响应正文中返回 响应代码和 `200 OK` [managementActionDeploymentStatus。](../resources/managedtenants-managementactiondeploymentstatus.md)</span><span class="sxs-lookup"><span data-stu-id="c53df-153">If successful, this action returns a `200 OK` response code and a [managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c53df-154">示例</span><span class="sxs-lookup"><span data-stu-id="c53df-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c53df-155">请求</span><span class="sxs-lookup"><span data-stu-id="c53df-155">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "managementactiontenantdeploymentstatus_changedeploymentstatus"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/changeDeploymentStatus
Content-Type: application/json
Content-length: 153

{
  "tenantGroupId": "String",
  "tenantId": "String",
  "managementActionId": "String",
  "managementTemplateId": "String",
  "status": "String"
}
```

### <a name="response"></a><span data-ttu-id="c53df-156">响应</span><span class="sxs-lookup"><span data-stu-id="c53df-156">Response</span></span>
><span data-ttu-id="c53df-157">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c53df-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.managedTenants.ManagementActionDeploymentStatus",
  "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
  "managementActionId": "e96a8cdb-0435-4808-9956-cf6b8ae77aa6",
  "status": "planned",
  "workloadActionDeploymentStatuses": []
}
```
