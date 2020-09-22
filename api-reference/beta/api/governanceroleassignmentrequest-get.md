---
title: 获取 governanceRoleAssignmentRequest
description: '获取 governanceRoleAssignmentRequest。 '
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 4e63269d627f83e6287e544eb7c6a59ac0e777e8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991101"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="a12d5-103">获取 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="a12d5-103">Get governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="a12d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a12d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a12d5-105">获取 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="a12d5-105">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="a12d5-106">权限</span><span class="sxs-lookup"><span data-stu-id="a12d5-106">Permissions</span></span>
<span data-ttu-id="a12d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a12d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a12d5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a12d5-109">Permission type</span></span>      | <span data-ttu-id="a12d5-110">权限</span><span class="sxs-lookup"><span data-stu-id="a12d5-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a12d5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a12d5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a12d5-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="a12d5-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="a12d5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a12d5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a12d5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a12d5-114">Not supported.</span></span>    |
|<span data-ttu-id="a12d5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a12d5-115">Application</span></span> | <span data-ttu-id="a12d5-116">PrivilegedAccess。 AzureResources</span><span class="sxs-lookup"><span data-stu-id="a12d5-116">PrivilegedAccess.Read.AzureResources</span></span> |

<span data-ttu-id="a12d5-117">除了权限范围之外，还需要请求程序</span><span class="sxs-lookup"><span data-stu-id="a12d5-117">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="a12d5-118">对资源至少有一个角色分配;和</span><span class="sxs-lookup"><span data-stu-id="a12d5-118">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="a12d5-119">是 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)的主题。</span><span class="sxs-lookup"><span data-stu-id="a12d5-119">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="a12d5-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a12d5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a12d5-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a12d5-121">Optional query parameters</span></span>
<span data-ttu-id="a12d5-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a12d5-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a12d5-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="a12d5-123">Request headers</span></span>
| <span data-ttu-id="a12d5-124">名称</span><span class="sxs-lookup"><span data-stu-id="a12d5-124">Name</span></span>      |<span data-ttu-id="a12d5-125">说明</span><span class="sxs-lookup"><span data-stu-id="a12d5-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a12d5-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a12d5-126">Authorization</span></span>  | <span data-ttu-id="a12d5-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a12d5-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a12d5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a12d5-128">Request body</span></span>
<span data-ttu-id="a12d5-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a12d5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a12d5-130">响应</span><span class="sxs-lookup"><span data-stu-id="a12d5-130">Response</span></span>
<span data-ttu-id="a12d5-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a12d5-131">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a12d5-132">示例</span><span class="sxs-lookup"><span data-stu-id="a12d5-132">Example</span></span>
<span data-ttu-id="a12d5-133">获取角色分配请求</span><span class="sxs-lookup"><span data-stu-id="a12d5-133">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="a12d5-134">请求</span><span class="sxs-lookup"><span data-stu-id="a12d5-134">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="a12d5-135">响应</span><span class="sxs-lookup"><span data-stu-id="a12d5-135">Response</span></span>
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


