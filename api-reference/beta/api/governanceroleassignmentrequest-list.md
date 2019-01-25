---
title: 列表 governanceRoleAssignmentRequests
description: '检索 governanceRoleAssignmentRequests 的集合。 '
localization_priority: Normal
ms.openlocfilehash: 5ad26ef352eae93e9c804cfb62f5d00df12e32ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515459"
---
# <a name="list-governanceroleassignmentrequests"></a><span data-ttu-id="ae251-103">列表 governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="ae251-103">List governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae251-104">检索[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="ae251-104">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="ae251-105">权限</span><span class="sxs-lookup"><span data-stu-id="ae251-105">Permissions</span></span>
<span data-ttu-id="ae251-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae251-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae251-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae251-108">Permission type</span></span>      | <span data-ttu-id="ae251-109">权限</span><span class="sxs-lookup"><span data-stu-id="ae251-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae251-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae251-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae251-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="ae251-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="ae251-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae251-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae251-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae251-113">Not supported.</span></span>    |
|<span data-ttu-id="ae251-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae251-114">Application</span></span> | <span data-ttu-id="ae251-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="ae251-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae251-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae251-116">HTTP request</span></span>
<span data-ttu-id="ae251-117"><!-- { "blockType": "ignored" } -->列出[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)对资源的集合。</span><span class="sxs-lookup"><span data-stu-id="ae251-117"><!-- { "blockType": "ignored" } --> List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource.</span></span>
    
><span data-ttu-id="ae251-118">**注意：** 除了权限范围，该请求需要具有至少一个角色分配对资源的请求程序。</span><span class="sxs-lookup"><span data-stu-id="ae251-118">**Note:** Besides the permission scope, the request requires the requestor to have at least one role assignment on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignmentRequests
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="ae251-119">列出的[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)我的集合。</span><span class="sxs-lookup"><span data-stu-id="ae251-119">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=subjectId+eq+'{myId}'
```

<span data-ttu-id="ae251-120">列出的[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)挂起管理员决策的集合。</span><span class="sxs-lookup"><span data-stu-id="ae251-120">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are pending administrator decisions.</span></span>
    
><span data-ttu-id="ae251-121">**注意：** 除了权限范围，此请求需要请求程序至少有一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="ae251-121">**Note:** Besides the permission scope, this request requires the requestor to have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=status/subStatus+eq+'PendingAdminDecision'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae251-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ae251-122">Optional query parameters</span></span>
<span data-ttu-id="ae251-123">此方法支持[OData 查询参数](/graph/query-parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="ae251-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae251-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae251-124">Request headers</span></span>
| <span data-ttu-id="ae251-125">名称</span><span class="sxs-lookup"><span data-stu-id="ae251-125">Name</span></span>      |<span data-ttu-id="ae251-126">说明</span><span class="sxs-lookup"><span data-stu-id="ae251-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ae251-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae251-127">Authorization</span></span>  | <span data-ttu-id="ae251-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ae251-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae251-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae251-129">Request body</span></span>
<span data-ttu-id="ae251-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ae251-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae251-131">响应</span><span class="sxs-lookup"><span data-stu-id="ae251-131">Response</span></span>
<span data-ttu-id="ae251-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="ae251-132">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae251-133">示例</span><span class="sxs-lookup"><span data-stu-id="ae251-133">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequests"
}-->
<span data-ttu-id="ae251-134">管理员查询订阅 Wingtip Toys-prod 移待处理的角色分配请求。</span><span class="sxs-lookup"><span data-stu-id="ae251-134">Administrators query pending role assignment requests for subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="ae251-135">请求</span><span class="sxs-lookup"><span data-stu-id="ae251-135">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="ae251-136">响应</span><span class="sxs-lookup"><span data-stu-id="ae251-136">Response</span></span>
<span data-ttu-id="ae251-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ae251-137">Here is an example of the response.</span></span> 

><span data-ttu-id="ae251-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ae251-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
