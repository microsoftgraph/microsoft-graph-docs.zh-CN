---
title: rbacApplication：roleScheduleInstances
description: 检索 roleAssignmentScheduleInstances 和 roleEligibilityScheduleInstances。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 497b29892bb510aec9763cab21ce8f06518a2eee
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679671"
---
# <a name="rbacapplication-rolescheduleinstances"></a><span data-ttu-id="d395c-103">rbacApplication：roleScheduleInstances</span><span class="sxs-lookup"><span data-stu-id="d395c-103">rbacApplication: roleScheduleInstances</span></span>
<span data-ttu-id="d395c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d395c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d395c-105">检索 roleAssignmentScheduleInstances 和 roleEligibilityScheduleInstances。</span><span class="sxs-lookup"><span data-stu-id="d395c-105">Retrieve both roleAssignmentScheduleInstances and roleEligibilityScheduleInstances.</span></span>

## <a name="permissions"></a><span data-ttu-id="d395c-106">权限</span><span class="sxs-lookup"><span data-stu-id="d395c-106">Permissions</span></span>
<span data-ttu-id="d395c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d395c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d395c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d395c-109">Permission type</span></span>|<span data-ttu-id="d395c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d395c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d395c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d395c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d395c-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="d395c-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="d395c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d395c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d395c-114">不支持</span><span class="sxs-lookup"><span data-stu-id="d395c-114">Not supported</span></span>|
|<span data-ttu-id="d395c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d395c-115">Application</span></span>|<span data-ttu-id="d395c-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="d395c-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="d395c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d395c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleScheduleInstances
```

## <a name="query-parameters"></a><span data-ttu-id="d395c-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="d395c-118">Query parameters</span></span>
<span data-ttu-id="d395c-119">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="d395c-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d395c-120">下表显示了可用于此方法的查询参数。</span><span class="sxs-lookup"><span data-stu-id="d395c-120">The following table shows the query parameters that can be used with this method.</span></span>

|<span data-ttu-id="d395c-121">参数</span><span class="sxs-lookup"><span data-stu-id="d395c-121">Parameter</span></span>|<span data-ttu-id="d395c-122">类型</span><span class="sxs-lookup"><span data-stu-id="d395c-122">Type</span></span>|<span data-ttu-id="d395c-123">说明</span><span class="sxs-lookup"><span data-stu-id="d395c-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d395c-124">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="d395c-124">directoryScopeId</span></span>|<span data-ttu-id="d395c-125">String</span><span class="sxs-lookup"><span data-stu-id="d395c-125">String</span></span>|<span data-ttu-id="d395c-126">表示工作分配范围的目录对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="d395c-126">Id of the directory object that represents the scope of the assignment.</span></span> <span data-ttu-id="d395c-127">工作分配的范围决定了已授予主体访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="d395c-127">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="d395c-128">目录作用域是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="d395c-128">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="d395c-129">应用程序作用域是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="d395c-129">App scopes are scopes that are defined and understood by this application only.</span></span> |
|<span data-ttu-id="d395c-130">appScopeId</span><span class="sxs-lookup"><span data-stu-id="d395c-130">appScopeId</span></span>|<span data-ttu-id="d395c-131">String</span><span class="sxs-lookup"><span data-stu-id="d395c-131">String</span></span>|<span data-ttu-id="d395c-132">特定于应用的范围的 ID。</span><span class="sxs-lookup"><span data-stu-id="d395c-132">Id of the app specific scope.</span></span> <span data-ttu-id="d395c-133">工作分配的范围决定了已授予主体访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="d395c-133">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="d395c-134">目录作用域是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="d395c-134">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="d395c-135">对租户范围范围使用"/"。</span><span class="sxs-lookup"><span data-stu-id="d395c-135">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="d395c-136">应用程序作用域是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="d395c-136">App scopes are scopes that are defined and understood by this application only.</span></span> |
|<span data-ttu-id="d395c-137">principalId</span><span class="sxs-lookup"><span data-stu-id="d395c-137">principalId</span></span>|<span data-ttu-id="d395c-138">String</span><span class="sxs-lookup"><span data-stu-id="d395c-138">String</span></span>|<span data-ttu-id="d395c-139">计划所属的主体的 Objectid。</span><span class="sxs-lookup"><span data-stu-id="d395c-139">Objectid of the principal to which the schedules belong.</span></span> |
|<span data-ttu-id="d395c-140">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="d395c-140">roleDefinitionId</span></span>|<span data-ttu-id="d395c-141">String</span><span class="sxs-lookup"><span data-stu-id="d395c-141">String</span></span>|<span data-ttu-id="d395c-142">工作分配的 unifiedRoleDefinition 的 ID。</span><span class="sxs-lookup"><span data-stu-id="d395c-142">ID of the unifiedRoleDefinition for the assignment.</span></span> <span data-ttu-id="d395c-143">只读。</span><span class="sxs-lookup"><span data-stu-id="d395c-143">Read only.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="d395c-144">请求标头</span><span class="sxs-lookup"><span data-stu-id="d395c-144">Request headers</span></span>
|<span data-ttu-id="d395c-145">名称</span><span class="sxs-lookup"><span data-stu-id="d395c-145">Name</span></span>|<span data-ttu-id="d395c-146">说明</span><span class="sxs-lookup"><span data-stu-id="d395c-146">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d395c-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="d395c-147">Authorization</span></span>|<span data-ttu-id="d395c-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d395c-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d395c-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="d395c-150">Request body</span></span>
<span data-ttu-id="d395c-151">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d395c-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d395c-152">响应</span><span class="sxs-lookup"><span data-stu-id="d395c-152">Response</span></span>

<span data-ttu-id="d395c-153">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="d395c-153">If successful, this method returns a `200 OK` response code and a [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d395c-154">示例</span><span class="sxs-lookup"><span data-stu-id="d395c-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d395c-155">请求</span><span class="sxs-lookup"><span data-stu-id="d395c-155">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d395c-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="d395c-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rbacapplication_rolescheduleinstances"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleScheduleInstances(directoryScopeId='parameterValue',appScopeId='parameterValue',principalId='parameterValue',roleDefinitionId='parameterValue')
```
# <a name="c"></a>[<span data-ttu-id="d395c-157">C#</span><span class="sxs-lookup"><span data-stu-id="d395c-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rbacapplication-rolescheduleinstances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d395c-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d395c-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rbacapplication-rolescheduleinstances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d395c-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d395c-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rbacapplication-rolescheduleinstances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d395c-160">Java</span><span class="sxs-lookup"><span data-stu-id="d395c-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rbacapplication-rolescheduleinstances-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d395c-161">响应</span><span class="sxs-lookup"><span data-stu-id="d395c-161">Response</span></span>
<span data-ttu-id="d395c-162">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d395c-162">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleScheduleInstanceBase)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.Identity.Governance.Common.Data.ExternalModels.V1.unifiedRoleScheduleInstanceBase",
      "id": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "principalId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "roleDefinitionId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "directoryScopeId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "appScopeId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea"
    }
  ]
}
```
