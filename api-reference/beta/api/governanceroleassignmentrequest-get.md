---
title: 获取 governanceRoleAssignmentRequest
description: '获取 governanceRoleAssignmentRequest。 '
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identitiy-platform
ms.openlocfilehash: 1e659e5b3aefbd3995bd4e04b28b5de87d2f4fe4
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639826"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="d3c54-103">获取 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="d3c54-103">Get governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="d3c54-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3c54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3c54-105">获取[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="d3c54-105">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="d3c54-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="d3c54-106">Permissions</span></span>
<span data-ttu-id="d3c54-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3c54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3c54-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3c54-109">Permission type</span></span>      | <span data-ttu-id="d3c54-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="d3c54-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3c54-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3c54-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d3c54-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="d3c54-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="d3c54-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3c54-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3c54-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3c54-114">Not supported.</span></span>    |
|<span data-ttu-id="d3c54-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3c54-115">Application</span></span> | <span data-ttu-id="d3c54-116">PrivilegedAccess。 AzureResources</span><span class="sxs-lookup"><span data-stu-id="d3c54-116">PrivilegedAccess.Read.AzureResources</span></span> |

<span data-ttu-id="d3c54-117">除了权限范围之外，还需要请求程序</span><span class="sxs-lookup"><span data-stu-id="d3c54-117">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="d3c54-118">对资源至少有一个角色分配;和</span><span class="sxs-lookup"><span data-stu-id="d3c54-118">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="d3c54-119">是[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)的主题。</span><span class="sxs-lookup"><span data-stu-id="d3c54-119">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="d3c54-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3c54-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d3c54-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d3c54-121">Optional query parameters</span></span>
<span data-ttu-id="d3c54-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d3c54-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3c54-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3c54-123">Request headers</span></span>
| <span data-ttu-id="d3c54-124">名称</span><span class="sxs-lookup"><span data-stu-id="d3c54-124">Name</span></span>      |<span data-ttu-id="d3c54-125">说明</span><span class="sxs-lookup"><span data-stu-id="d3c54-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d3c54-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3c54-126">Authorization</span></span>  | <span data-ttu-id="d3c54-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d3c54-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3c54-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3c54-128">Request body</span></span>
<span data-ttu-id="d3c54-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d3c54-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3c54-130">响应</span><span class="sxs-lookup"><span data-stu-id="d3c54-130">Response</span></span>
<span data-ttu-id="d3c54-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d3c54-131">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3c54-132">示例</span><span class="sxs-lookup"><span data-stu-id="d3c54-132">Example</span></span>
<span data-ttu-id="d3c54-133">获取角色分配请求</span><span class="sxs-lookup"><span data-stu-id="d3c54-133">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="d3c54-134">请求</span><span class="sxs-lookup"><span data-stu-id="d3c54-134">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="d3c54-135">响应</span><span class="sxs-lookup"><span data-stu-id="d3c54-135">Response</span></span>
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
