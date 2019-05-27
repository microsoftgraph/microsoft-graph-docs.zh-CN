---
title: 获取 governanceRoleAssignmentRequest
description: '获取 governanceRoleAssignmentRequest。 '
localization_priority: Normal
ms.openlocfilehash: ce48ed5596d9ad3000bc7ee24ff67c08d0b1814b
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422411"
---
# <a name="get-governanceroleassignmentrequest"></a><span data-ttu-id="6c44b-103">获取 governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="6c44b-103">Get governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c44b-104">获取[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="6c44b-104">Get a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="6c44b-105">权限</span><span class="sxs-lookup"><span data-stu-id="6c44b-105">Permissions</span></span>
<span data-ttu-id="6c44b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c44b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c44b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c44b-108">Permission type</span></span>      | <span data-ttu-id="6c44b-109">权限</span><span class="sxs-lookup"><span data-stu-id="6c44b-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c44b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c44b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6c44b-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="6c44b-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="6c44b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c44b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c44b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c44b-113">Not supported.</span></span>    |
|<span data-ttu-id="6c44b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c44b-114">Application</span></span> | <span data-ttu-id="6c44b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c44b-115">Not supported.</span></span> |

<span data-ttu-id="6c44b-116">除了权限范围之外, 还需要请求程序</span><span class="sxs-lookup"><span data-stu-id="6c44b-116">Besides the permission scope, it requires the requestor</span></span> 
*   <span data-ttu-id="6c44b-117">对资源至少有一个角色分配;和</span><span class="sxs-lookup"><span data-stu-id="6c44b-117">to have at least one role assignment on the resource; or</span></span>
*   <span data-ttu-id="6c44b-118">是[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)的主题。</span><span class="sxs-lookup"><span data-stu-id="6c44b-118">is the subject of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="6c44b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c44b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleAssignmentRequests/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6c44b-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6c44b-120">Optional query parameters</span></span>
<span data-ttu-id="6c44b-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6c44b-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c44b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c44b-122">Request headers</span></span>
| <span data-ttu-id="6c44b-123">名称</span><span class="sxs-lookup"><span data-stu-id="6c44b-123">Name</span></span>      |<span data-ttu-id="6c44b-124">说明</span><span class="sxs-lookup"><span data-stu-id="6c44b-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6c44b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c44b-125">Authorization</span></span>  | <span data-ttu-id="6c44b-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6c44b-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c44b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c44b-127">Request body</span></span>
<span data-ttu-id="6c44b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6c44b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c44b-129">响应</span><span class="sxs-lookup"><span data-stu-id="6c44b-129">Response</span></span>
<span data-ttu-id="6c44b-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6c44b-130">If successful, this method returns a `200 OK` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c44b-131">示例</span><span class="sxs-lookup"><span data-stu-id="6c44b-131">Example</span></span>
<span data-ttu-id="6c44b-132">获取角色分配请求</span><span class="sxs-lookup"><span data-stu-id="6c44b-132">Get a role assignment request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequest"
}-->
##### <a name="request"></a><span data-ttu-id="6c44b-133">请求</span><span class="sxs-lookup"><span data-stu-id="6c44b-133">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/e68ff888-4af5-4ccb-8b74-39156090344b
```
##### <a name="response"></a><span data-ttu-id="6c44b-134">响应</span><span class="sxs-lookup"><span data-stu-id="6c44b-134">Response</span></span>
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
