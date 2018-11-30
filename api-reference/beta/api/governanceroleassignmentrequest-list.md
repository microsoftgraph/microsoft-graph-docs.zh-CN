---
title: 列表 governanceRoleAssignmentRequests
description: '检索 governanceRoleAssignmentRequests 的集合。 '
ms.openlocfilehash: 2d3cb7e668e6da4016106843f2e80ed4be784aef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043611"
---
# <a name="list-governanceroleassignmentrequests"></a><span data-ttu-id="367ea-103">列表 governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="367ea-103">List governanceRoleAssignmentRequests</span></span>

> <span data-ttu-id="367ea-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="367ea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="367ea-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="367ea-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="367ea-106">检索[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="367ea-106">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="367ea-107">权限</span><span class="sxs-lookup"><span data-stu-id="367ea-107">Permissions</span></span>
<span data-ttu-id="367ea-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="367ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="367ea-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="367ea-110">Permission type</span></span>      | <span data-ttu-id="367ea-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="367ea-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="367ea-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="367ea-112">Delegated (work or school account)</span></span> | <span data-ttu-id="367ea-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="367ea-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="367ea-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="367ea-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="367ea-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="367ea-115">Not supported.</span></span>    |
|<span data-ttu-id="367ea-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="367ea-116">Application</span></span> | <span data-ttu-id="367ea-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="367ea-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="367ea-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="367ea-118">HTTP request</span></span>
<span data-ttu-id="367ea-119"><!-- { "blockType": "ignored" } -->列出[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)对资源的集合。</span><span class="sxs-lookup"><span data-stu-id="367ea-119"><!-- { "blockType": "ignored" } --> List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource.</span></span>
    
><span data-ttu-id="367ea-120">**注意：** 除了权限范围，该请求需要具有至少一个角色分配对资源的请求程序。</span><span class="sxs-lookup"><span data-stu-id="367ea-120">**Note:** Besides the permission scope, the request requires the requestor to have at least one role assignment on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignmentRequests
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="367ea-121">列出的[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)我的集合。</span><span class="sxs-lookup"><span data-stu-id="367ea-121">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=subjectId+eq+'{myId}'
```

<span data-ttu-id="367ea-122">列出的[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)挂起管理员决策的集合。</span><span class="sxs-lookup"><span data-stu-id="367ea-122">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are pending administrator decisions.</span></span>
    
><span data-ttu-id="367ea-123">**注意：** 除了权限范围，此请求需要请求程序至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="367ea-123">**Note:** Besides the permission scope, this request requires the requestor to have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=status/subStatus+eq+'PendingAdminDecision'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="367ea-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="367ea-124">Optional query parameters</span></span>
<span data-ttu-id="367ea-125">此方法支持[OData 查询参数](/graph/query-parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="367ea-125">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="367ea-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="367ea-126">Request headers</span></span>
| <span data-ttu-id="367ea-127">名称</span><span class="sxs-lookup"><span data-stu-id="367ea-127">Name</span></span>      |<span data-ttu-id="367ea-128">说明</span><span class="sxs-lookup"><span data-stu-id="367ea-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="367ea-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="367ea-129">Authorization</span></span>  | <span data-ttu-id="367ea-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="367ea-130">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="367ea-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="367ea-131">Request body</span></span>
<span data-ttu-id="367ea-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="367ea-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="367ea-133">响应</span><span class="sxs-lookup"><span data-stu-id="367ea-133">Response</span></span>
<span data-ttu-id="367ea-134">如果成功，此方法返回`200 OK`响应代码和响应正文中的[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="367ea-134">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="367ea-135">示例</span><span class="sxs-lookup"><span data-stu-id="367ea-135">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequests"
}-->
<span data-ttu-id="367ea-136">管理员查询订阅 Wingtip Toys-prod 移待处理的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="367ea-136">Administrators query pending role assignment requests for subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="367ea-137">请求</span><span class="sxs-lookup"><span data-stu-id="367ea-137">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="367ea-138">响应</span><span class="sxs-lookup"><span data-stu-id="367ea-138">Response</span></span>
<span data-ttu-id="367ea-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="367ea-139">Here is an example of the response.</span></span> 

><span data-ttu-id="367ea-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="367ea-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests",
    "value": [
        {
            "id": "d75c65d8-9e66-44ff-b1cd-1ab0947fde1d",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": "",
            "type": "UserRemove",
            "assignmentState": "Active",
            "requestedDateTime": "2018-01-09T23:41:34.367Z",
            "roleAssignmentStartDateTime": null,
            "roleAssignmentEndDateTime": null,
            "reason": "Deactivation request",
            "schedule": null,
            "status": {
                "status": "Closed",
                "subStatus": "Revoked",
                "statusDetails": []
            }
        },
        {
            "id": "38f42071-3e81-4191-8c0b-11450fb6b547",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": "",
            "type": "UserAdd",
            "assignmentState": "Active",
            "requestedDateTime": "2018-01-10T20:58:09.163Z",
            "roleAssignmentStartDateTime": "2018-01-10T20:58:11.363Z",
            "roleAssignmentEndDateTime": "2018-01-11T01:58:11.363914Z",
            "reason": "test activations",
            "status": {
                "status": "Closed",
                "subStatus": "Provisioned",
                "statusDetails": [
                    {
                        "key": "EligibilityRule",
                        "value": "Grant"
                    },
                    {
                        "key": "ExpirationRule",
                        "value": "Grant"
                    },
                    {
                        "key": "MfaRule",
                        "value": "Grant"
                    },
                    {
                        "key": "JustificationRule",
                        "value": "Grant"
                    },
                    {
                        "key": "ActivationDayRule",
                        "value": "Grant"
                    },
                    {
                        "key": "ApprovalRule",
                        "value": "Grant"
                    }
                ]
            },
            "schedule": {
                "type": "Once",
                "startDateTime": "2018-01-10T20:58:11.363914Z",
                "endDateTime": "0001-01-01T00:00:00Z",
                "duration": "PT5H"
            }
        },
        ...
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
