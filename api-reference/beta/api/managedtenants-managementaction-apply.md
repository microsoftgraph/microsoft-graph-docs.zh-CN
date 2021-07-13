---
title: managementAction： apply
description: 对特定托管租户应用管理操作。 通过执行此操作，将进行适当的配置并创建策略。 例如，当对管理员管理操作应用需要多重身份验证时，将创建一个 Azure Active Directory 条件访问策略，该策略要求对分配了管理目录角色的所有用户进行多重身份验证。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: c5ba45154faf95e85a3f7f7878c18a4bb4981d16
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402317"
---
# <a name="managementaction-apply"></a><span data-ttu-id="96dd2-105">managementAction： apply</span><span class="sxs-lookup"><span data-stu-id="96dd2-105">managementAction: apply</span></span>
<span data-ttu-id="96dd2-106">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="96dd2-106">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96dd2-107">对特定托管租户应用管理操作。</span><span class="sxs-lookup"><span data-stu-id="96dd2-107">Applies a management action against a specific managed tenant.</span></span> <span data-ttu-id="96dd2-108">通过执行此操作，将进行适当的配置并创建策略。</span><span class="sxs-lookup"><span data-stu-id="96dd2-108">By performing this operation the appropriate configurations will be made and policies created.</span></span> <span data-ttu-id="96dd2-109">例如，当对管理员管理操作应用需要多重身份验证时，将创建一个 Azure Active Directory 条件访问策略，该策略要求对分配了管理目录角色的所有用户进行多重身份验证。</span><span class="sxs-lookup"><span data-stu-id="96dd2-109">As example when applying the require multi-factor authentication for admins management action will create an Azure Active Directory conditional access policy that requires multi-factor authentication for all users that have been assigned an administrative directory role.</span></span>

## <a name="permissions"></a><span data-ttu-id="96dd2-110">权限</span><span class="sxs-lookup"><span data-stu-id="96dd2-110">Permissions</span></span>
<span data-ttu-id="96dd2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96dd2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96dd2-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="96dd2-113">Permission type</span></span>|<span data-ttu-id="96dd2-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96dd2-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96dd2-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96dd2-115">Delegated (work or school account)</span></span>|<span data-ttu-id="96dd2-116">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96dd2-116">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="96dd2-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96dd2-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96dd2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="96dd2-118">Not supported.</span></span>|
|<span data-ttu-id="96dd2-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="96dd2-119">Application</span></span>|<span data-ttu-id="96dd2-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="96dd2-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96dd2-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96dd2-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/managementActions/{managementActionId}/apply
```

## <a name="request-headers"></a><span data-ttu-id="96dd2-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="96dd2-122">Request headers</span></span>
|<span data-ttu-id="96dd2-123">名称</span><span class="sxs-lookup"><span data-stu-id="96dd2-123">Name</span></span>|<span data-ttu-id="96dd2-124">说明</span><span class="sxs-lookup"><span data-stu-id="96dd2-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="96dd2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="96dd2-125">Authorization</span></span>|<span data-ttu-id="96dd2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96dd2-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="96dd2-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="96dd2-128">Content-Type</span></span>|<span data-ttu-id="96dd2-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="96dd2-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="96dd2-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="96dd2-131">Request body</span></span>
<span data-ttu-id="96dd2-132">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96dd2-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="96dd2-133">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="96dd2-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="96dd2-134">参数</span><span class="sxs-lookup"><span data-stu-id="96dd2-134">Parameter</span></span>|<span data-ttu-id="96dd2-135">类型</span><span class="sxs-lookup"><span data-stu-id="96dd2-135">Type</span></span>|<span data-ttu-id="96dd2-136">说明</span><span class="sxs-lookup"><span data-stu-id="96dd2-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96dd2-137">tenantId</span><span class="sxs-lookup"><span data-stu-id="96dd2-137">tenantId</span></span>|<span data-ttu-id="96dd2-138">String</span><span class="sxs-lookup"><span data-stu-id="96dd2-138">String</span></span>|<span data-ttu-id="96dd2-139">托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。</span><span class="sxs-lookup"><span data-stu-id="96dd2-139">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|
|<span data-ttu-id="96dd2-140">tenantGroupId</span><span class="sxs-lookup"><span data-stu-id="96dd2-140">tenantGroupId</span></span>|<span data-ttu-id="96dd2-141">String</span><span class="sxs-lookup"><span data-stu-id="96dd2-141">String</span></span>|<span data-ttu-id="96dd2-142">租户组的标识符。</span><span class="sxs-lookup"><span data-stu-id="96dd2-142">The identifier of the tenant group.</span></span>|
|<span data-ttu-id="96dd2-143">managementTemplateId</span><span class="sxs-lookup"><span data-stu-id="96dd2-143">managementTemplateId</span></span>|<span data-ttu-id="96dd2-144">String</span><span class="sxs-lookup"><span data-stu-id="96dd2-144">String</span></span>|<span data-ttu-id="96dd2-145">管理模板 [的标识符](../resources/managedtenants-managementtemplate.md)。</span><span class="sxs-lookup"><span data-stu-id="96dd2-145">The identifier of the [management template](../resources/managedtenants-managementtemplate.md).</span></span>|

## <a name="response"></a><span data-ttu-id="96dd2-146">响应</span><span class="sxs-lookup"><span data-stu-id="96dd2-146">Response</span></span>

<span data-ttu-id="96dd2-147">如果成功，此操作在响应正文中返回 响应代码和 `200 OK` [managementActionDeploymentStatus。](../resources/managedtenants-managementactiondeploymentstatus.md)</span><span class="sxs-lookup"><span data-stu-id="96dd2-147">If successful, this action returns a `200 OK` response code and a [managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="96dd2-148">示例</span><span class="sxs-lookup"><span data-stu-id="96dd2-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="96dd2-149">请求</span><span class="sxs-lookup"><span data-stu-id="96dd2-149">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "managementaction_apply"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActions/{managementActionId}/apply
Content-Type: application/json
Content-length: 95

{
  "tenantId": "String",
  "tenantGroupId": "String",
  "managementTemplateId": "String"
}
```

### <a name="response"></a><span data-ttu-id="96dd2-150">响应</span><span class="sxs-lookup"><span data-stu-id="96dd2-150">Response</span></span>
><span data-ttu-id="96dd2-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="96dd2-151">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "managementTemplateId": "e2cadc41-a08f-45e7-8eb1-942d224dfb9a",
  "managementActionId": "b22a4713-8428-4952-8cac-d48962ecbdc9",
  "status": "completed",
  "workloadActionDeploymentStatuses": [
    {
      "actionId": "46b80b42-06c7-45b4-b6fb-aa0aecace87b",
      "status": "completed",
      "deployedPolicyId": null,
      "lastDeploymentDateTime": "2021-07-11T19:35:10.4463799Z",
      "error": null
    }
  ]
}
```
