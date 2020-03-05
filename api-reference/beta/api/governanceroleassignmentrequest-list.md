---
title: 列出 governanceRoleAssignmentRequests
description: '检索 governanceRoleAssignmentRequests 的集合。 '
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 69dddf7e6073412c2398769165e52c530a3a68e1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42421058"
---
# <a name="list-governanceroleassignmentrequests"></a><span data-ttu-id="8d7c1-103">列出 governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="8d7c1-103">List governanceRoleAssignmentRequests</span></span>

<span data-ttu-id="8d7c1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8d7c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d7c1-105">检索[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="8d7c1-105">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="8d7c1-106">权限</span><span class="sxs-lookup"><span data-stu-id="8d7c1-106">Permissions</span></span>
<span data-ttu-id="8d7c1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d7c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d7c1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d7c1-109">Permission type</span></span>      | <span data-ttu-id="8d7c1-110">权限</span><span class="sxs-lookup"><span data-stu-id="8d7c1-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d7c1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d7c1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8d7c1-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="8d7c1-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="8d7c1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d7c1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d7c1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d7c1-114">Not supported.</span></span>    |
|<span data-ttu-id="8d7c1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d7c1-115">Application</span></span> | <span data-ttu-id="8d7c1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d7c1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d7c1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d7c1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="8d7c1-118">列出资源上的[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="8d7c1-118">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource.</span></span>
    
><span data-ttu-id="8d7c1-119">**注意：** 除了权限范围之外，该请求还要求请求者在资源上至少有一个角色分配。</span><span class="sxs-lookup"><span data-stu-id="8d7c1-119">**Note:** Besides the permission scope, the request requires the requestor to have at least one role assignment on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignmentRequests
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="8d7c1-120">列出地雷的[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="8d7c1-120">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=subjectId+eq+'{myId}'
```

<span data-ttu-id="8d7c1-121">列出作为等待管理员决策的[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="8d7c1-121">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are pending administrator decisions.</span></span>
    
><span data-ttu-id="8d7c1-122">**注意：** 除了权限范围之外，此请求还要求请求者在资源上至少`Active`有一个管理员角色`owner`分配`user access administrator`（或）。</span><span class="sxs-lookup"><span data-stu-id="8d7c1-122">**Note:** Besides the permission scope, this request requires the requestor to have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=status/subStatus+eq+'PendingAdminDecision'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d7c1-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8d7c1-123">Optional query parameters</span></span>
<span data-ttu-id="8d7c1-124">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8d7c1-124">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d7c1-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d7c1-125">Request headers</span></span>
| <span data-ttu-id="8d7c1-126">名称</span><span class="sxs-lookup"><span data-stu-id="8d7c1-126">Name</span></span>      |<span data-ttu-id="8d7c1-127">说明</span><span class="sxs-lookup"><span data-stu-id="8d7c1-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8d7c1-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d7c1-128">Authorization</span></span>  | <span data-ttu-id="8d7c1-129">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8d7c1-129">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d7c1-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d7c1-130">Request body</span></span>
<span data-ttu-id="8d7c1-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8d7c1-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d7c1-132">响应</span><span class="sxs-lookup"><span data-stu-id="8d7c1-132">Response</span></span>
<span data-ttu-id="8d7c1-133">如果成功，此方法在响应`200 OK`正文中返回响应代码和[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="8d7c1-133">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d7c1-134">示例</span><span class="sxs-lookup"><span data-stu-id="8d7c1-134">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequests"
}-->
<span data-ttu-id="8d7c1-135">管理员查询挂起的订阅 Wingtip 玩具的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="8d7c1-135">Administrators query pending role assignment requests for subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="8d7c1-136">请求</span><span class="sxs-lookup"><span data-stu-id="8d7c1-136">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="8d7c1-137">响应</span><span class="sxs-lookup"><span data-stu-id="8d7c1-137">Response</span></span>
<span data-ttu-id="8d7c1-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8d7c1-138">Here is an example of the response.</span></span> 

><span data-ttu-id="8d7c1-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8d7c1-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
