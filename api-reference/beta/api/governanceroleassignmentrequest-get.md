---
title: 获取 governanceRoleAssignmentRequest
description: '获取 governanceRoleAssignmentRequest。 '
ms.openlocfilehash: aac41bd8443d6066a7866462624a072db57b35da
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191093"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="2493f-103">获取 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="2493f-103">Get governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="2493f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2493f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2493f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2493f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2493f-106">获取[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="2493f-106">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="2493f-107">权限</span><span class="sxs-lookup"><span data-stu-id="2493f-107">Permissions</span></span>
<span data-ttu-id="2493f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2493f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2493f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2493f-110">Permission type</span></span>      | <span data-ttu-id="2493f-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="2493f-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2493f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2493f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2493f-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="2493f-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="2493f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2493f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2493f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2493f-115">Not supported.</span></span>    |
|<span data-ttu-id="2493f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2493f-116">Application</span></span> | <span data-ttu-id="2493f-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="2493f-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="2493f-118">除了权限范围，它需要请求程序</span><span class="sxs-lookup"><span data-stu-id="2493f-118">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="2493f-119">若要对资源; 具有至少一个角色分配或</span><span class="sxs-lookup"><span data-stu-id="2493f-119">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="2493f-120">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)的主题。</span><span class="sxs-lookup"><span data-stu-id="2493f-120">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="2493f-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2493f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2493f-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2493f-122">Optional query parameters</span></span>
<span data-ttu-id="2493f-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2493f-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2493f-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="2493f-124">Request headers</span></span>
| <span data-ttu-id="2493f-125">名称</span><span class="sxs-lookup"><span data-stu-id="2493f-125">Name</span></span>      |<span data-ttu-id="2493f-126">说明</span><span class="sxs-lookup"><span data-stu-id="2493f-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2493f-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="2493f-127">Authorization</span></span>  | <span data-ttu-id="2493f-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2493f-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2493f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="2493f-129">Request body</span></span>
<span data-ttu-id="2493f-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2493f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2493f-131">响应</span><span class="sxs-lookup"><span data-stu-id="2493f-131">Response</span></span>
<span data-ttu-id="2493f-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2493f-132">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2493f-133">示例</span><span class="sxs-lookup"><span data-stu-id="2493f-133">Example</span></span>
<span data-ttu-id="2493f-134">获取一个角色分配请求</span><span class="sxs-lookup"><span data-stu-id="2493f-134">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="2493f-135">请求</span><span class="sxs-lookup"><span data-stu-id="2493f-135">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="2493f-136">响应</span><span class="sxs-lookup"><span data-stu-id="2493f-136">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->