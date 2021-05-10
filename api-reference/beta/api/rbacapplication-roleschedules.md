---
title: rbacApplication：roleSchedules
description: 检索 roleAssignmentSchedules 和 roleEligibilitySchedules。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bb226f2b8e116b57e8514b642ecd46d0b4c9bde4
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299165"
---
# <a name="rbacapplication-roleschedules"></a><span data-ttu-id="c4621-103">rbacApplication：roleSchedules</span><span class="sxs-lookup"><span data-stu-id="c4621-103">rbacApplication: roleSchedules</span></span>
<span data-ttu-id="c4621-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4621-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4621-105">检索 roleAssignmentSchedules 和 roleEligibilitySchedules。</span><span class="sxs-lookup"><span data-stu-id="c4621-105">Retrieve both roleAssignmentSchedules and roleEligibilitySchedules.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4621-106">权限</span><span class="sxs-lookup"><span data-stu-id="c4621-106">Permissions</span></span>
<span data-ttu-id="c4621-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4621-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4621-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4621-109">Permission type</span></span>|<span data-ttu-id="c4621-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4621-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4621-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4621-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c4621-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="c4621-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="c4621-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4621-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4621-114">不支持</span><span class="sxs-lookup"><span data-stu-id="c4621-114">Not supported</span></span>|
|<span data-ttu-id="c4621-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4621-115">Application</span></span>|<span data-ttu-id="c4621-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="c4621-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4621-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4621-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleSchedules
```

## <a name="function-parameters"></a><span data-ttu-id="c4621-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="c4621-118">Function parameters</span></span>
<span data-ttu-id="c4621-119">下表显示了可用于此方法的查询参数。</span><span class="sxs-lookup"><span data-stu-id="c4621-119">The following table shows the query parameters that can be used with this method.</span></span>

|<span data-ttu-id="c4621-120">参数</span><span class="sxs-lookup"><span data-stu-id="c4621-120">Parameter</span></span>|<span data-ttu-id="c4621-121">类型</span><span class="sxs-lookup"><span data-stu-id="c4621-121">Type</span></span>|<span data-ttu-id="c4621-122">说明</span><span class="sxs-lookup"><span data-stu-id="c4621-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4621-123">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="c4621-123">directoryScopeId</span></span>|<span data-ttu-id="c4621-124">String</span><span class="sxs-lookup"><span data-stu-id="c4621-124">String</span></span>|<span data-ttu-id="c4621-125">表示工作分配范围的目录对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="c4621-125">Id of the directory object that represents the scope of the assignment.</span></span> <span data-ttu-id="c4621-126">工作分配的范围决定了已授予主体访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="c4621-126">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="c4621-127">目录作用域是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="c4621-127">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="c4621-128">应用程序作用域是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="c4621-128">App scopes are scopes that are defined and understood by this application only.</span></span> |
|<span data-ttu-id="c4621-129">appScopeId</span><span class="sxs-lookup"><span data-stu-id="c4621-129">appScopeId</span></span>|<span data-ttu-id="c4621-130">String</span><span class="sxs-lookup"><span data-stu-id="c4621-130">String</span></span>|<span data-ttu-id="c4621-131">特定于应用的范围的 ID。</span><span class="sxs-lookup"><span data-stu-id="c4621-131">Id of the app specific scope.</span></span> <span data-ttu-id="c4621-132">工作分配的范围决定了已授予主体访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="c4621-132">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="c4621-133">目录作用域是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="c4621-133">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="c4621-134">对租户范围范围使用"/"。</span><span class="sxs-lookup"><span data-stu-id="c4621-134">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="c4621-135">应用程序作用域是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="c4621-135">App scopes are scopes that are defined and understood by this application only.</span></span> |
|<span data-ttu-id="c4621-136">principalId</span><span class="sxs-lookup"><span data-stu-id="c4621-136">principalId</span></span>|<span data-ttu-id="c4621-137">String</span><span class="sxs-lookup"><span data-stu-id="c4621-137">String</span></span>|<span data-ttu-id="c4621-138">计划所属的主体的 Objectid。</span><span class="sxs-lookup"><span data-stu-id="c4621-138">Objectid of the principal to which the schedules belong.</span></span> |
|<span data-ttu-id="c4621-139">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c4621-139">roleDefinitionId</span></span>|<span data-ttu-id="c4621-140">String</span><span class="sxs-lookup"><span data-stu-id="c4621-140">String</span></span>|<span data-ttu-id="c4621-141">工作分配的 unifiedRoleDefinition 的 ID。</span><span class="sxs-lookup"><span data-stu-id="c4621-141">ID of the unifiedRoleDefinition for the assignment.</span></span> <span data-ttu-id="c4621-142">只读。</span><span class="sxs-lookup"><span data-stu-id="c4621-142">Read only.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="c4621-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4621-143">Request headers</span></span>
|<span data-ttu-id="c4621-144">名称</span><span class="sxs-lookup"><span data-stu-id="c4621-144">Name</span></span>|<span data-ttu-id="c4621-145">说明</span><span class="sxs-lookup"><span data-stu-id="c4621-145">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c4621-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4621-146">Authorization</span></span>|<span data-ttu-id="c4621-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4621-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4621-149">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4621-149">Request body</span></span>
<span data-ttu-id="c4621-150">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c4621-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4621-151">响应</span><span class="sxs-lookup"><span data-stu-id="c4621-151">Response</span></span>

<span data-ttu-id="c4621-152">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="c4621-152">If successful, this method returns a `200 OK` response code and a [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c4621-153">示例</span><span class="sxs-lookup"><span data-stu-id="c4621-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c4621-154">请求</span><span class="sxs-lookup"><span data-stu-id="c4621-154">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "rbacapplication_roleschedules"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleSchedules(directoryScopeId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',appScopeId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',principalId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',roleDefinitionId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea')
```


### <a name="response"></a><span data-ttu-id="c4621-155">响应</span><span class="sxs-lookup"><span data-stu-id="c4621-155">Response</span></span>
<span data-ttu-id="c4621-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c4621-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleScheduleBase)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.Identity.Governance.Common.Data.ExternalModels.V1.unifiedRoleScheduleBase",
      "id": "String (identifier)",
      "principalId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "roleDefinitionId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "directoryScopeId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "appScopeId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "createdUsing": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "createdDateTime": "2020-09-09T21:32:27.91Z",
      "modifiedDateTime": "2020-09-09T21:32:27.91Z",
      "status": "Provisioned"
    }
  ]
}
```
