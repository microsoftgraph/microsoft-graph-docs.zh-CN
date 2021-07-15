---
title: managementActionTenantDeploymentStatus： changeDeploymentStatus
description: 更改管理操作租户级别的部署状态。 此信息用于提供对特定状态中的管理操作的见解。 例如，可能有一个计划对管理员应用需要多重身份验证，因此最好将状态更改为计划状态以反映相应的状态。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 572ee7f6c6769ec500c47edee5d35dd18fe75d3f
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440904"
---
# <a name="managementactiontenantdeploymentstatus-changedeploymentstatus"></a><span data-ttu-id="e3436-105">managementActionTenantDeploymentStatus： changeDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="e3436-105">managementActionTenantDeploymentStatus: changeDeploymentStatus</span></span>
<span data-ttu-id="e3436-106">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="e3436-106">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3436-107">更改管理操作租户级别的部署状态。</span><span class="sxs-lookup"><span data-stu-id="e3436-107">Changes the tenant level deployment status for the management action.</span></span> <span data-ttu-id="e3436-108">此信息用于提供对特定状态中的管理操作的见解。</span><span class="sxs-lookup"><span data-stu-id="e3436-108">This information is used to provide insights into what management actions are in a specific state.</span></span> <span data-ttu-id="e3436-109">例如，可能有一个计划对管理员应用需要多重身份验证，因此最好将状态更改为计划状态以反映相应的状态。</span><span class="sxs-lookup"><span data-stu-id="e3436-109">As example there might be a plan to apply the require multi-factor authentication for admins, so it would be ideal to change the status to planned to reflect the appropriate status.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3436-110">权限</span><span class="sxs-lookup"><span data-stu-id="e3436-110">Permissions</span></span>
<span data-ttu-id="e3436-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3436-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3436-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3436-113">Permission type</span></span>|<span data-ttu-id="e3436-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3436-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3436-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3436-115">Delegated (work or school account)</span></span>|<span data-ttu-id="e3436-116">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3436-116">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="e3436-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3436-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3436-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3436-118">Not supported.</span></span>|
|<span data-ttu-id="e3436-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3436-119">Application</span></span>|<span data-ttu-id="e3436-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3436-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3436-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3436-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/changeDeploymentStatus
```

## <a name="request-headers"></a><span data-ttu-id="e3436-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3436-122">Request headers</span></span>
|<span data-ttu-id="e3436-123">名称</span><span class="sxs-lookup"><span data-stu-id="e3436-123">Name</span></span>|<span data-ttu-id="e3436-124">说明</span><span class="sxs-lookup"><span data-stu-id="e3436-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e3436-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3436-125">Authorization</span></span>|<span data-ttu-id="e3436-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e3436-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e3436-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3436-128">Content-Type</span></span>|<span data-ttu-id="e3436-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e3436-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3436-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3436-131">Request body</span></span>
<span data-ttu-id="e3436-132">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3436-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e3436-133">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="e3436-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e3436-134">参数</span><span class="sxs-lookup"><span data-stu-id="e3436-134">Parameter</span></span>|<span data-ttu-id="e3436-135">类型</span><span class="sxs-lookup"><span data-stu-id="e3436-135">Type</span></span>|<span data-ttu-id="e3436-136">说明</span><span class="sxs-lookup"><span data-stu-id="e3436-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3436-137">tenantGroupId</span><span class="sxs-lookup"><span data-stu-id="e3436-137">tenantGroupId</span></span>|<span data-ttu-id="e3436-138">String</span><span class="sxs-lookup"><span data-stu-id="e3436-138">String</span></span>|<span data-ttu-id="e3436-139">租户组的标识符。</span><span class="sxs-lookup"><span data-stu-id="e3436-139">The identifier for the tenant group.</span></span>|
|<span data-ttu-id="e3436-140">tenantId</span><span class="sxs-lookup"><span data-stu-id="e3436-140">tenantId</span></span>|<span data-ttu-id="e3436-141">String</span><span class="sxs-lookup"><span data-stu-id="e3436-141">String</span></span>|<span data-ttu-id="e3436-142">托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。</span><span class="sxs-lookup"><span data-stu-id="e3436-142">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|
|<span data-ttu-id="e3436-143">managementActionId</span><span class="sxs-lookup"><span data-stu-id="e3436-143">managementActionId</span></span>|<span data-ttu-id="e3436-144">String</span><span class="sxs-lookup"><span data-stu-id="e3436-144">String</span></span>|<span data-ttu-id="e3436-145">管理操作 [的标识符](../resources/managedtenants-managementaction.md)。</span><span class="sxs-lookup"><span data-stu-id="e3436-145">The identifier for the [management action](../resources/managedtenants-managementaction.md).</span></span>|
|<span data-ttu-id="e3436-146">managementTemplateId</span><span class="sxs-lookup"><span data-stu-id="e3436-146">managementTemplateId</span></span>|<span data-ttu-id="e3436-147">String</span><span class="sxs-lookup"><span data-stu-id="e3436-147">String</span></span>|<span data-ttu-id="e3436-148">管理模板 [的标识符](../resources/managedtenants-managementtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="e3436-148">The identifier for the [management template](../resources/managedtenants-managementtemplate.md).</span></span>|
|<span data-ttu-id="e3436-149">状态</span><span class="sxs-lookup"><span data-stu-id="e3436-149">status</span></span>|<span data-ttu-id="e3436-150">String</span><span class="sxs-lookup"><span data-stu-id="e3436-150">String</span></span>|<span data-ttu-id="e3436-151">管理操作租户 [部署的新](../resources/managedtenants-managementaction.md) 状态。</span><span class="sxs-lookup"><span data-stu-id="e3436-151">The new status for the [management action](../resources/managedtenants-managementaction.md) tenant deployment.</span></span>|

## <a name="response"></a><span data-ttu-id="e3436-152">响应</span><span class="sxs-lookup"><span data-stu-id="e3436-152">Response</span></span>

<span data-ttu-id="e3436-153">如果成功，此操作在响应正文中返回 响应代码和 `200 OK` [managementActionDeploymentStatus。](../resources/managedtenants-managementactiondeploymentstatus.md)</span><span class="sxs-lookup"><span data-stu-id="e3436-153">If successful, this action returns a `200 OK` response code and a [managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3436-154">示例</span><span class="sxs-lookup"><span data-stu-id="e3436-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e3436-155">请求</span><span class="sxs-lookup"><span data-stu-id="e3436-155">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e3436-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3436-156">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e3436-157">C#</span><span class="sxs-lookup"><span data-stu-id="e3436-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/managementactiontenantdeploymentstatus-changedeploymentstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3436-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3436-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/managementactiontenantdeploymentstatus-changedeploymentstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3436-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3436-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/managementactiontenantdeploymentstatus-changedeploymentstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e3436-160">Java</span><span class="sxs-lookup"><span data-stu-id="e3436-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/managementactiontenantdeploymentstatus-changedeploymentstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e3436-161">响应</span><span class="sxs-lookup"><span data-stu-id="e3436-161">Response</span></span>
><span data-ttu-id="e3436-162">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e3436-162">**Note:** The response object shown here might be shortened for readability.</span></span>
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
