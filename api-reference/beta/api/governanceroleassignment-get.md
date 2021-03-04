---
title: 获取 governanceRoleAssignment
description: 检索 governanceRoleAssignment 的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 3f01060b80c9f50712014a16987d519d19b5bf91
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435922"
---
# <a name="get-governanceroleassignment"></a><span data-ttu-id="c7347-103">获取 governanceRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c7347-103">Get governanceRoleAssignment</span></span>

<span data-ttu-id="c7347-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7347-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7347-105">检索 [governanceRoleAssignment 的属性和关系](../resources/governanceroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="c7347-105">Retrieve the properties and relationships of a [governanceRoleAssignment](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c7347-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c7347-106">Permissions</span></span>
<span data-ttu-id="c7347-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="c7347-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="c7347-109">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="c7347-109">Azure resources</span></span>

| <span data-ttu-id="c7347-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7347-110">Permission type</span></span> | <span data-ttu-id="c7347-111">权限</span><span class="sxs-lookup"><span data-stu-id="c7347-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="c7347-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7347-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c7347-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c7347-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="c7347-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7347-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7347-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7347-115">Not supported.</span></span> |
| <span data-ttu-id="c7347-116">Application</span><span class="sxs-lookup"><span data-stu-id="c7347-116">Application</span></span> | <span data-ttu-id="c7347-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c7347-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="c7347-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="c7347-118">Azure AD</span></span>

| <span data-ttu-id="c7347-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7347-119">Permission type</span></span> | <span data-ttu-id="c7347-120">权限</span><span class="sxs-lookup"><span data-stu-id="c7347-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="c7347-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7347-121">Delegated (work or school account)</span></span> | <span data-ttu-id="c7347-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="c7347-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="c7347-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7347-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7347-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7347-124">Not supported.</span></span> |
| <span data-ttu-id="c7347-125">Application</span><span class="sxs-lookup"><span data-stu-id="c7347-125">Application</span></span> | <span data-ttu-id="c7347-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="c7347-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="c7347-127">组</span><span class="sxs-lookup"><span data-stu-id="c7347-127">Groups</span></span>

|<span data-ttu-id="c7347-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7347-128">Permission type</span></span> | <span data-ttu-id="c7347-129">权限</span><span class="sxs-lookup"><span data-stu-id="c7347-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="c7347-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7347-130">Delegated (work or school account)</span></span> | <span data-ttu-id="c7347-131">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="c7347-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="c7347-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7347-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7347-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7347-133">Not supported.</span></span> |
| <span data-ttu-id="c7347-134">Application</span><span class="sxs-lookup"><span data-stu-id="c7347-134">Application</span></span> | <span data-ttu-id="c7347-135">PrivilegedAccess.Read.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="c7347-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7347-136">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7347-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
1. <span data-ttu-id="c7347-137">获取[资源上的 governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c7347-137">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on a resource</span></span>

    <span data-ttu-id="c7347-138">*注意：除了权限范围之外，它要求请求者至少对资源角色分配一个权限。*</span><span class="sxs-lookup"><span data-stu-id="c7347-138">*Note: Besides the permission scope, it requires the requestor to have at least one role assignment on the resource.*</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments/{id}
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=resourceId+eq+'{resourceId}'
```
2. <span data-ttu-id="c7347-139">获取[我的 governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c7347-139">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/{id}?$filter=subjectId+eq+'{myId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7347-140">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c7347-140">Optional query parameters</span></span>
<span data-ttu-id="c7347-141">除了帮助 **自定义** 响应外，此方法不支持 [OData](/graph/query-parameters) 查询 `$filter` 参数。</span><span class="sxs-lookup"><span data-stu-id="c7347-141">This method does **not** supports [OData Query Parameters](/graph/query-parameters) other than `$filter` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7347-142">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7347-142">Request headers</span></span>
| <span data-ttu-id="c7347-143">名称</span><span class="sxs-lookup"><span data-stu-id="c7347-143">Name</span></span>      |<span data-ttu-id="c7347-144">说明</span><span class="sxs-lookup"><span data-stu-id="c7347-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c7347-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7347-145">Authorization</span></span>  | <span data-ttu-id="c7347-146">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c7347-146">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7347-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7347-147">Request body</span></span>
<span data-ttu-id="c7347-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c7347-148">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c7347-149">响应</span><span class="sxs-lookup"><span data-stu-id="c7347-149">Response</span></span>
<span data-ttu-id="c7347-150">如果成功，此方法在响应正文中返回响应 `200 OK` 代码 [和 governanceRoleAssignment](../resources/governanceroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c7347-150">If successful, this method returns a `200 OK` response code and [governanceRoleAssignment](../resources/governanceroleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c7347-151">示例</span><span class="sxs-lookup"><span data-stu-id="c7347-151">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignment"
}-->
<span data-ttu-id="c7347-152">获取订阅"Wingtip Toys - Prod"的[governanceRoleAssignment](../resources/governanceroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c7347-152">Get a [governanceRoleAssignment](../resources/governanceroleassignment.md) on subscription "Wingtip Toys - Prod"</span></span>
##### <a name="request"></a><span data-ttu-id="c7347-153">请求</span><span class="sxs-lookup"><span data-stu-id="c7347-153">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/0ba78f41-ee7a-4227-adb9-1499431b2164?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="c7347-154">响应</span><span class="sxs-lookup"><span data-stu-id="c7347-154">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 182

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignments/$entity",
    "id": "0ba78f41-ee7a-4227-adb9-1499431b2164",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
    "subjectId": "74487eb5-1630-4fa8-9581-0bb076ea5de3",
    "linkedEligibleRoleAssignmentId": null,
    "externalId": null,
    "startDateTime": "2018-01-22T23:47:19.687Z",
    "endDateTime": "2018-07-21T23:47:02.887Z",
    "memberType": "Direct",
    "assignmentState": "Eligible",
    "status": "Provisioned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


