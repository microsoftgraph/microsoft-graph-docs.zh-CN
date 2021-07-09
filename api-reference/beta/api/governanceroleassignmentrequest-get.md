---
title: 获取 governanceRoleAssignmentRequest
description: '获取 governanceRoleAssignmentRequest。 '
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 87eae92aac54284407da6e33158e65819eadbd4e
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350764"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="c4da3-103">获取 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="c4da3-103">Get governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="c4da3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4da3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4da3-105">获取 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="c4da3-105">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="c4da3-106">权限</span><span class="sxs-lookup"><span data-stu-id="c4da3-106">Permissions</span></span>
<span data-ttu-id="c4da3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="c4da3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="c4da3-109">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="c4da3-109">Azure resources</span></span>

| <span data-ttu-id="c4da3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4da3-110">Permission type</span></span> | <span data-ttu-id="c4da3-111">权限</span><span class="sxs-lookup"><span data-stu-id="c4da3-111">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="c4da3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4da3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c4da3-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c4da3-113">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="c4da3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4da3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4da3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4da3-115">Not supported.</span></span> |
| <span data-ttu-id="c4da3-116">Application</span><span class="sxs-lookup"><span data-stu-id="c4da3-116">Application</span></span> | <span data-ttu-id="c4da3-117">PrivilegedAccess.Read.AzureResources</span><span class="sxs-lookup"><span data-stu-id="c4da3-117">PrivilegedAccess.Read.AzureResources</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="c4da3-118">Azure AD</span><span class="sxs-lookup"><span data-stu-id="c4da3-118">Azure AD</span></span>

| <span data-ttu-id="c4da3-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4da3-119">Permission type</span></span> | <span data-ttu-id="c4da3-120">权限</span><span class="sxs-lookup"><span data-stu-id="c4da3-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="c4da3-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4da3-121">Delegated (work or school account)</span></span> | <span data-ttu-id="c4da3-122">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="c4da3-122">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="c4da3-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4da3-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4da3-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4da3-124">Not supported.</span></span> |
| <span data-ttu-id="c4da3-125">Application</span><span class="sxs-lookup"><span data-stu-id="c4da3-125">Application</span></span> | <span data-ttu-id="c4da3-126">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="c4da3-126">PrivilegedAccess.Read.AzureAD</span></span> |

### <a name="groups"></a><span data-ttu-id="c4da3-127">组</span><span class="sxs-lookup"><span data-stu-id="c4da3-127">Groups</span></span>

|<span data-ttu-id="c4da3-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4da3-128">Permission type</span></span> | <span data-ttu-id="c4da3-129">权限</span><span class="sxs-lookup"><span data-stu-id="c4da3-129">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="c4da3-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4da3-130">Delegated (work or school account)</span></span> | <span data-ttu-id="c4da3-131">PrivilegedAccess.ReadWrite.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="c4da3-131">PrivilegedAccess.ReadWrite.AzureADGroup</span></span> |
| <span data-ttu-id="c4da3-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4da3-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4da3-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4da3-133">Not supported.</span></span> |
| <span data-ttu-id="c4da3-134">Application</span><span class="sxs-lookup"><span data-stu-id="c4da3-134">Application</span></span> | <span data-ttu-id="c4da3-135">PrivilegedAccess.Read.AzureADGroup</span><span class="sxs-lookup"><span data-stu-id="c4da3-135">PrivilegedAccess.Read.AzureADGroup</span></span> |

<span data-ttu-id="c4da3-136">除了权限范围之外，它还需要请求者</span><span class="sxs-lookup"><span data-stu-id="c4da3-136">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="c4da3-137">至少对资源角色分配一个资源;或</span><span class="sxs-lookup"><span data-stu-id="c4da3-137">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="c4da3-138">是 [governanceRoleAssignmentRequest 的主题](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="c4da3-138">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="c4da3-139">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4da3-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c4da3-140">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c4da3-140">Optional query parameters</span></span>
<span data-ttu-id="c4da3-141">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c4da3-141">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4da3-142">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4da3-142">Request headers</span></span>
| <span data-ttu-id="c4da3-143">名称</span><span class="sxs-lookup"><span data-stu-id="c4da3-143">Name</span></span>      |<span data-ttu-id="c4da3-144">说明</span><span class="sxs-lookup"><span data-stu-id="c4da3-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c4da3-145">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4da3-145">Authorization</span></span>  | <span data-ttu-id="c4da3-146">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c4da3-146">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4da3-147">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4da3-147">Request body</span></span>
<span data-ttu-id="c4da3-148">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c4da3-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4da3-149">响应</span><span class="sxs-lookup"><span data-stu-id="c4da3-149">Response</span></span>
<span data-ttu-id="c4da3-150">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c4da3-150">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4da3-151">示例</span><span class="sxs-lookup"><span data-stu-id="c4da3-151">Example</span></span>
<span data-ttu-id="c4da3-152">获取角色分配请求</span><span class="sxs-lookup"><span data-stu-id="c4da3-152">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="c4da3-153">请求</span><span class="sxs-lookup"><span data-stu-id="c4da3-153">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="c4da3-154">响应</span><span class="sxs-lookup"><span data-stu-id="c4da3-154">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"e68ff888-4af5-4ccb-8b74-39156090344b",
  "resourceId":"ec3a00f7-81dc-43b3-bbe7-650d3a5f7d46",
  "roleDefinitionId":"be0767b9-2c31-4b0d-b820-726228e7ff5c",
  "subjectId":"a4c5a837-b546-4ec5-a7df-e61547a46a4b",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminRemove",
  "assignmentState":"Eligible",
  "requestedDateTime":"2018-05-09T21:26:15.73-07:00",
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


