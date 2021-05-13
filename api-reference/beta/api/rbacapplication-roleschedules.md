---
title: rbacApplication：roleSchedules
description: 检索 roleAssignmentSchedules 和 roleEligibilitySchedules。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d8bd07d0d029182c163322d2b93ea25a38d94cfd
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474680"
---
# <a name="rbacapplication-roleschedules"></a><span data-ttu-id="4263c-103">rbacApplication：roleSchedules</span><span class="sxs-lookup"><span data-stu-id="4263c-103">rbacApplication: roleSchedules</span></span>
<span data-ttu-id="4263c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4263c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4263c-105">检索 roleAssignmentSchedules 和 roleEligibilitySchedules。</span><span class="sxs-lookup"><span data-stu-id="4263c-105">Retrieve both roleAssignmentSchedules and roleEligibilitySchedules.</span></span>

## <a name="permissions"></a><span data-ttu-id="4263c-106">权限</span><span class="sxs-lookup"><span data-stu-id="4263c-106">Permissions</span></span>
<span data-ttu-id="4263c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4263c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4263c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4263c-109">Permission type</span></span>|<span data-ttu-id="4263c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4263c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4263c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4263c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4263c-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="4263c-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="4263c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4263c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4263c-114">不支持</span><span class="sxs-lookup"><span data-stu-id="4263c-114">Not supported</span></span>|
|<span data-ttu-id="4263c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4263c-115">Application</span></span>|<span data-ttu-id="4263c-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="4263c-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="4263c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4263c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleSchedules
```

## <a name="function-parameters"></a><span data-ttu-id="4263c-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="4263c-118">Function parameters</span></span>
<span data-ttu-id="4263c-119">下表显示了可用于此方法的查询参数。</span><span class="sxs-lookup"><span data-stu-id="4263c-119">The following table shows the query parameters that can be used with this method.</span></span>

|<span data-ttu-id="4263c-120">参数</span><span class="sxs-lookup"><span data-stu-id="4263c-120">Parameter</span></span>|<span data-ttu-id="4263c-121">类型</span><span class="sxs-lookup"><span data-stu-id="4263c-121">Type</span></span>|<span data-ttu-id="4263c-122">说明</span><span class="sxs-lookup"><span data-stu-id="4263c-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4263c-123">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="4263c-123">directoryScopeId</span></span>|<span data-ttu-id="4263c-124">String</span><span class="sxs-lookup"><span data-stu-id="4263c-124">String</span></span>|<span data-ttu-id="4263c-125">表示工作分配范围的目录对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="4263c-125">Id of the directory object that represents the scope of the assignment.</span></span> <span data-ttu-id="4263c-126">工作分配的范围决定了已授予主体访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="4263c-126">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="4263c-127">目录作用域是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="4263c-127">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="4263c-128">应用程序作用域是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="4263c-128">App scopes are scopes that are defined and understood by this application only.</span></span> |
|<span data-ttu-id="4263c-129">appScopeId</span><span class="sxs-lookup"><span data-stu-id="4263c-129">appScopeId</span></span>|<span data-ttu-id="4263c-130">String</span><span class="sxs-lookup"><span data-stu-id="4263c-130">String</span></span>|<span data-ttu-id="4263c-131">特定于应用的范围的 ID。</span><span class="sxs-lookup"><span data-stu-id="4263c-131">Id of the app specific scope.</span></span> <span data-ttu-id="4263c-132">工作分配的范围决定了已授予主体访问权限的资源集。</span><span class="sxs-lookup"><span data-stu-id="4263c-132">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="4263c-133">目录作用域是存储在目录中的多个应用程序可以理解的共享范围。</span><span class="sxs-lookup"><span data-stu-id="4263c-133">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="4263c-134">对租户范围范围使用"/"。</span><span class="sxs-lookup"><span data-stu-id="4263c-134">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="4263c-135">应用程序作用域是仅由此应用程序定义和理解的范围。</span><span class="sxs-lookup"><span data-stu-id="4263c-135">App scopes are scopes that are defined and understood by this application only.</span></span> |
|<span data-ttu-id="4263c-136">principalId</span><span class="sxs-lookup"><span data-stu-id="4263c-136">principalId</span></span>|<span data-ttu-id="4263c-137">String</span><span class="sxs-lookup"><span data-stu-id="4263c-137">String</span></span>|<span data-ttu-id="4263c-138">计划所属的主体的 Objectid。</span><span class="sxs-lookup"><span data-stu-id="4263c-138">Objectid of the principal to which the schedules belong.</span></span> |
|<span data-ttu-id="4263c-139">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="4263c-139">roleDefinitionId</span></span>|<span data-ttu-id="4263c-140">String</span><span class="sxs-lookup"><span data-stu-id="4263c-140">String</span></span>|<span data-ttu-id="4263c-141">工作分配的 unifiedRoleDefinition 的 ID。</span><span class="sxs-lookup"><span data-stu-id="4263c-141">ID of the unifiedRoleDefinition for the assignment.</span></span> <span data-ttu-id="4263c-142">只读。</span><span class="sxs-lookup"><span data-stu-id="4263c-142">Read only.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="4263c-143">请求标头</span><span class="sxs-lookup"><span data-stu-id="4263c-143">Request headers</span></span>
|<span data-ttu-id="4263c-144">名称</span><span class="sxs-lookup"><span data-stu-id="4263c-144">Name</span></span>|<span data-ttu-id="4263c-145">说明</span><span class="sxs-lookup"><span data-stu-id="4263c-145">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4263c-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="4263c-146">Authorization</span></span>|<span data-ttu-id="4263c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4263c-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4263c-149">请求正文</span><span class="sxs-lookup"><span data-stu-id="4263c-149">Request body</span></span>
<span data-ttu-id="4263c-150">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4263c-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4263c-151">响应</span><span class="sxs-lookup"><span data-stu-id="4263c-151">Response</span></span>

<span data-ttu-id="4263c-152">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="4263c-152">If successful, this method returns a `200 OK` response code and a [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4263c-153">示例</span><span class="sxs-lookup"><span data-stu-id="4263c-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4263c-154">请求</span><span class="sxs-lookup"><span data-stu-id="4263c-154">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4263c-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="4263c-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rbacapplication_roleschedules"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleSchedules(directoryScopeId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',appScopeId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',principalId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',roleDefinitionId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea')
```
# <a name="c"></a>[<span data-ttu-id="4263c-156">C#</span><span class="sxs-lookup"><span data-stu-id="4263c-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rbacapplication-roleschedules-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4263c-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4263c-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rbacapplication-roleschedules-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4263c-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4263c-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rbacapplication-roleschedules-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4263c-159">Java</span><span class="sxs-lookup"><span data-stu-id="4263c-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rbacapplication-roleschedules-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4263c-160">响应</span><span class="sxs-lookup"><span data-stu-id="4263c-160">Response</span></span>
<span data-ttu-id="4263c-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4263c-161">**Note:** The response object shown here might be shortened for readability.</span></span>
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
