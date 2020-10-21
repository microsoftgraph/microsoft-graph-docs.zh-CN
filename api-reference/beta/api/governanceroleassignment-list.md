---
title: 列出 governanceRoleAssignments
description: 检索 governanceRoleAssignments 的集合。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 338fb9c4d02b87e940fbb0fc867edbb374e9d42b
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635024"
---
# <a name="list-governanceroleassignments"></a><span data-ttu-id="0361b-103">列出 governanceRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="0361b-103">List governanceRoleAssignments</span></span>

<span data-ttu-id="0361b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0361b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0361b-105">检索 [governanceRoleAssignments](../resources/governanceroleassignment.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="0361b-105">Retrieve a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0361b-106">权限</span><span class="sxs-lookup"><span data-stu-id="0361b-106">Permissions</span></span>
<span data-ttu-id="0361b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="0361b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="0361b-109">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="0361b-109">Azure resources</span></span>

| <span data-ttu-id="0361b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0361b-110">Permission type</span></span> | <span data-ttu-id="0361b-111">权限</span><span class="sxs-lookup"><span data-stu-id="0361b-111">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="0361b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0361b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0361b-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="0361b-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="0361b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0361b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0361b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0361b-115">Not supported.</span></span> |
| <span data-ttu-id="0361b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0361b-116">Application</span></span> | <span data-ttu-id="0361b-117">PrivilegedAccess。 AzureResources</span><span class="sxs-lookup"><span data-stu-id="0361b-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="0361b-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="0361b-118">Azure AD</span></span>

| <span data-ttu-id="0361b-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="0361b-119">Permission type</span></span> | <span data-ttu-id="0361b-120">权限</span><span class="sxs-lookup"><span data-stu-id="0361b-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="0361b-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0361b-121">Delegated (work or school account)</span></span> | <span data-ttu-id="0361b-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="0361b-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="0361b-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0361b-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0361b-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="0361b-124">Not supported.</span></span> |
| <span data-ttu-id="0361b-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="0361b-125">Application</span></span> | <span data-ttu-id="0361b-126">PrivilegedAccess。 AzureAD</span><span class="sxs-lookup"><span data-stu-id="0361b-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="0361b-127">组</span><span class="sxs-lookup"><span data-stu-id="0361b-127">Groups</span></span>

|<span data-ttu-id="0361b-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="0361b-128">Permission type</span></span> | <span data-ttu-id="0361b-129">权限</span><span class="sxs-lookup"><span data-stu-id="0361b-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="0361b-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0361b-130">Delegated (work or school account)</span></span> | <span data-ttu-id="0361b-131">PrivilegedAccess AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="0361b-131">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="0361b-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0361b-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0361b-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="0361b-133">Not supported.</span></span> |
| <span data-ttu-id="0361b-134">应用程序</span><span class="sxs-lookup"><span data-stu-id="0361b-134">Application</span></span> | <span data-ttu-id="0361b-135">PrivilegedAccess。 AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="0361b-135">PrivilegedAccess.Read.AzureADGroups</span></span> |

## <a name="http-request"></a><span data-ttu-id="0361b-136">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0361b-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="0361b-137">列出资源上的 [governanceRoleAssignments](../resources/governanceroleassignment.md) 的集合。</span><span class="sxs-lookup"><span data-stu-id="0361b-137">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) on a resource.</span></span>

><span data-ttu-id="0361b-138">**注意：** 除了权限范围之外，此请求还要求请求者在资源上至少有一个角色分配。</span><span class="sxs-lookup"><span data-stu-id="0361b-138">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignments
GET /privilegedAccess/azureResources/roleAssignments?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="0361b-139">列出地雷的 [governanceRoleAssignments](../resources/governanceroleassignment.md) 的集合。</span><span class="sxs-lookup"><span data-stu-id="0361b-139">List a collection of [governanceRoleAssignments](../resources/governanceroleassignment.md) of mine.</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0361b-140">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0361b-140">Optional query parameters</span></span>
<span data-ttu-id="0361b-141">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0361b-141">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0361b-142">请求标头</span><span class="sxs-lookup"><span data-stu-id="0361b-142">Request headers</span></span>
| <span data-ttu-id="0361b-143">名称</span><span class="sxs-lookup"><span data-stu-id="0361b-143">Name</span></span>      |<span data-ttu-id="0361b-144">说明</span><span class="sxs-lookup"><span data-stu-id="0361b-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0361b-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="0361b-145">Authorization</span></span>  | <span data-ttu-id="0361b-146">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0361b-146">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0361b-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="0361b-147">Request body</span></span>
<span data-ttu-id="0361b-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0361b-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0361b-149">响应</span><span class="sxs-lookup"><span data-stu-id="0361b-149">Response</span></span>
<span data-ttu-id="0361b-150">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [governanceRoleAssignment](../resources/governanceroleassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0361b-150">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignment](../resources/governanceroleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0361b-151">示例</span><span class="sxs-lookup"><span data-stu-id="0361b-151">Example</span></span>

<span data-ttu-id="0361b-152">本示例演示如何在订阅 Wingtip 玩具-生产中获取我的角色分配。</span><span class="sxs-lookup"><span data-stu-id="0361b-152">This example shows how to get my role assignments on the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignments"
}-->
##### <a name="request"></a><span data-ttu-id="0361b-153">请求</span><span class="sxs-lookup"><span data-stu-id="0361b-153">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments?$filter=subjectId+eq+'918e54be-12c4-4f4c-a6d3-2ee0e3661c51'
```
##### <a name="response"></a><span data-ttu-id="0361b-154">响应</span><span class="sxs-lookup"><span data-stu-id="0361b-154">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 2062

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignments",
    "value": [
        {
            "id": "20f4157d-5837-4356-9630-ebd3a832f227",
            "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
            "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": null,
            "externalId": null,
            "startDateTime": "2018-03-13T01:19:08.59Z",
            "endDateTime": "2018-06-11T01:18:37.08Z",
            "memberType": "Direct",
            "assignmentState": "Eligible",
            "status": "Provisioned"
        },
        {
            "id": "e327f4be-42a0-47a2-8579-0a39b025b394",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": null,
            "externalId": null,
            "startDateTime": "2018-03-28T16:56:48.243Z",
            "endDateTime": "2018-09-24T16:56:30.547Z",
            "memberType": "Direct",
            "assignmentState": "Eligible",
            "status": "Provisioned"
        },
        ...
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List roleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


