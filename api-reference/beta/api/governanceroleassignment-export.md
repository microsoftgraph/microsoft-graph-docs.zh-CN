---
title: 导出 governanceRoleAssignmentRequests
description: 检索格式为 的 governanceRoleAssignmentRequests 集合，该集合可在浏览器中.csv `application/octet-stream` 文件的形式进行分析。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 8faff2bbd4b41eda693467b55641204cb6bbaef3
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350843"
---
# <a name="export-governanceroleassignmentrequests"></a><span data-ttu-id="3485c-103">导出 governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="3485c-103">Export governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="3485c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3485c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3485c-105">检索格式为 [的 governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) 集合，该集合可在浏览器中.csv `application/octet-stream` 文件的形式进行分析。</span><span class="sxs-lookup"><span data-stu-id="3485c-105">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) in the format `application/octet-stream`, which can be parsed as a .csv file in the browser.</span></span>

## <a name="permissions"></a><span data-ttu-id="3485c-106">权限</span><span class="sxs-lookup"><span data-stu-id="3485c-106">Permissions</span></span>
<span data-ttu-id="3485c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="3485c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="3485c-109">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="3485c-109">Azure resources</span></span>

| <span data-ttu-id="3485c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3485c-110">Permission type</span></span> | <span data-ttu-id="3485c-111">权限</span><span class="sxs-lookup"><span data-stu-id="3485c-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="3485c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3485c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3485c-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="3485c-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="3485c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3485c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3485c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3485c-115">Not supported.</span></span> |
| <span data-ttu-id="3485c-116">Application</span><span class="sxs-lookup"><span data-stu-id="3485c-116">Application</span></span> | <span data-ttu-id="3485c-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="3485c-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="3485c-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="3485c-118">Azure AD</span></span>

| <span data-ttu-id="3485c-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="3485c-119">Permission type</span></span> | <span data-ttu-id="3485c-120">权限</span><span class="sxs-lookup"><span data-stu-id="3485c-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="3485c-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3485c-121">Delegated (work or school account)</span></span> | <span data-ttu-id="3485c-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="3485c-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="3485c-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3485c-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3485c-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="3485c-124">Not supported.</span></span> |
| <span data-ttu-id="3485c-125">Application</span><span class="sxs-lookup"><span data-stu-id="3485c-125">Application</span></span> | <span data-ttu-id="3485c-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="3485c-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="3485c-127">组</span><span class="sxs-lookup"><span data-stu-id="3485c-127">Groups</span></span>

|<span data-ttu-id="3485c-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="3485c-128">Permission type</span></span> | <span data-ttu-id="3485c-129">权限</span><span class="sxs-lookup"><span data-stu-id="3485c-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="3485c-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3485c-130">Delegated (work or school account)</span></span> | <span data-ttu-id="3485c-131">PrivilegedAccess.ReadWrite.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="3485c-131">PrivilegedAccess.ReadWrite.AzureADGroup</span></span> |
| <span data-ttu-id="3485c-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3485c-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3485c-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="3485c-133">Not supported.</span></span> |
| <span data-ttu-id="3485c-134">Application</span><span class="sxs-lookup"><span data-stu-id="3485c-134">Application</span></span> | <span data-ttu-id="3485c-135">PrivilegedAccess.Read.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="3485c-135">PrivilegedAccess.Read.AzureADGroup</span></span> |


## <a name="http-request"></a><span data-ttu-id="3485c-136">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3485c-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="3485c-137">导出资源上的 [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3485c-137">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource</span></span>
    
><span data-ttu-id="3485c-138">**注意：** 除了权限范围之外，此请求要求请求者至少具有一角色分配资源访问权限。</span><span class="sxs-lookup"><span data-stu-id="3485c-138">**Note:** Besides the permission scope, this request requires the requestor to have at least one role assignment on the resource.</span></span> 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

<span data-ttu-id="3485c-139">导出 mine 的 [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3485c-139">Export a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine</span></span>
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3485c-140">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3485c-140">Optional query parameters</span></span>
<span data-ttu-id="3485c-141">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3485c-141">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3485c-142">请求标头</span><span class="sxs-lookup"><span data-stu-id="3485c-142">Request headers</span></span>
| <span data-ttu-id="3485c-143">名称</span><span class="sxs-lookup"><span data-stu-id="3485c-143">Name</span></span>      |<span data-ttu-id="3485c-144">说明</span><span class="sxs-lookup"><span data-stu-id="3485c-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3485c-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="3485c-145">Authorization</span></span>  | <span data-ttu-id="3485c-146">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3485c-146">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3485c-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="3485c-147">Request body</span></span>
<span data-ttu-id="3485c-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3485c-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3485c-149">响应</span><span class="sxs-lookup"><span data-stu-id="3485c-149">Response</span></span>
<span data-ttu-id="3485c-150">如果成功，此方法返回 响应 `200 OK` 代码和类型 的内容 `application/octet-stream` 。</span><span class="sxs-lookup"><span data-stu-id="3485c-150">If successful, this method returns a `200 OK` response code and content of type `application/octet-stream`.</span></span>

## <a name="example"></a><span data-ttu-id="3485c-151">示例</span><span class="sxs-lookup"><span data-stu-id="3485c-151">Example</span></span>
<span data-ttu-id="3485c-152">本示例将订阅 Wingtip Toys - Prod .csv所有角色分配另存为一个角色分配文件。</span><span class="sxs-lookup"><span data-stu-id="3485c-152">This example saves all role assignments as a .csv file in the subscription Wingtip Toys - Prod.</span></span> 

##### <a name="request"></a><span data-ttu-id="3485c-153">请求</span><span class="sxs-lookup"><span data-stu-id="3485c-153">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a><span data-ttu-id="3485c-154">响应</span><span class="sxs-lookup"><span data-stu-id="3485c-154">Response</span></span>
<span data-ttu-id="3485c-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3485c-155">Here is an example of the response.</span></span> 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


